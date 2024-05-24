# Comparing `tmp/dgenerate-3.5.0.tar.gz` & `tmp/dgenerate-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgenerate-3.5.0.tar", last modified: Thu May 23 14:41:34 2024, max compression
+gzip compressed data, was "dgenerate-3.5.1.tar", last modified: Fri May 24 16:33:01 2024, max compression
```

## Comparing `dgenerate-3.5.0.tar` & `dgenerate-3.5.1.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.697167 dgenerate-3.5.0/
--rw-rw-rw-   0        0        0       26 2024-05-23 14:23:04.000000 dgenerate-3.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0   208673 2024-05-23 14:41:34.696168 dgenerate-3.5.0/PKG-INFO
--rw-rw-rw-   0        0        0   204672 2024-05-23 14:23:04.000000 dgenerate-3.5.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.527639 dgenerate-3.5.0/dgenerate/
--rw-rw-rw-   0        0        0     8240 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/__init__.py
--rw-rw-rw-   0        0        0   107194 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/arguments.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.536145 dgenerate-3.5.0/dgenerate/batchprocess/
--rw-rw-rw-   0        0        0     2079 2024-05-21 21:54:50.000000 dgenerate-3.5.0/dgenerate/batchprocess/__init__.py
--rw-rw-rw-   0        0        0    32568 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/batchprocess/batchprocessor.py
--rw-rw-rw-   0        0        0    50695 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/batchprocess/configrunner.py
--rw-rw-rw-   0        0        0     6910 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/batchprocess/configrunnerplugin.py
--rw-rw-rw-   0        0        0     3212 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/batchprocess/configrunnerpluginloader.py
--rw-rw-rw-   0        0        0     3132 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/batchprocess/image_process_directive.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.541804 dgenerate-3.5.0/dgenerate/console/
--rw-rw-rw-   0        0        0     1627 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/console/__init__.py
--rw-rw-rw-   0        0        0    49785 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/console/console.py
--rw-rw-rw-   0        0        0     2546 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/console/filedialog.py
--rw-rw-rw-   0        0        0    18723 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/console/finddialog.py
--rw-rw-rw-   0        0        0     5174 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/console/karrasschedulerselect.py
--rw-rw-rw-   0        0        0    26243 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/console/recipes.py
--rw-rw-rw-   0        0        0    24390 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/console/recipesform.py
--rw-rw-rw-   0        0        0     4859 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/console/resources.py
--rw-rw-rw-   0        0        0     2804 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/console/scrolledtext.py
--rw-rw-rw-   0        0        0     1897 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/dgenerate.py
--rw-rw-rw-   0        0        0     6090 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/events.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.542805 dgenerate-3.5.0/dgenerate/extras/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.544805 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/
--rw-rw-rw-   0        0        0      599 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.545671 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/canny/
--rw-rw-rw-   0        0        0     1389 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/canny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.547747 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/
--rw-rw-rw-   0        0        0     3087 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.549314 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/__init__.py
--rw-rw-rw-   0        0        0     7710 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py
--rw-rw-rw-   0        0        0    10963 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/util.py
--rw-rw-rw-   0        0        0     4697 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/wholebody.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.550348 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/yolox_config/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/yolox_config/__init__.py
--rw-rw-rw-   0        0        0     7784 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.550868 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/hed/
--rw-rw-rw-   0        0        0     5861 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/hed/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.551902 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/
--rw-rw-rw-   0        0        0     4489 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.556658 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/
--rw-rw-rw-   0        0        0     6440 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/Resnet.py
--rw-rw-rw-   0        0        0     8784 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/Resnext_torch.py
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/__init__.py
--rw-rw-rw-   0        0        0    23459 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/depthmap.py
--rw-rw-rw-   0        0        0     1156 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
--rw-rw-rw-   0        0        0     2099 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/net_tools.py
--rw-rw-rw-   0        0        0    17304 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/network_auxi.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.557700 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.561349 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/
--rw-rw-rw-   0        0        0     3179 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/__init__.py
--rw-rw-rw-   0        0        0    10958 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model.py
--rw-rw-rw-   0        0        0     1718 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model_hg.py
--rw-rw-rw-   0        0        0    29583 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/networks.py
--rw-rw-rw-   0        0        0     7558 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.563438 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/options/
--rw-rw-rw-   0        0        0      137 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/options/__init__.py
--rw-rw-rw-   0        0        0     9520 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/options/base_options.py
--rw-rw-rw-   0        0        0     1084 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/options/test_options.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.564991 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/util/
--rw-rw-rw-   0        0        0       84 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/util/__init__.py
--rw-rw-rw-   0        0        0     3215 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/util/util.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.565507 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/lineart/
--rw-rw-rw-   0        0        0     5972 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/lineart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.566550 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/lineart_anime/
--rw-rw-rw-   0        0        0     8393 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/lineart_anime/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.568097 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mediapipe_face/
--rw-rw-rw-   0        0        0     1997 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mediapipe_face/__init__.py
--rw-rw-rw-   0        0        0     7281 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mediapipe_face/mediapipe_face_common.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.570237 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/
--rw-rw-rw-   0        0        0     3676 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/__init__.py
--rw-rw-rw-   0        0        0     5445 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.575751 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/__init__.py
--rw-rw-rw-   0        0        0      383 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/base_model.py
--rw-rw-rw-   0        0        0     9584 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/blocks.py
--rw-rw-rw-   0        0        0     3263 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/dpt_depth.py
--rw-rw-rw-   0        0        0     2785 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/midas_net.py
--rw-rw-rw-   0        0        0     5334 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/midas_net_custom.py
--rw-rw-rw-   0        0        0     8103 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/transforms.py
--rw-rw-rw-   0        0        0    15116 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/vit.py
--rw-rw-rw-   0        0        0     4771 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.577256 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/
--rw-rw-rw-   0        0        0     2895 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.579262 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/models/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/models/__init__.py
--rw-rw-rw-   0        0        0     9969 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-rw-rw-   0        0        0     9454 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-rw-   0        0        0    24773 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.579262 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/
--rw-rw-rw-   0        0        0     3755 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.581261 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/
--rw-rw-rw-   0        0        0      618 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/NNET.py
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/__init__.py
--rw-rw-rw-   0        0        0     3065 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/baseline.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.584262 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/__init__.py
--rw-rw-rw-   0        0        0    10682 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/decoder.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.594901 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
--rw-rw-rw-   0        0        0     2493 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
--rw-rw-rw-   0        0        0     6131 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.604025 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
--rw-rw-rw-   0        0        0      210 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.607530 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
--rw-rw-rw-   0        0        0     4307 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
--rw-rw-rw-   0        0        0     2792 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
--rw-rw-rw-   0        0        0     2373 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
--rw-rw-rw-   0        0        0     4723 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
--rw-rw-rw-   0        0        0     3473 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
--rw-rw-rw-   0        0        0    12397 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
--rw-rw-rw-   0        0        0    27197 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
--rw-rw-rw-   0        0        0    61375 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
--rw-rw-rw-   0        0        0     2904 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
--rw-rw-rw-   0        0        0    15373 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
--rw-rw-rw-   0        0        0      734 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
--rw-rw-rw-   0        0        0       23 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
--rw-rw-rw-   0        0        0     2814 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
--rw-rw-rw-   0        0        0     5941 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
--rw-rw-rw-   0        0        0     3016 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
--rw-rw-rw-   0        0        0      870 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
--rw-rw-rw-   0        0        0     5017 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
--rw-rw-rw-   0        0        0     1784 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
--rw-rw-rw-   0        0        0     1349 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
--rw-rw-rw-   0        0        0     6798 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
--rw-rw-rw-   0        0        0     1094 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/encoder.py
--rw-rw-rw-   0        0        0     5842 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/submodules.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.612537 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/
--rw-rw-rw-   0        0        0     9711 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/__init__.py
--rw-rw-rw-   0        0        0    12688 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/body.py
--rw-rw-rw-   0        0        0    13854 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/face.py
--rw-rw-rw-   0        0        0     3299 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/hand.py
--rw-rw-rw-   0        0        0     8960 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/model.py
--rw-rw-rw-   0        0        0    14125 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/util.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.614537 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/pidi/
--rw-rw-rw-   0        0        0     3215 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/pidi/__init__.py
--rw-rw-rw-   0        0        0    22524 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/pidi/model.py
--rw-rw-rw-   0        0        0     6407 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/processor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.618650 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/
--rw-rw-rw-   0        0        0     3456 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/__init__.py
--rw-rw-rw-   0        0        0    15520 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/automatic_mask_generator.py
--rw-rw-rw-   0        0        0     4854 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/build_sam.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.625648 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/
--rw-rw-rw-   0        0        0      431 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/__init__.py
--rw-rw-rw-   0        0        0     1522 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/common.py
--rw-rw-rw-   0        0        0    14815 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/image_encoder.py
--rw-rw-rw-   0        0        0     6791 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/mask_decoder.py
--rw-rw-rw-   0        0        0     8808 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/prompt_encoder.py
--rw-rw-rw-   0        0        0     7458 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/sam.py
--rw-rw-rw-   0        0        0    25423 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py
--rw-rw-rw-   0        0        0     8637 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/transformer.py
--rw-rw-rw-   0        0        0    11902 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/predictor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.628157 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/utils/
--rw-rw-rw-   0        0        0      202 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/utils/__init__.py
--rw-rw-rw-   0        0        0    13058 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/utils/amg.py
--rw-rw-rw-   0        0        0     5956 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/utils/onnx.py
--rw-rw-rw-   0        0        0     4074 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/utils/transforms.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.629166 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/shuffle/
--rw-rw-rw-   0        0        0     3430 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/shuffle/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.630165 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/tests/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/tests/__init__.py
--rw-rw-rw-   0        0        0     3083 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/tests/test_processor.py
--rw-rw-rw-   0        0        0     1858 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/tests/test_processor_pytest.py
--rw-rw-rw-   0        0        0     5580 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/util.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.631717 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/
--rw-rw-rw-   0        0        0     2997 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.631717 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.634723 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/
--rw-rw-rw-   0        0        0     1178 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.635723 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/
--rw-rw-rw-   0        0        0     1178 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
--rw-rw-rw-   0        0        0    15627 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.636723 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
--rw-rw-rw-   0        0        0    14192 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.643232 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.649333 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
--rw-rw-rw-   0        0        0     7105 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
--rw-rw-rw-   0        0        0     3542 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
--rw-rw-rw-   0        0        0     1084 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
--rw-rw-rw-   0        0        0      346 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
--rw-rw-rw-   0        0        0      965 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
--rw-rw-rw-   0        0        0     1628 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
--rw-rw-rw-   0        0        0     7533 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
--rw-rw-rw-   0        0        0     7120 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
--rw-rw-rw-   0        0        0      383 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
--rw-rw-rw-   0        0        0    13231 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
--rw-rw-rw-   0        0        0     6265 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
--rw-rw-rw-   0        0        0     2785 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
--rw-rw-rw-   0        0        0     5334 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
--rw-rw-rw-   0        0        0     8794 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
--rw-rw-rw-   0        0        0     8103 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
--rw-rw-rw-   0        0        0     2441 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/builder.py
--rw-rw-rw-   0        0        0     7513 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/depth_model.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.653333 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/
--rw-rw-rw-   0        0        0     1176 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
--rw-rw-rw-   0        0        0     8901 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
--rw-rw-rw-   0        0        0     4959 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
--rw-rw-rw-   0        0        0     6901 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
--rw-rw-rw-   0        0        0     4254 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
--rw-rw-rw-   0        0        0     3529 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/model_io.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.655332 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/
--rw-rw-rw-   0        0        0     1300 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
--rw-rw-rw-   0        0        0    12880 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.657329 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
--rw-rw-rw-   0        0        0     1306 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
--rw-rw-rw-   0        0        0    16596 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.658833 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/
--rw-rw-rw-   0        0        0     1178 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/__init__.py
--rw-rw-rw-   0        0        0      657 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
--rw-rw-rw-   0        0        0    16747 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/config.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.659839 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/
--rw-rw-rw-   0        0        0     3583 2024-04-16 05:15:22.000000 dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
--rw-rw-rw-   0        0        0    17835 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/filecache.py
--rw-rw-rw-   0        0        0     5825 2024-04-13 06:02:43.000000 dgenerate-3.5.0/dgenerate/filelock.py
--rw-rw-rw-   0        0        0     4830 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/files.py
--rw-rw-rw-   0        0        0    40096 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/icon.ico
--rw-rw-rw-   0        0        0     7189 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/image.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.663440 dgenerate-3.5.0/dgenerate/image_process/
--rw-rw-rw-   0        0        0     2588 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/image_process/__init__.py
--rw-rw-rw-   0        0        0    10254 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/image_process/arguments.py
--rw-rw-rw-   0        0        0     7831 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/image_process/invoker.py
--rw-rw-rw-   0        0        0    20004 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/image_process/renderloop.py
--rw-rw-rw-   0        0        0     7986 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/image_process/renderloopconfig.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.677528 dgenerate-3.5.0/dgenerate/imageprocessors/
--rw-rw-rw-   0        0        0     4055 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/__init__.py
--rw-rw-rw-   0        0        0    12211 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/canny.py
--rw-rw-rw-   0        0        0     1952 2023-12-14 08:15:38.000000 dgenerate-3.5.0/dgenerate/imageprocessors/exceptions.py
--rw-rw-rw-   0        0        0     9077 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/hed.py
--rw-rw-rw-   0        0        0     7531 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/imageops.py
--rw-rw-rw-   0        0        0    15785 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/imageprocessor.py
--rw-rw-rw-   0        0        0     5308 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/imageprocessorchain.py
--rw-rw-rw-   0        0        0     4777 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/imageprocessorloader.py
--rw-rw-rw-   0        0        0     6313 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/imageprocessormixin.py
--rw-rw-rw-   0        0        0     9582 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/leres.py
--rw-rw-rw-   0        0        0     8078 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/linart_anime.py
--rw-rw-rw-   0        0        0     8101 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/lineart.py
--rw-rw-rw-   0        0        0     8848 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/midas.py
--rw-rw-rw-   0        0        0     8616 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/mlsd.py
--rw-rw-rw-   0        0        0     7558 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/normal_bae.py
--rw-rw-rw-   0        0        0     9273 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/openpose.py
--rw-rw-rw-   0        0        0     8517 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/pidi.py
--rw-rw-rw-   0        0        0     8712 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/sam.py
--rw-rw-rw-   0        0        0    17489 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/imageprocessors/upscaler.py
--rw-rw-rw-   0        0        0    15329 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/invoker.py
--rw-rw-rw-   0        0        0    82944 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/mediainput.py
--rw-rw-rw-   0        0        0     9866 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/mediaoutput.py
--rw-rw-rw-   0        0        0     7701 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/memoize.py
--rw-rw-rw-   0        0        0    12396 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/memory.py
--rw-rw-rw-   0        0        0     6593 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/messages.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.684060 dgenerate-3.5.0/dgenerate/pipelinewrapper/
--rw-rw-rw-   0        0        0     5946 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/pipelinewrapper/__init__.py
--rw-rw-rw-   0        0        0    29441 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/pipelinewrapper/cache.py
--rw-rw-rw-   0        0        0     3515 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/pipelinewrapper/constants.py
--rw-rw-rw-   0        0        0    15329 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/pipelinewrapper/enums.py
--rw-rw-rw-   0        0        0    23954 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/pipelinewrapper/hfutil.py
--rw-rw-rw-   0        0        0    70615 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/pipelinewrapper/pipelines.py
--rw-rw-rw-   0        0        0    71913 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/pipelinewrapper/uris.py
--rw-rw-rw-   0        0        0     2844 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/pipelinewrapper/util.py
--rw-rw-rw-   0        0        0   101143 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/pipelinewrapper/wrapper.py
--rw-rw-rw-   0        0        0    29164 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/plugin.py
--rw-rw-rw-   0        0        0     3519 2023-12-14 08:15:38.000000 dgenerate-3.5.0/dgenerate/prompt.py
--rw-rw-rw-   0        0        0    52254 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/renderloop.py
--rw-rw-rw-   0        0        0    59500 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/renderloopconfig.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.688058 dgenerate-3.5.0/dgenerate/subcommands/
--rw-rw-rw-   0        0        0     3196 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/subcommands/__init__.py
--rw-rw-rw-   0        0        0     1935 2023-12-14 08:15:38.000000 dgenerate-3.5.0/dgenerate/subcommands/exceptions.py
--rw-rw-rw-   0        0        0     2636 2023-12-14 08:15:38.000000 dgenerate-3.5.0/dgenerate/subcommands/image_process.py
--rw-rw-rw-   0        0        0     2536 2023-12-14 08:15:38.000000 dgenerate-3.5.0/dgenerate/subcommands/subcommand.py
--rw-rw-rw-   0        0        0     2727 2024-05-21 21:55:09.000000 dgenerate-3.5.0/dgenerate/subcommands/subcommandloader.py
--rw-rw-rw-   0        0        0    45482 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/textprocessing.py
--rw-rw-rw-   0        0        0    18578 2024-05-23 14:23:04.000000 dgenerate-3.5.0/dgenerate/types.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.692656 dgenerate-3.5.0/dgenerate.egg-info/
--rw-rw-rw-   0        0        0   208673 2024-05-23 14:41:34.000000 dgenerate-3.5.0/dgenerate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13696 2024-05-23 14:41:34.000000 dgenerate-3.5.0/dgenerate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:41:34.000000 dgenerate-3.5.0/dgenerate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-23 14:41:34.000000 dgenerate-3.5.0/dgenerate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1345 2024-05-23 14:41:34.000000 dgenerate-3.5.0/dgenerate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 14:41:34.000000 dgenerate-3.5.0/dgenerate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 14:41:34.697167 dgenerate-3.5.0/setup.cfg
--rw-rw-rw-   0        0        0    10893 2024-05-23 14:23:04.000000 dgenerate-3.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.688058 dgenerate-3.5.0/tests/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.5.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:41:34.691569 dgenerate-3.5.0/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.5.0/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     9682 2023-12-14 08:15:38.000000 dgenerate-3.5.0/tests/unit/concept_uri_parser_test.py
--rw-rw-rw-   0        0        0    10155 2023-12-14 08:15:38.000000 dgenerate-3.5.0/tests/unit/image_seed_parse_test.py
--rw-rw-rw-   0        0        0    18395 2023-12-14 08:15:38.000000 dgenerate-3.5.0/tests/unit/plugin_loading_test.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.493152 dgenerate-3.5.1/
+-rw-rw-rw-   0        0        0       26 2024-05-23 14:23:04.000000 dgenerate-3.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0   208673 2024-05-24 16:33:01.492147 dgenerate-3.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0   204672 2024-05-24 16:31:07.000000 dgenerate-3.5.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.309180 dgenerate-3.5.1/dgenerate/
+-rw-rw-rw-   0        0        0     8240 2024-05-24 16:23:57.000000 dgenerate-3.5.1/dgenerate/__init__.py
+-rw-rw-rw-   0        0        0   107194 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/arguments.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.319691 dgenerate-3.5.1/dgenerate/batchprocess/
+-rw-rw-rw-   0        0        0     2079 2024-05-21 21:54:50.000000 dgenerate-3.5.1/dgenerate/batchprocess/__init__.py
+-rw-rw-rw-   0        0        0    32658 2024-05-24 16:19:56.000000 dgenerate-3.5.1/dgenerate/batchprocess/batchprocessor.py
+-rw-rw-rw-   0        0        0    50695 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/batchprocess/configrunner.py
+-rw-rw-rw-   0        0        0     6910 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/batchprocess/configrunnerplugin.py
+-rw-rw-rw-   0        0        0     3212 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/batchprocess/configrunnerpluginloader.py
+-rw-rw-rw-   0        0        0     3132 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/batchprocess/image_process_directive.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.326208 dgenerate-3.5.1/dgenerate/console/
+-rw-rw-rw-   0        0        0     1627 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/console/__init__.py
+-rw-rw-rw-   0        0        0    49785 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/console/console.py
+-rw-rw-rw-   0        0        0     2546 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/console/filedialog.py
+-rw-rw-rw-   0        0        0    18723 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/console/finddialog.py
+-rw-rw-rw-   0        0        0     5174 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/console/karrasschedulerselect.py
+-rw-rw-rw-   0        0        0    26243 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/console/recipes.py
+-rw-rw-rw-   0        0        0    24390 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/console/recipesform.py
+-rw-rw-rw-   0        0        0     4859 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/console/resources.py
+-rw-rw-rw-   0        0        0     2804 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/console/scrolledtext.py
+-rw-rw-rw-   0        0        0     1897 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/dgenerate.py
+-rw-rw-rw-   0        0        0     6090 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/events.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.326208 dgenerate-3.5.1/dgenerate/extras/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.328209 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/
+-rw-rw-rw-   0        0        0      599 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.329209 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/canny/
+-rw-rw-rw-   0        0        0     1389 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/canny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.331206 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/
+-rw-rw-rw-   0        0        0     3087 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.332711 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/__init__.py
+-rw-rw-rw-   0        0        0     7710 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py
+-rw-rw-rw-   0        0        0    10963 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/util.py
+-rw-rw-rw-   0        0        0     4697 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/wholebody.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.333719 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/yolox_config/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/yolox_config/__init__.py
+-rw-rw-rw-   0        0        0     7784 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.334717 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/hed/
+-rw-rw-rw-   0        0        0     5861 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/hed/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.335718 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/
+-rw-rw-rw-   0        0        0     4489 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.339719 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/
+-rw-rw-rw-   0        0        0     6440 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/Resnet.py
+-rw-rw-rw-   0        0        0     8784 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/Resnext_torch.py
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/__init__.py
+-rw-rw-rw-   0        0        0    23459 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/depthmap.py
+-rw-rw-rw-   0        0        0     1156 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
+-rw-rw-rw-   0        0        0     2099 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/net_tools.py
+-rw-rw-rw-   0        0        0    17304 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/network_auxi.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.340717 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.345233 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/
+-rw-rw-rw-   0        0        0     3179 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/__init__.py
+-rw-rw-rw-   0        0        0    10958 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model.py
+-rw-rw-rw-   0        0        0     1718 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model_hg.py
+-rw-rw-rw-   0        0        0    29583 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/networks.py
+-rw-rw-rw-   0        0        0     7558 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.347233 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/options/
+-rw-rw-rw-   0        0        0      137 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/options/__init__.py
+-rw-rw-rw-   0        0        0     9520 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/options/base_options.py
+-rw-rw-rw-   0        0        0     1084 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/options/test_options.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.348233 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/util/
+-rw-rw-rw-   0        0        0       84 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/util/__init__.py
+-rw-rw-rw-   0        0        0     3215 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/util/util.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.349233 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/lineart/
+-rw-rw-rw-   0        0        0     5972 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/lineart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.349233 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/lineart_anime/
+-rw-rw-rw-   0        0        0     8393 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/lineart_anime/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.351233 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mediapipe_face/
+-rw-rw-rw-   0        0        0     1997 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mediapipe_face/__init__.py
+-rw-rw-rw-   0        0        0     7281 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mediapipe_face/mediapipe_face_common.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.353233 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/
+-rw-rw-rw-   0        0        0     3676 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/__init__.py
+-rw-rw-rw-   0        0        0     5445 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.358744 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/__init__.py
+-rw-rw-rw-   0        0        0      383 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/base_model.py
+-rw-rw-rw-   0        0        0     9584 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/blocks.py
+-rw-rw-rw-   0        0        0     3263 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/dpt_depth.py
+-rw-rw-rw-   0        0        0     2785 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/midas_net.py
+-rw-rw-rw-   0        0        0     5334 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8103 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/transforms.py
+-rw-rw-rw-   0        0        0    15116 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/vit.py
+-rw-rw-rw-   0        0        0     4771 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.360743 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/
+-rw-rw-rw-   0        0        0     2895 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.362744 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/models/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/models/__init__.py
+-rw-rw-rw-   0        0        0     9969 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-rw-   0        0        0     9454 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-rw-   0        0        0    24773 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.363743 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/
+-rw-rw-rw-   0        0        0     3755 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.365255 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/
+-rw-rw-rw-   0        0        0      618 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/NNET.py
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/__init__.py
+-rw-rw-rw-   0        0        0     3065 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/baseline.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.367254 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/__init__.py
+-rw-rw-rw-   0        0        0    10682 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/decoder.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.375765 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
+-rw-rw-rw-   0        0        0     2493 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
+-rw-rw-rw-   0        0        0     6131 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.390877 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
+-rw-rw-rw-   0        0        0      210 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.395379 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
+-rw-rw-rw-   0        0        0     4307 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
+-rw-rw-rw-   0        0        0     2792 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
+-rw-rw-rw-   0        0        0     2373 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
+-rw-rw-rw-   0        0        0     4723 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
+-rw-rw-rw-   0        0        0     3473 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
+-rw-rw-rw-   0        0        0    12397 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
+-rw-rw-rw-   0        0        0    27197 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
+-rw-rw-rw-   0        0        0    61375 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
+-rw-rw-rw-   0        0        0     2904 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
+-rw-rw-rw-   0        0        0    15373 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
+-rw-rw-rw-   0        0        0      734 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
+-rw-rw-rw-   0        0        0       23 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
+-rw-rw-rw-   0        0        0     2814 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
+-rw-rw-rw-   0        0        0     5941 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
+-rw-rw-rw-   0        0        0     3016 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
+-rw-rw-rw-   0        0        0      870 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
+-rw-rw-rw-   0        0        0     5017 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
+-rw-rw-rw-   0        0        0     1784 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
+-rw-rw-rw-   0        0        0     1349 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
+-rw-rw-rw-   0        0        0     6798 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
+-rw-rw-rw-   0        0        0     1094 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/encoder.py
+-rw-rw-rw-   0        0        0     5842 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/submodules.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.399387 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/
+-rw-rw-rw-   0        0        0     9711 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/__init__.py
+-rw-rw-rw-   0        0        0    12688 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/body.py
+-rw-rw-rw-   0        0        0    13854 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/face.py
+-rw-rw-rw-   0        0        0     3299 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/hand.py
+-rw-rw-rw-   0        0        0     8960 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/model.py
+-rw-rw-rw-   0        0        0    14125 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/util.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.401387 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/pidi/
+-rw-rw-rw-   0        0        0     3215 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/pidi/__init__.py
+-rw-rw-rw-   0        0        0    22524 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/pidi/model.py
+-rw-rw-rw-   0        0        0     6407 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/processor.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.404387 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/
+-rw-rw-rw-   0        0        0     3456 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/__init__.py
+-rw-rw-rw-   0        0        0    15520 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/automatic_mask_generator.py
+-rw-rw-rw-   0        0        0     4854 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/build_sam.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.411906 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/
+-rw-rw-rw-   0        0        0      431 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/__init__.py
+-rw-rw-rw-   0        0        0     1522 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/common.py
+-rw-rw-rw-   0        0        0    14815 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/image_encoder.py
+-rw-rw-rw-   0        0        0     6791 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/mask_decoder.py
+-rw-rw-rw-   0        0        0     8808 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/prompt_encoder.py
+-rw-rw-rw-   0        0        0     7458 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/sam.py
+-rw-rw-rw-   0        0        0    25423 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py
+-rw-rw-rw-   0        0        0     8637 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/transformer.py
+-rw-rw-rw-   0        0        0    11902 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/predictor.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.414902 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/utils/
+-rw-rw-rw-   0        0        0      202 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/utils/__init__.py
+-rw-rw-rw-   0        0        0    13058 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/utils/amg.py
+-rw-rw-rw-   0        0        0     5956 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/utils/onnx.py
+-rw-rw-rw-   0        0        0     4074 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/utils/transforms.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.415903 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/shuffle/
+-rw-rw-rw-   0        0        0     3430 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/shuffle/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.417415 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/tests/__init__.py
+-rw-rw-rw-   0        0        0     3083 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/tests/test_processor.py
+-rw-rw-rw-   0        0        0     1858 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/tests/test_processor_pytest.py
+-rw-rw-rw-   0        0        0     5580 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/util.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.418415 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/
+-rw-rw-rw-   0        0        0     2997 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.419415 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.422413 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/
+-rw-rw-rw-   0        0        0     1178 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.423414 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/
+-rw-rw-rw-   0        0        0     1178 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
+-rw-rw-rw-   0        0        0    15627 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.425415 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
+-rw-rw-rw-   0        0        0    14192 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.431928 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.440445 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
+-rw-rw-rw-   0        0        0     7105 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
+-rw-rw-rw-   0        0        0     3542 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
+-rw-rw-rw-   0        0        0     1084 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
+-rw-rw-rw-   0        0        0      346 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
+-rw-rw-rw-   0        0        0      965 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
+-rw-rw-rw-   0        0        0     1628 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
+-rw-rw-rw-   0        0        0     7533 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
+-rw-rw-rw-   0        0        0     7120 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
+-rw-rw-rw-   0        0        0      383 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
+-rw-rw-rw-   0        0        0    13231 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
+-rw-rw-rw-   0        0        0     6265 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
+-rw-rw-rw-   0        0        0     2785 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
+-rw-rw-rw-   0        0        0     5334 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8794 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
+-rw-rw-rw-   0        0        0     8103 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
+-rw-rw-rw-   0        0        0     2441 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/builder.py
+-rw-rw-rw-   0        0        0     7513 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/depth_model.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.444445 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/
+-rw-rw-rw-   0        0        0     1176 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
+-rw-rw-rw-   0        0        0     8901 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
+-rw-rw-rw-   0        0        0     4959 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
+-rw-rw-rw-   0        0        0     6901 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
+-rw-rw-rw-   0        0        0     4254 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
+-rw-rw-rw-   0        0        0     3529 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/model_io.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.445444 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/
+-rw-rw-rw-   0        0        0     1300 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
+-rw-rw-rw-   0        0        0    12880 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.447446 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
+-rw-rw-rw-   0        0        0     1306 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
+-rw-rw-rw-   0        0        0    16596 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.449959 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/
+-rw-rw-rw-   0        0        0     1178 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/__init__.py
+-rw-rw-rw-   0        0        0      657 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
+-rw-rw-rw-   0        0        0    16747 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/config.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.450960 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/
+-rw-rw-rw-   0        0        0     3583 2024-04-16 05:15:22.000000 dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
+-rw-rw-rw-   0        0        0    17835 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/filecache.py
+-rw-rw-rw-   0        0        0     5825 2024-04-13 06:02:43.000000 dgenerate-3.5.1/dgenerate/filelock.py
+-rw-rw-rw-   0        0        0     4830 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/files.py
+-rw-rw-rw-   0        0        0    40096 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/icon.ico
+-rw-rw-rw-   0        0        0     7189 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/image.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.453959 dgenerate-3.5.1/dgenerate/image_process/
+-rw-rw-rw-   0        0        0     2588 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/image_process/__init__.py
+-rw-rw-rw-   0        0        0    10254 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/image_process/arguments.py
+-rw-rw-rw-   0        0        0     7831 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/image_process/invoker.py
+-rw-rw-rw-   0        0        0    20004 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/image_process/renderloop.py
+-rw-rw-rw-   0        0        0     7986 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/image_process/renderloopconfig.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.469635 dgenerate-3.5.1/dgenerate/imageprocessors/
+-rw-rw-rw-   0        0        0     4055 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/__init__.py
+-rw-rw-rw-   0        0        0    12211 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/canny.py
+-rw-rw-rw-   0        0        0     1952 2023-12-14 08:15:38.000000 dgenerate-3.5.1/dgenerate/imageprocessors/exceptions.py
+-rw-rw-rw-   0        0        0     9077 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/hed.py
+-rw-rw-rw-   0        0        0     7531 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/imageops.py
+-rw-rw-rw-   0        0        0    15785 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/imageprocessor.py
+-rw-rw-rw-   0        0        0     5308 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/imageprocessorchain.py
+-rw-rw-rw-   0        0        0     4777 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/imageprocessorloader.py
+-rw-rw-rw-   0        0        0     6313 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/imageprocessormixin.py
+-rw-rw-rw-   0        0        0     9582 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/leres.py
+-rw-rw-rw-   0        0        0     8078 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/linart_anime.py
+-rw-rw-rw-   0        0        0     8101 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/lineart.py
+-rw-rw-rw-   0        0        0     8848 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/midas.py
+-rw-rw-rw-   0        0        0     8616 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/mlsd.py
+-rw-rw-rw-   0        0        0     7558 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/normal_bae.py
+-rw-rw-rw-   0        0        0     9273 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/openpose.py
+-rw-rw-rw-   0        0        0     8517 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/pidi.py
+-rw-rw-rw-   0        0        0     8712 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/sam.py
+-rw-rw-rw-   0        0        0    17489 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/imageprocessors/upscaler.py
+-rw-rw-rw-   0        0        0    15329 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/invoker.py
+-rw-rw-rw-   0        0        0    82944 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/mediainput.py
+-rw-rw-rw-   0        0        0     9866 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/mediaoutput.py
+-rw-rw-rw-   0        0        0     7701 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/memoize.py
+-rw-rw-rw-   0        0        0    12396 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/memory.py
+-rw-rw-rw-   0        0        0     6593 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.477636 dgenerate-3.5.1/dgenerate/pipelinewrapper/
+-rw-rw-rw-   0        0        0     5946 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/pipelinewrapper/__init__.py
+-rw-rw-rw-   0        0        0    29441 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/pipelinewrapper/cache.py
+-rw-rw-rw-   0        0        0     3515 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/pipelinewrapper/constants.py
+-rw-rw-rw-   0        0        0    15329 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/pipelinewrapper/enums.py
+-rw-rw-rw-   0        0        0    23954 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/pipelinewrapper/hfutil.py
+-rw-rw-rw-   0        0        0    70615 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/pipelinewrapper/pipelines.py
+-rw-rw-rw-   0        0        0    71913 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/pipelinewrapper/uris.py
+-rw-rw-rw-   0        0        0     2844 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/pipelinewrapper/util.py
+-rw-rw-rw-   0        0        0   101143 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/pipelinewrapper/wrapper.py
+-rw-rw-rw-   0        0        0    29164 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/plugin.py
+-rw-rw-rw-   0        0        0     3519 2023-12-14 08:15:38.000000 dgenerate-3.5.1/dgenerate/prompt.py
+-rw-rw-rw-   0        0        0    52254 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/renderloop.py
+-rw-rw-rw-   0        0        0    59500 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/renderloopconfig.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.482148 dgenerate-3.5.1/dgenerate/subcommands/
+-rw-rw-rw-   0        0        0     3196 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/subcommands/__init__.py
+-rw-rw-rw-   0        0        0     1935 2023-12-14 08:15:38.000000 dgenerate-3.5.1/dgenerate/subcommands/exceptions.py
+-rw-rw-rw-   0        0        0     2636 2023-12-14 08:15:38.000000 dgenerate-3.5.1/dgenerate/subcommands/image_process.py
+-rw-rw-rw-   0        0        0     2536 2023-12-14 08:15:38.000000 dgenerate-3.5.1/dgenerate/subcommands/subcommand.py
+-rw-rw-rw-   0        0        0     2727 2024-05-21 21:55:09.000000 dgenerate-3.5.1/dgenerate/subcommands/subcommandloader.py
+-rw-rw-rw-   0        0        0    45482 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/textprocessing.py
+-rw-rw-rw-   0        0        0    18578 2024-05-23 14:23:04.000000 dgenerate-3.5.1/dgenerate/types.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.486147 dgenerate-3.5.1/dgenerate.egg-info/
+-rw-rw-rw-   0        0        0   208673 2024-05-24 16:33:01.000000 dgenerate-3.5.1/dgenerate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13696 2024-05-24 16:33:01.000000 dgenerate-3.5.1/dgenerate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 16:33:01.000000 dgenerate-3.5.1/dgenerate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-24 16:33:01.000000 dgenerate-3.5.1/dgenerate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1345 2024-05-24 16:33:01.000000 dgenerate-3.5.1/dgenerate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-24 16:33:01.000000 dgenerate-3.5.1/dgenerate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 16:33:01.493152 dgenerate-3.5.1/setup.cfg
+-rw-rw-rw-   0        0        0    10893 2024-05-23 14:23:04.000000 dgenerate-3.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.482148 dgenerate-3.5.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.5.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:33:01.485148 dgenerate-3.5.1/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.5.1/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     9682 2023-12-14 08:15:38.000000 dgenerate-3.5.1/tests/unit/concept_uri_parser_test.py
+-rw-rw-rw-   0        0        0    10155 2023-12-14 08:15:38.000000 dgenerate-3.5.1/tests/unit/image_seed_parse_test.py
+-rw-rw-rw-   0        0        0    18395 2023-12-14 08:15:38.000000 dgenerate-3.5.1/tests/unit/plugin_loading_test.py
```

### Comparing `dgenerate-3.5.0/PKG-INFO` & `dgenerate-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2064 6765  : 2.1..Name: dge
 00000020: 6e65 7261 7465 0d0a 5665 7273 696f 6e3a  nerate..Version:
-00000030: 2033 2e35 2e30 0d0a 5375 6d6d 6172 793a   3.5.0..Summary:
+00000030: 2033 2e35 2e31 0d0a 5375 6d6d 6172 793a   3.5.1..Summary:
 00000040: 2042 6174 6368 2069 6d61 6765 2067 656e   Batch image gen
 00000050: 6572 6174 696f 6e20 616e 6420 6d61 6e69  eration and mani
 00000060: 7075 6c61 7469 6f6e 2074 6f6f 6c20 7375  pulation tool su
 00000070: 7070 6f72 7469 6e67 2053 7461 626c 6520  pporting Stable 
 00000080: 4469 6666 7573 696f 6e20 616e 6420 7265  Diffusion and re
 00000090: 6c61 7465 6420 7465 6368 6e69 7175 6573  lated techniques
 000000a0: 202f 2061 6c67 6f72 6974 686d 732c 2077   / algorithms, w
@@ -250,18 +250,18 @@
 00000f90: 2272 6561 6474 6865 646f 6373 220d 0a0d  "readthedocs"...
 00000fa0: 0a2e 2e20 7c44 6f63 756d 656e 7461 7469  ... |Documentati
 00000fb0: 6f6e 2053 7461 7475 737c 2069 6d61 6765  on Status| image
 00000fc0: 3a3a 2068 7474 7073 3a2f 2f72 6561 6474  :: https://readt
 00000fd0: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
 00000fe0: 6374 732f 6467 656e 6572 6174 652f 6261  cts/dgenerate/ba
 00000ff0: 6467 652f 3f76 6572 7369 6f6e 3d76 332e  dge/?version=v3.
-00001000: 352e 300d 0a20 2020 3a74 6172 6765 743a  5.0..   :target:
+00001000: 352e 310d 0a20 2020 3a74 6172 6765 743a  5.1..   :target:
 00001010: 2068 7474 703a 2f2f 6467 656e 6572 6174   http://dgenerat
 00001020: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00001030: 2f65 6e2f 7633 2e35 2e30 2f0d 0a0d 0a4f  /en/v3.5.0/....O
+00001030: 2f65 6e2f 7633 2e35 2e31 2f0d 0a0d 0a4f  /en/v3.5.1/....O
 00001040: 7665 7276 6965 770d 0a3d 3d3d 3d3d 3d3d  verview..=======
 00001050: 3d0d 0a0d 0a7c 446f 6375 6d65 6e74 6174  =....|Documentat
 00001060: 696f 6e20 5374 6174 7573 7c0d 0a0d 0a2a  ion Status|....*
 00001070: 2a64 6765 6e65 7261 7465 2a2a 2069 7320  *dgenerate** is 
 00001080: 6120 636f 6d6d 616e 6420 6c69 6e65 2074  a command line t
 00001090: 6f6f 6c20 616e 6420 6c69 6272 6172 7920  ool and library 
 000010a0: 666f 7220 6765 6e65 7261 7469 6e67 2069  for generating i
@@ -386,15 +386,15 @@
 00001810: 7469 6f6e 7320 6275 7420 6578 7472 616f  tions but extrao
 00001820: 7264 696e 6172 696c 7920 736c 6f77 2e0d  rdinarily slow..
 00001830: 0a0d 0a46 6f72 206c 6962 7261 7279 2064  ...For library d
 00001840: 6f63 756d 656e 7461 7469 6f6e 2076 6973  ocumentation vis
 00001850: 6974 2060 7265 6164 7468 6564 6f63 7320  it `readthedocs 
 00001860: 3c68 7474 703a 2f2f 6467 656e 6572 6174  <http://dgenerat
 00001870: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00001880: 2f65 6e2f 7633 2e35 2e30 2f3e 605f 2e0d  /en/v3.5.0/>`_..
+00001880: 2f65 6e2f 7633 2e35 2e31 2f3e 605f 2e0d  /en/v3.5.1/>`_..
 00001890: 0a0d 0a2d 2d2d 2d0d 0a0d 0a2a 2048 6f77  ...----....* How
 000018a0: 2074 6f20 696e 7374 616c 6c0d 0a20 2020   to install..   
 000018b0: 202a 2060 5769 6e64 6f77 7320 496e 7374   * `Windows Inst
 000018c0: 616c 6c60 5f0d 0a20 2020 202a 2060 4c69  all`_..    * `Li
 000018d0: 6e75 7820 6f72 2057 534c 2049 6e73 7461  nux or WSL Insta
 000018e0: 6c6c 605f 0d0a 0d0a 2a20 5573 6167 6520  ll`_....* Usage 
 000018f0: 4578 616d 706c 6573 0d0a 2020 2020 2a20  Examples..    * 
@@ -4920,15 +4920,15 @@
 00013370: 2020 2020 2020 2020 2020 2275 7365 645f            "used_
 00013380: 7065 7263 656e 7420 3e20 3730 2220 466f  percent > 70" Fo
 00013390: 7220 5379 6e74 6178 2053 6565 3a20 5b68  r Syntax See: [h
 000133a0: 7474 7073 3a2f 2f64 6765 6e65 7261 7465  ttps://dgenerate
 000133b0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
 000133c0: 656e 2f76 0d0a 2020 2020 2020 2020 2020  en/v..          
 000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 2020 332e 352e 302f 6467 656e 6572 6174    3.5.0/dgenerat
+000133e0: 2020 332e 352e 312f 6467 656e 6572 6174    3.5.1/dgenerat
 000133f0: 655f 7375 626d 6f64 756c 6573 2e68 746d  e_submodules.htm
 00013400: 6c23 6467 656e 6572 6174 652e 7069 7065  l#dgenerate.pipe
 00013410: 6c69 6e65 7772 6170 7065 722e 4341 4348  linewrapper.CACH
 00013420: 455f 4d45 4d4f 5259 5f43 4f4e 0d0a 2020  E_MEMORY_CON..  
 00013430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013440: 2020 2020 2020 2020 2020 5354 5241 494e            STRAIN
 00013450: 5453 5d0d 0a20 2020 2020 202d 706d 6320  TS]..      -pmc 
@@ -4973,15 +4973,15 @@
 000136c0: 6520 3e20 2861 7661 696c 6162 6c65 202a  e > (available *
 000136d0: 2030 2e37 3529 2220 466f 7220 5379 6e74   0.75)" For Synt
 000136e0: 6178 2053 6565 3a20 5b68 7474 7073 3a2f  ax See: [https:/
 000136f0: 2f64 6765 6e65 7261 7465 2e72 650d 0a20  /dgenerate.re.. 
 00013700: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013710: 2020 2020 2020 2020 2020 2061 6474 6865             adthe
 00013720: 646f 6373 2e69 6f2f 656e 2f76 332e 352e  docs.io/en/v3.5.
-00013730: 302f 6467 656e 6572 6174 655f 7375 626d  0/dgenerate_subm
+00013730: 312f 6467 656e 6572 6174 655f 7375 626d  1/dgenerate_subm
 00013740: 6f64 756c 6573 2e68 746d 6c23 6467 656e  odules.html#dgen
 00013750: 6572 6174 652e 7069 7065 6c69 6e65 7772  erate.pipelinewr
 00013760: 6170 7065 720d 0a20 2020 2020 2020 2020  apper..         
 00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013780: 2020 202e 5049 5045 4c49 4e45 5f43 4143     .PIPELINE_CAC
 00013790: 4845 5f4d 454d 4f52 595f 434f 4e53 5452  HE_MEMORY_CONSTR
 000137a0: 4149 4e54 535d 0d0a 2020 2020 2020 2d75  AINTS]..      -u
@@ -5022,15 +5022,15 @@
 000139d0: 756e 6574 5f73 697a 6520 3e20 2861 7661  unet_size > (ava
 000139e0: 696c 6162 6c65 202a 2030 2e37 3529 2220  ilable * 0.75)" 
 000139f0: 466f 720d 0a20 2020 2020 2020 2020 2020  For..           
 00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a10: 2053 796e 7461 7820 5365 653a 205b 6874   Syntax See: [ht
 00013a20: 7470 733a 2f2f 6467 656e 6572 6174 652e  tps://dgenerate.
 00013a30: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00013a40: 6e2f 7633 2e35 2e30 2f64 6765 6e65 7261  n/v3.5.0/dgenera
+00013a40: 6e2f 7633 2e35 2e31 2f64 6765 6e65 7261  n/v3.5.1/dgenera
 00013a50: 7465 5f73 7562 6d6f 6475 6c0d 0a20 2020  te_submodul..   
 00013a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a70: 2020 2020 2020 2020 2065 732e 6874 6d6c           es.html
 00013a80: 2364 6765 6e65 7261 7465 2e70 6970 656c  #dgenerate.pipel
 00013a90: 696e 6577 7261 7070 6572 2e55 4e45 545f  inewrapper.UNET_
 00013aa0: 4341 4348 455f 4d45 4d4f 5259 5f43 4f4e  CACHE_MEMORY_CON
 00013ab0: 5354 5241 494e 5453 5d0d 0a20 2020 2020  STRAINTS]..     
@@ -5071,15 +5071,15 @@
 00013ce0: 6165 5f73 697a 6520 3e20 2861 7661 696c  ae_size > (avail
 00013cf0: 6162 6c65 202a 2030 2e37 3529 2220 466f  able * 0.75)" Fo
 00013d00: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
 00013d10: 2020 2020 2020 2020 2020 2020 2020 2053                 S
 00013d20: 796e 7461 7820 5365 653a 205b 6874 7470  yntax See: [http
 00013d30: 733a 2f2f 6467 656e 6572 6174 652e 7265  s://dgenerate.re
 00013d40: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00013d50: 7633 2e35 2e30 2f64 6765 6e65 7261 7465  v3.5.0/dgenerate
+00013d50: 7633 2e35 2e31 2f64 6765 6e65 7261 7465  v3.5.1/dgenerate
 00013d60: 5f73 7562 6d6f 6475 6c0d 0a20 2020 2020  _submodul..     
 00013d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013d80: 2020 2020 2020 2065 732e 6874 6d6c 2364         es.html#d
 00013d90: 6765 6e65 7261 7465 2e70 6970 656c 696e  generate.pipelin
 00013da0: 6577 7261 7070 6572 2e56 4145 5f43 4143  ewrapper.VAE_CAC
 00013db0: 4845 5f4d 454d 4f52 595f 434f 4e53 5452  HE_MEMORY_CONSTR
 00013dc0: 4149 4e54 535d 0d0a 2020 2020 2020 2d63  AINTS]..      -c
@@ -5124,15 +5124,15 @@
 00014030: 2020 2020 2020 2020 2028 6176 6169 6c61           (availa
 00014040: 626c 6520 2a20 302e 3735 2922 2046 6f72  ble * 0.75)" For
 00014050: 2053 796e 7461 7820 5365 653a 205b 6874   Syntax See: [ht
 00014060: 7470 733a 2f2f 6467 656e 6572 6174 652e  tps://dgenerate.
 00014070: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
 00014080: 6e2f 760d 0a20 2020 2020 2020 2020 2020  n/v..           
 00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140a0: 2033 2e35 2e30 2f64 6765 6e65 7261 7465   3.5.0/dgenerate
+000140a0: 2033 2e35 2e31 2f64 6765 6e65 7261 7465   3.5.1/dgenerate
 000140b0: 5f73 7562 6d6f 6475 6c65 732e 6874 6d6c  _submodules.html
 000140c0: 2364 6765 6e65 7261 7465 2e70 6970 656c  #dgenerate.pipel
 000140d0: 696e 6577 7261 7070 6572 2e43 4f4e 5452  inewrapper.CONTR
 000140e0: 4f4c 5f4e 4554 5f43 4143 480d 0a20 2020  OL_NET_CACH..   
 000140f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014100: 2020 2020 2020 2020 2045 5f4d 454d 4f52           E_MEMOR
 00014110: 595f 434f 4e53 5452 4149 4e54 535d 0d0a  Y_CONSTRAINTS]..
@@ -5216,27 +5216,27 @@
 000145f0: 6465 782d 7572 6c20 6874 7470 733a 2f2f  dex-url https://
 00014600: 646f 776e 6c6f 6164 2e70 7974 6f72 6368  download.pytorch
 00014610: 2e6f 7267 2f77 686c 2f63 7531 3231 2f22  .org/whl/cu121/"
 00014620: 0d0a 0d0a 2020 2020 2320 4966 2079 6f75  ....    # If you
 00014630: 2077 616e 7420 6120 7370 6563 6966 6963   want a specific
 00014640: 2076 6572 7369 6f6e 0d0a 0d0a 2020 2020   version....    
 00014650: 7069 7078 2069 6e73 7461 6c6c 2064 6765  pipx install dge
-00014660: 6e65 7261 7465 3d3d 332e 352e 3020 5e0d  nerate==3.5.0 ^.
+00014660: 6e65 7261 7465 3d3d 332e 352e 3120 5e0d  nerate==3.5.1 ^.
 00014670: 0a20 2020 202d 2d70 6970 2d61 7267 7320  .    --pip-args 
 00014680: 222d 2d65 7874 7261 2d69 6e64 6578 2d75  "--extra-index-u
 00014690: 726c 2068 7474 7073 3a2f 2f64 6f77 6e6c  rl https://downl
 000146a0: 6f61 642e 7079 746f 7263 682e 6f72 672f  oad.pytorch.org/
 000146b0: 7768 6c2f 6375 3132 312f 220d 0a0d 0a20  whl/cu121/".... 
 000146c0: 2020 2023 2059 6f75 2063 616e 2069 6e73     # You can ins
 000146d0: 7461 6c6c 2077 6974 686f 7574 2070 6970  tall without pip
 000146e0: 7820 696e 746f 2079 6f75 7220 6f77 6e20  x into your own 
 000146f0: 656e 7669 726f 6e6d 656e 7420 6c69 6b65  environment like
 00014700: 2073 6f0d 0a0d 0a20 2020 2070 6970 2069   so....    pip i
 00014710: 6e73 7461 6c6c 2064 6765 6e65 7261 7465  nstall dgenerate
-00014720: 3d3d 332e 352e 3020 2d2d 6578 7472 612d  ==3.5.0 --extra-
+00014720: 3d3d 332e 352e 3120 2d2d 6578 7472 612d  ==3.5.1 --extra-
 00014730: 696e 6465 782d 7572 6c20 6874 7470 733a  index-url https:
 00014740: 2f2f 646f 776e 6c6f 6164 2e70 7974 6f72  //download.pytor
 00014750: 6368 2e6f 7267 2f77 686c 2f63 7531 3231  ch.org/whl/cu121
 00014760: 2f0d 0a0d 0a0d 0a49 7420 6973 2072 6563  /......It is rec
 00014770: 6f6d 6d65 6e64 6564 2074 6f20 696e 7374  ommended to inst
 00014780: 616c 6c20 6467 656e 6572 6174 6520 7769  all dgenerate wi
 00014790: 7468 2070 6970 7820 6966 2079 6f75 2061  th pipx if you a
@@ -5418,26 +5418,26 @@
 00015290: 6f67 6c65 6170 6973 2e63 6f6d 2f6a 6178  ogleapis.com/jax
 000152a0: 2d72 656c 6561 7365 732f 6a61 785f 6375  -releases/jax_cu
 000152b0: 6461 5f72 656c 6561 7365 732e 6874 6d6c  da_releases.html
 000152c0: 220d 0a0d 0a20 2020 2023 2049 6620 796f  "....    # If yo
 000152d0: 7520 7761 6e74 2061 2073 7065 6369 6669  u want a specifi
 000152e0: 6320 7665 7273 696f 6e0d 0a0d 0a20 2020  c version....   
 000152f0: 2070 6970 7820 696e 7374 616c 6c20 6467   pipx install dg
-00015300: 656e 6572 6174 653d 3d33 2e35 2e30 205c  enerate==3.5.0 \
+00015300: 656e 6572 6174 653d 3d33 2e35 2e31 205c  enerate==3.5.1 \
 00015310: 0d0a 2020 2020 2d2d 7069 702d 6172 6773  ..    --pip-args
 00015320: 2022 2d2d 6578 7472 612d 696e 6465 782d   "--extra-index-
 00015330: 7572 6c20 6874 7470 733a 2f2f 646f 776e  url https://down
 00015340: 6c6f 6164 2e70 7974 6f72 6368 2e6f 7267  load.pytorch.org
 00015350: 2f77 686c 2f63 7531 3231 2f22 0d0a 0d0a  /whl/cu121/"....
 00015360: 2020 2020 2320 5370 6563 6966 6963 2076      # Specific v
 00015370: 6572 7369 6f6e 2077 6974 6820 666c 6178  ersion with flax
 00015380: 2f6a 6178 2073 7570 706f 7274 0d0a 0d0a  /jax support....
 00015390: 2020 2020 7069 7078 2069 6e73 7461 6c6c      pipx install
 000153a0: 2064 6765 6e65 7261 7465 5b66 6c61 785d   dgenerate[flax]
-000153b0: 3d3d 332e 352e 3020 5c0d 0a20 2020 202d  ==3.5.0 \..    -
+000153b0: 3d3d 332e 352e 3120 5c0d 0a20 2020 202d  ==3.5.1 \..    -
 000153c0: 2d70 6970 2d61 7267 7320 222d 2d65 7874  -pip-args "--ext
 000153d0: 7261 2d69 6e64 6578 2d75 726c 2068 7474  ra-index-url htt
 000153e0: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
 000153f0: 746f 7263 682e 6f72 672f 7768 6c2f 6375  torch.org/whl/cu
 00015400: 3132 312f 205c 0d0a 2020 2020 2d66 2068  121/ \..    -f h
 00015410: 7474 7073 3a2f 2f73 746f 7261 6765 2e67  ttps://storage.g
 00015420: 6f6f 676c 6561 7069 732e 636f 6d2f 6a61  oogleapis.com/ja
@@ -5445,23 +5445,23 @@
 00015440: 7564 615f 7265 6c65 6173 6573 2e68 746d  uda_releases.htm
 00015450: 6c22 0d0a 0d0a 2020 2020 2320 596f 7520  l"....    # You 
 00015460: 6361 6e20 696e 7374 616c 6c20 7769 7468  can install with
 00015470: 6f75 7420 7069 7078 2069 6e74 6f20 796f  out pipx into yo
 00015480: 7572 206f 776e 2065 6e76 6972 6f6e 6d65  ur own environme
 00015490: 6e74 206c 696b 6520 736f 0d0a 0d0a 2020  nt like so....  
 000154a0: 2020 7069 7033 2069 6e73 7461 6c6c 2064    pip3 install d
-000154b0: 6765 6e65 7261 7465 3d3d 332e 352e 3020  generate==3.5.0 
+000154b0: 6765 6e65 7261 7465 3d3d 332e 352e 3120  generate==3.5.1 
 000154c0: 2d2d 6578 7472 612d 696e 6465 782d 7572  --extra-index-ur
 000154d0: 6c20 6874 7470 733a 2f2f 646f 776e 6c6f  l https://downlo
 000154e0: 6164 2e70 7974 6f72 6368 2e6f 7267 2f77  ad.pytorch.org/w
 000154f0: 686c 2f63 7531 3231 2f0d 0a0d 0a20 2020  hl/cu121/....   
 00015500: 2023 204f 7220 7769 7468 2066 6c61 780d   # Or with flax.
 00015510: 0a0d 0a20 2020 2070 6970 3320 696e 7374  ...    pip3 inst
 00015520: 616c 6c20 6467 656e 6572 6174 655b 666c  all dgenerate[fl
-00015530: 6178 5d3d 3d33 2e35 2e30 202d 2d65 7874  ax]==3.5.0 --ext
+00015530: 6178 5d3d 3d33 2e35 2e31 202d 2d65 7874  ax]==3.5.1 --ext
 00015540: 7261 2d69 6e64 6578 2d75 726c 2068 7474  ra-index-url htt
 00015550: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
 00015560: 746f 7263 682e 6f72 672f 7768 6c2f 6375  torch.org/whl/cu
 00015570: 3132 312f 205c 0d0a 2020 2020 2d66 2068  121/ \..    -f h
 00015580: 7474 7073 3a2f 2f73 746f 7261 6765 2e67  ttps://storage.g
 00015590: 6f6f 676c 6561 7069 732e 636f 6d2f 6a61  oogleapis.com/ja
 000155a0: 782d 7265 6c65 6173 6573 2f6a 6178 5f63  x-releases/jax_c
@@ -6007,22 +6007,22 @@
 00017760: 7479 2e0d 0a0d 0a59 6f75 2063 616e 2064  ty.....You can d
 00017770: 6f77 6e6c 6f61 6420 7468 656d 2068 6572  ownload them her
 00017780: 653a 0d0a 0d0a 202a 2060 6d79 2d69 6d61  e:.... * `my-ima
 00017790: 6765 2d73 6565 642e 706e 6720 3c68 7474  ge-seed.png <htt
 000177a0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
 000177b0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f54  sercontent.com/T
 000177c0: 6572 696b 732f 6467 656e 6572 6174 652f  eriks/dgenerate/
-000177d0: 7633 2e35 2e30 2f65 7861 6d70 6c65 732f  v3.5.0/examples/
+000177d0: 7633 2e35 2e31 2f65 7861 6d70 6c65 732f  v3.5.1/examples/
 000177e0: 6d65 6469 612f 646f 672d 6f6e 2d62 656e  media/dog-on-ben
 000177f0: 6368 2e70 6e67 3e60 5f0d 0a20 2a20 606d  ch.png>`_.. * `m
 00017800: 792d 6d61 736b 2d69 6d61 6765 2e70 6e67  y-mask-image.png
 00017810: 203c 6874 7470 733a 2f2f 7261 772e 6769   <https://raw.gi
 00017820: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
 00017830: 636f 6d2f 5465 7269 6b73 2f64 6765 6e65  com/Teriks/dgene
-00017840: 7261 7465 2f76 332e 352e 302f 6578 616d  rate/v3.5.0/exam
+00017840: 7261 7465 2f76 332e 352e 312f 6578 616d  rate/v3.5.1/exam
 00017850: 706c 6573 2f6d 6564 6961 2f64 6f67 2d6f  ples/media/dog-o
 00017860: 6e2d 6265 6e63 682d 6d61 736b 2e70 6e67  n-bench-mask.png
 00017870: 3e60 5f0d 0a0d 0a54 6865 2063 6f6d 6d61  >`_....The comma
 00017880: 6e64 2062 656c 6f77 2067 656e 6572 6174  nd below generat
 00017890: 6573 2061 2063 6174 2073 6974 7469 6e67  es a cat sitting
 000178a0: 206f 6e20 6120 6265 6e63 6820 7769 7468   on a bench with
 000178b0: 2074 6865 2069 6d61 6765 7320 6672 6f6d   the images from
@@ -8723,15 +8723,15 @@
 00022120: 2069 6e66 6572 656e 6365 2073 7465 702e   inference step.
 00022130: 0d0a 0d0a 0d0a 5468 6573 6520 6578 616d  ......These exam
 00022140: 706c 6573 2075 7365 3a20 6076 6572 6d65  ples use: `verme
 00022150: 6572 5f63 616e 6e79 5f65 6467 6564 2e70  er_canny_edged.p
 00022160: 6e67 203c 6874 7470 733a 2f2f 7261 772e  ng <https://raw.
 00022170: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
 00022180: 742e 636f 6d2f 5465 7269 6b73 2f64 6765  t.com/Teriks/dge
-00022190: 6e65 7261 7465 2f76 332e 352e 302f 6578  nerate/v3.5.0/ex
+00022190: 6e65 7261 7465 2f76 332e 352e 312f 6578  nerate/v3.5.1/ex
 000221a0: 616d 706c 6573 2f6d 6564 6961 2f76 6572  amples/media/ver
 000221b0: 6d65 6572 5f63 616e 6e79 5f65 6467 6564  meer_canny_edged
 000221c0: 2e70 6e67 3e60 5f0d 0a0d 0a0d 0a2e 2e20  .png>`_........ 
 000221d0: 636f 6465 2d62 6c6f 636b 3a3a 2062 6173  code-block:: bas
 000221e0: 680d 0a0d 0a20 2020 2023 2054 6f72 6368  h....    # Torch
 000221f0: 2065 7861 6d70 6c65 2c20 7573 6520 2276   example, use "v
 00022200: 6572 6d65 6572 5f63 616e 6e79 5f65 6467  ermeer_canny_edg
@@ -9310,15 +9310,15 @@
 000245d0: 6f72 2067 656e 6572 6174 696f 6e20 7769  or generation wi
 000245e0: 7468 2061 206d 6f64 656c 202b 2061 2043  th a model + a C
 000245f0: 6f6e 7472 6f6c 4e65 742e 0d0a 0d0a 5468  ontrolNet.....Th
 00024600: 6973 2069 6d61 6765 206f 6620 6120 6068  is image of a `h
 00024610: 6f72 7365 203c 6874 7470 733a 2f2f 7261  orse <https://ra
 00024620: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
 00024630: 656e 742e 636f 6d2f 5465 7269 6b73 2f64  ent.com/Teriks/d
-00024640: 6765 6e65 7261 7465 2f76 332e 352e 302f  generate/v3.5.0/
+00024640: 6765 6e65 7261 7465 2f76 332e 352e 312f  generate/v3.5.1/
 00024650: 6578 616d 706c 6573 2f6d 6564 6961 2f68  examples/media/h
 00024660: 6f72 7365 322e 6a70 6567 3e60 5f0d 0a69  orse2.jpeg>`_..i
 00024670: 7320 7573 6564 2069 6e20 7468 6520 6578  s used in the ex
 00024680: 616d 706c 6520 6265 6c6f 7720 7769 7468  ample below with
 00024690: 2061 2043 6f6e 7472 6f6c 4e65 7420 7468   a ControlNet th
 000246a0: 6174 2069 7320 7472 6169 6e65 6420 746f  at is trained to
 000246b0: 2067 656e 6572 6174 6520 696d 6167 6573   generate images
@@ -9550,15 +9550,15 @@
 000254d0: 6520 696d 6167 6520 7573 6564 2069 6e20  e image used in 
 000254e0: 7468 6520 6578 616d 706c 6520 6265 6c6f  the example belo
 000254f0: 7720 6973 2074 6869 7320 606c 6f77 2072  w is this `low r
 00025500: 6573 6f6c 7574 696f 6e20 6361 7420 3c68  esolution cat <h
 00025510: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
 00025520: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
 00025530: 2f54 6572 696b 732f 6467 656e 6572 6174  /Teriks/dgenerat
-00025540: 652f 7633 2e35 2e30 2f65 7861 6d70 6c65  e/v3.5.0/example
+00025540: 652f 7633 2e35 2e31 2f65 7861 6d70 6c65  e/v3.5.1/example
 00025550: 732f 6d65 6469 612f 6c6f 775f 7265 735f  s/media/low_res_
 00025560: 6361 742e 706e 673e 605f 0d0a 0d0a 2e2e  cat.png>`_......
 00025570: 2063 6f64 652d 626c 6f63 6b3a 3a20 6261   code-block:: ba
 00025580: 7368 0d0a 0d0a 2020 2020 2320 5468 6520  sh....    # The 
 00025590: 696d 6167 6520 7072 6f64 7563 6564 2077  image produced w
 000255a0: 6974 6820 7468 6973 206d 6f64 656c 2077  ith this model w
 000255b0: 696c 6c20 6265 0d0a 2020 2020 2320 7477  ill be..    # tw
@@ -10601,15 +10601,15 @@
 00029680: 6f77 696e 6720 6973 2061 2063 6f6e 6669  owing is a confi
 00029690: 6720 6669 6c65 2065 7861 6d70 6c65 2074  g file example t
 000296a0: 6861 7420 636f 7665 7273 2076 6572 7920  hat covers very 
 000296b0: 6261 7369 6320 7379 6e74 6178 2063 6f6e  basic syntax con
 000296c0: 6365 7074 733a 0d0a 0d0a 2e2e 2063 6f64  cepts:...... cod
 000296d0: 652d 626c 6f63 6b3a 3a20 6a69 6e6a 610d  e-block:: jinja.
 000296e0: 0a0d 0a20 2020 2023 2120 6467 656e 6572  ...    #! dgener
-000296f0: 6174 6520 332e 352e 300d 0a0d 0a20 2020  ate 3.5.0....   
+000296f0: 6174 6520 332e 352e 310d 0a0d 0a20 2020  ate 3.5.1....   
 00029700: 2023 2049 6620 6120 6861 7368 2d62 616e   # If a hash-ban
 00029710: 6720 7665 7273 696f 6e20 6973 2070 726f  g version is pro
 00029720: 7669 6465 6420 696e 2074 6865 2066 6f72  vided in the for
 00029730: 6d61 7420 6162 6f76 650d 0a20 2020 2023  mat above..    #
 00029740: 2061 2077 6172 6e69 6e67 2077 696c 6c20   a warning will 
 00029750: 6265 2070 726f 6475 6365 6420 6966 2074  be produced if t
 00029760: 6865 2076 6572 7369 6f6e 2079 6f75 2061  he version you a
@@ -10869,15 +10869,15 @@
 0002a740: 2060 605c 7365 7460 6020 616e 6420 6060   ``\set`` and ``
 0002a750: 5c73 6574 7060 6020 6469 7265 6374 6976  \setp`` directiv
 0002a760: 6520 7769 6c6c 2061 6c73 6f20 6265 206d  e will also be m
 0002a770: 656e 7469 6f6e 6564 2069 6e20 7468 6973  entioned in this
 0002a780: 206f 7574 7075 742e 0d0a 0d0a 2e2e 2063   output....... c
 0002a790: 6f64 652d 626c 6f63 6b3a 3a20 6a69 6e6a  ode-block:: jinj
 0002a7a0: 610d 0a0d 0a20 2020 2023 2120 6467 656e  a....    #! dgen
-0002a7b0: 6572 6174 6520 332e 352e 300d 0a0d 0a20  erate 3.5.0.... 
+0002a7b0: 6572 6174 6520 332e 352e 310d 0a0d 0a20  erate 3.5.1.... 
 0002a7c0: 2020 2023 2049 6e76 6f63 6174 696f 6e20     # Invocation 
 0002a7d0: 7769 6c6c 2070 726f 6365 6564 2061 7320  will proceed as 
 0002a7e0: 6e6f 726d 616c 0d0a 0d0a 2020 2020 7374  normal....    st
 0002a7f0: 6162 696c 6974 7961 692f 7374 6162 6c65  abilityai/stable
 0002a800: 2d64 6966 6675 7369 6f6e 2d32 2d31 202d  -diffusion-2-1 -
 0002a810: 2d70 726f 6d70 7473 2022 6120 6d61 6e20  -prompts "a man 
 0002a820: 7761 6c6b 696e 6720 6f6e 2074 6865 206d  walking on the m
@@ -11780,15 +11780,15 @@
 0002e030: 6573 0d0a 7375 6368 2061 7320 5641 4573  es..such as VAEs
 0002e040: 2065 7463 2e20 6f75 7473 6964 6520 6f66   etc. outside of
 0002e050: 2072 656c 7969 6e67 206f 6e20 7468 6520   relying on the 
 0002e060: 6361 6368 696e 6720 7379 7374 656d 2e0d  caching system..
 0002e070: 0a0d 0a2e 2e20 636f 6465 2d62 6c6f 636b  ..... code-block
 0002e080: 3a3a 206a 696e 6a61 0d0a 0d0a 2020 2020  :: jinja....    
 0002e090: 2321 2064 6765 6e65 7261 7465 2033 2e35  #! dgenerate 3.5
-0002e0a0: 2e30 0d0a 0d0a 2020 2020 2320 596f 7520  .0....    # You 
+0002e0a0: 2e31 0d0a 0d0a 2020 2020 2320 596f 7520  .1....    # You 
 0002e0b0: 6361 6e20 6465 6669 6e65 2079 6f75 7220  can define your 
 0002e0c0: 6f77 6e20 7465 6d70 6c61 7465 2076 6172  own template var
 0002e0d0: 6961 626c 6573 2077 6974 6820 7468 6520  iables with the 
 0002e0e0: 5c73 6574 2064 6972 6563 7469 7665 0d0a  \set directive..
 0002e0f0: 2020 2020 2320 7468 6520 5c73 6574 2064      # the \set d
 0002e100: 6972 6563 7469 7665 2064 6f65 7320 6e6f  irective does no
 0002e110: 7420 646f 2061 6e79 2073 6865 6c6c 2061  t do any shell a
@@ -12267,15 +12267,15 @@
 0002fea0: 2067 6c6f 6220 6d6f 6475 6c65 2c20 796f   glob module, yo
 0002feb0: 7520 6361 6e20 616c 736f 2067 6c6f 6220  u can also glob 
 0002fec0: 6469 7265 6374 6f72 7927 7320 7573 696e  directory's usin
 0002fed0: 6720 7368 656c 6c0d 0a67 6c6f 6262 696e  g shell..globbin
 0002fee0: 672e 0d0a 0d0a 2e2e 2063 6f64 652d 626c  g....... code-bl
 0002fef0: 6f63 6b3a 3a20 6a69 6e6a 610d 0a0d 0a20  ock:: jinja.... 
 0002ff00: 2020 2023 2120 6467 656e 6572 6174 6520     #! dgenerate 
-0002ff10: 332e 352e 300d 0a0d 0a20 2020 2023 2067  3.5.0....    # g
+0002ff10: 332e 352e 310d 0a0d 0a20 2020 2023 2067  3.5.1....    # g
 0002ff20: 6c6f 6262 696e 6720 6361 6e20 6265 2070  lobbing can be p
 0002ff30: 7265 666f 726d 6564 2076 6961 2073 6865  reformed via she
 0002ff40: 6c6c 2065 7870 616e 7369 6f6e 206f 7220  ll expansion or 
 0002ff50: 7573 696e 670d 0a20 2020 2023 2074 6865  using..    # the
 0002ff60: 2067 6c6f 6220 6d6f 6475 6c65 2069 6e73   glob module ins
 0002ff70: 6964 6520 6a69 6e6a 6120 7465 6d70 6c61  ide jinja templa
 0002ff80: 7465 730d 0a0d 0a20 2020 2023 206e 6f74  tes....    # not
@@ -12366,15 +12366,15 @@
 000304d0: 622d 636f 6d6d 616e 6420 6060 696d 6167  b-command ``imag
 000304e0: 652d 7072 6f63 6573 7360 6020 6861 7320  e-process`` has 
 000304f0: 6120 636f 6e66 6967 2064 6972 6563 7469  a config directi
 00030500: 7665 2069 6d70 6c65 6d65 6e74 6174 696f  ve implementatio
 00030510: 6e2e 0d0a 0d0a 0d0a 2e2e 2063 6f64 652d  n......... code-
 00030520: 626c 6f63 6b3a 3a20 6a69 6e6a 610d 0a0d  block:: jinja...
 00030530: 0a20 2020 2023 2120 6467 656e 6572 6174  .    #! dgenerat
-00030540: 6520 332e 352e 300d 0a0d 0a20 2020 2023  e 3.5.0....    #
+00030540: 6520 332e 352e 310d 0a0d 0a20 2020 2023  e 3.5.1....    #
 00030550: 2070 7269 6e74 2074 6865 2068 656c 7020   print the help 
 00030560: 6d65 7373 6167 6520 6f66 202d 2d73 7562  message of --sub
 00030570: 2d63 6f6d 6d61 6e64 2069 6d61 6765 2d70  -command image-p
 00030580: 726f 6365 7373 2c20 7468 6973 2064 6f65  rocess, this doe
 00030590: 730d 0a20 2020 2023 206e 6f74 2063 6175  s..    # not cau
 000305a0: 7365 2074 6865 2063 6f6e 6669 6720 746f  se the config to
 000305b0: 2065 7869 740d 0a0d 0a20 2020 205c 696d   exit....    \im
@@ -12442,15 +12442,15 @@
 00030990: 2069 6d61 6765 2070 726f 6365 7373 696e   image processin
 000309a0: 6720 7574 696c 6974 6965 7320 6173 2073  g utilities as s
 000309b0: 7562 7072 6f63 6573 7365 7320 6672 6f6d  ubprocesses from
 000309c0: 2077 6974 6869 6e20 610d 0a63 6f6e 6669   within a..confi
 000309d0: 6720 7363 7269 7074 2e0d 0a0d 0a0d 0a2e  g script........
 000309e0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 0d0a  . code-block::..
 000309f0: 0d0a 2020 2020 2321 2064 6765 6e65 7261  ..    #! dgenera
-00030a00: 7465 2033 2e35 2e30 0d0a 0d0a 2020 2020  te 3.5.0....    
+00030a00: 7465 2033 2e35 2e31 0d0a 0d0a 2020 2020  te 3.5.1....    
 00030a10: 2320 7275 6e20 6467 656e 6572 6174 6520  # run dgenerate 
 00030a20: 6173 2061 2073 7562 7072 6f63 6573 732c  as a subprocess,
 00030a30: 2072 6561 6420 6120 636f 6e66 6967 0d0a   read a config..
 00030a40: 2020 2020 2320 616e 6420 7365 6e64 2073      # and send s
 00030a50: 7464 6f75 7420 616e 6420 7374 6465 7272  tdout and stderr
 00030a60: 2074 6f20 6120 6669 6c65 0d0a 0d0a 2020   to a file....  
 00030a70: 2020 5c65 7865 6320 6467 656e 6572 6174    \exec dgenerat
@@ -12477,15 +12477,15 @@
 00030bc0: 0d0a 596f 7520 6361 6e20 6578 6974 2061  ..You can exit a
 00030bd0: 2063 6f6e 6669 6720 6561 726c 7920 6966   config early if
 00030be0: 206e 6565 6420 6265 2075 7369 6e67 2074   need be using t
 00030bf0: 6865 2060 605c 6578 6974 6060 2064 6972  he ``\exit`` dir
 00030c00: 6563 7469 7665 0d0a 0d0a 0d0a 2e2e 2063  ective........ c
 00030c10: 6f64 652d 626c 6f63 6b3a 3a20 6a69 6e6a  ode-block:: jinj
 00030c20: 610d 0a0d 0a20 2020 2023 2120 6467 656e  a....    #! dgen
-00030c30: 6572 6174 6520 332e 352e 300d 0a0d 0a20  erate 3.5.0.... 
+00030c30: 6572 6174 6520 332e 352e 310d 0a0d 0a20  erate 3.5.1.... 
 00030c40: 2020 2023 2065 7869 7420 7468 6520 7072     # exit the pr
 00030c50: 6f63 6573 7320 7769 7468 2072 6574 7572  ocess with retur
 00030c60: 6e20 636f 6465 2031 2c20 7768 6963 6820  n code 1, which 
 00030c70: 696e 6469 6361 7465 7320 616e 2065 7272  indicates an err
 00030c80: 6f72 0d0a 0d0a 2020 2020 5c70 7269 6e74  or....    \print
 00030c90: 2022 736f 6d65 2065 7272 6f72 206f 6363   "some error occ
 00030ca0: 7572 7265 6422 0d0a 2020 2020 5c65 7869  urred"..    \exi
@@ -12607,15 +12607,15 @@
 000313e0: 7465 645f 706c 7567 696e 5f6d 6f64 756c  ted_plugin_modul
 000313f0: 6573 2065 6c73 6520 2727 207d 7d0d 0a0d  es else '' }}...
 00031400: 0a43 6f6e 736f 6c65 2055 490d 0a3d 3d3d  .Console UI..===
 00031410: 3d3d 3d3d 3d3d 3d0d 0a0d 0a2e 2e20 696d  =======...... im
 00031420: 6167 653a 3a20 6874 7470 733a 2f2f 7261  age:: https://ra
 00031430: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
 00031440: 656e 742e 636f 6d2f 5465 7269 6b73 2f64  ent.com/Teriks/d
-00031450: 6765 6e65 7261 7465 2f76 332e 352e 302f  generate/v3.5.0/
+00031450: 6765 6e65 7261 7465 2f76 332e 352e 312f  generate/v3.5.1/
 00031460: 6578 616d 706c 6573 2f6d 6564 6961 2f75  examples/media/u
 00031470: 692e 6769 660d 0a20 2020 3a61 6c74 3a20  i.gif..   :alt: 
 00031480: 636f 6e73 6f6c 6520 7569 0d0a 0d0a 596f  console ui....Yo
 00031490: 7520 6361 6e20 6c61 756e 6368 2061 2063  u can launch a c
 000314a0: 726f 7373 2070 6c61 7466 6f72 6d20 546b  ross platform Tk
 000314b0: 696e 7465 7220 4755 4920 666f 7220 696e  inter GUI for in
 000314c0: 7465 7261 6374 696e 6720 7769 7468 2061  teracting with a
@@ -12831,41 +12831,41 @@
 000321e0: 7220 706c 7567 696e 7320 6361 6e20 6265  r plugins can be
 000321f0: 2066 6f75 6e64 0d0a 696e 2074 6865 2060   found..in the `
 00032200: 2277 7269 7469 6e67 5f70 6c75 6769 6e73  "writing_plugins
 00032210: 2f69 6d61 6765 5f70 726f 6365 7373 6f72  /image_processor
 00032220: 2220 3c68 7474 7073 3a2f 2f67 6974 6875  " <https://githu
 00032230: 622e 636f 6d2f 5465 7269 6b73 2f64 6765  b.com/Teriks/dge
 00032240: 6e65 7261 7465 2f74 7265 652f 7633 2e35  nerate/tree/v3.5
-00032250: 2e30 2f65 7861 6d70 6c65 732f 7772 6974  .0/examples/writ
+00032250: 2e31 2f65 7861 6d70 6c65 732f 7772 6974  .1/examples/writ
 00032260: 696e 675f 706c 7567 696e 732f 696d 6167  ing_plugins/imag
 00032270: 655f 7072 6f63 6573 736f 723e 605f 0d0a  e_processor>`_..
 00032280: 666f 6c64 6572 206f 6620 7468 6520 6578  folder of the ex
 00032290: 616d 706c 6573 2066 6f6c 6465 722e 0d0a  amples folder...
 000322a0: 0d0a 5468 6520 736f 7572 6365 2063 6f64  ..The source cod
 000322b0: 6520 666f 7220 7468 6520 6275 696c 7420  e for the built 
 000322c0: 696e 2060 6361 6e6e 7920 3c68 7474 7073  in `canny <https
 000322d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5465  ://github.com/Te
 000322e0: 7269 6b73 2f64 6765 6e65 7261 7465 2f62  riks/dgenerate/b
-000322f0: 6c6f 622f 7633 2e35 2e30 2f64 6765 6e65  lob/v3.5.0/dgene
+000322f0: 6c6f 622f 7633 2e35 2e31 2f64 6765 6e65  lob/v3.5.1/dgene
 00032300: 7261 7465 2f69 6d61 6765 7072 6f63 6573  rate/imageproces
 00032310: 736f 7273 2f63 616e 6e79 2e70 793e 605f  sors/canny.py>`_
 00032320: 2070 726f 6365 7373 6f72 2c0d 0a74 6865   processor,..the
 00032330: 2060 6f70 656e 706f 7365 203c 6874 7470   `openpose <http
 00032340: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
 00032350: 6572 696b 732f 6467 656e 6572 6174 652f  eriks/dgenerate/
-00032360: 626c 6f62 2f76 332e 352e 302f 6467 656e  blob/v3.5.0/dgen
+00032360: 626c 6f62 2f76 332e 352e 312f 6467 656e  blob/v3.5.1/dgen
 00032370: 6572 6174 652f 696d 6167 6570 726f 6365  erate/imageproce
 00032380: 7373 6f72 732f 6f70 656e 706f 7365 2e70  ssors/openpose.p
 00032390: 793e 605f 2070 726f 6365 7373 6f72 2c20  y>`_ processor, 
 000323a0: 616e 6420 7468 6520 7369 6d70 6c65 0d0a  and the simple..
 000323b0: 6070 696c 6c6f 7720 696d 6167 6520 6f70  `pillow image op
 000323c0: 6572 6174 696f 6e73 203c 6874 7470 733a  erations <https:
 000323d0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6572  //github.com/Ter
 000323e0: 696b 732f 6467 656e 6572 6174 652f 626c  iks/dgenerate/bl
-000323f0: 6f62 2f76 332e 352e 302f 6467 656e 6572  ob/v3.5.0/dgener
+000323f0: 6f62 2f76 332e 352e 312f 6467 656e 6572  ob/v3.5.1/dgener
 00032400: 6174 652f 696d 6167 6570 726f 6365 7373  ate/imageprocess
 00032410: 6f72 732f 696d 6167 656f 7073 2e70 793e  ors/imageops.py>
 00032420: 605f 2070 726f 6365 7373 6f72 7320 6361  `_ processors ca
 00032430: 6e20 616c 736f 0d0a 6265 206f 6620 7265  n also..be of re
 00032440: 6665 7265 6e63 6520 6173 2074 6865 7920  ference as they 
 00032450: 6172 6520 7772 6974 7465 6e20 6173 2069  are written as i
 00032460: 6e74 6572 6e61 6c20 696d 6167 6520 7072  nternal image pr
@@ -12875,29 +12875,29 @@
 000324a0: 6720 6469 7265 6374 6976 6573 2063 616e  g directives can
 000324b0: 2062 6520 666f 756e 6420 696e 2074 6865   be found in the
 000324c0: 0d0a 6022 7772 6974 696e 675f 706c 7567  ..`"writing_plug
 000324d0: 696e 732f 636f 6e66 6967 5f64 6972 6563  ins/config_direc
 000324e0: 7469 7665 2220 3c68 7474 7073 3a2f 2f67  tive" <https://g
 000324f0: 6974 6875 622e 636f 6d2f 5465 7269 6b73  ithub.com/Teriks
 00032500: 2f64 6765 6e65 7261 7465 2f74 7265 652f  /dgenerate/tree/
-00032510: 7633 2e35 2e30 2f65 7861 6d70 6c65 732f  v3.5.0/examples/
+00032510: 7633 2e35 2e31 2f65 7861 6d70 6c65 732f  v3.5.1/examples/
 00032520: 7772 6974 696e 675f 706c 7567 696e 732f  writing_plugins/
 00032530: 636f 6e66 6967 5f64 6972 6563 7469 7665  config_directive
 00032540: 3e60 5f20 666f 6c64 6572 0d0a 6f66 2074  >`_ folder..of t
 00032550: 6865 2065 7861 6d70 6c65 7320 666f 6c64  he examples fold
 00032560: 6572 2e20 436f 6e66 6967 2074 656d 706c  er. Config templ
 00032570: 6174 6520 6675 6e63 7469 6f6e 7320 6361  ate functions ca
 00032580: 6e20 616c 736f 2062 6520 696d 706c 656d  n also be implem
 00032590: 656e 7465 6420 6279 2070 6c75 6769 6e73  ented by plugins
 000325a0: 2c0d 0a73 6565 3a20 6022 7772 6974 696e  ,..see: `"writin
 000325b0: 675f 706c 7567 696e 732f 7465 6d70 6c61  g_plugins/templa
 000325c0: 7465 5f66 756e 6374 696f 6e22 203c 6874  te_function" <ht
 000325d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000325e0: 2f54 6572 696b 732f 6467 656e 6572 6174  /Teriks/dgenerat
-000325f0: 652f 7472 6565 2f76 332e 352e 302f 6578  e/tree/v3.5.0/ex
+000325f0: 652f 7472 6565 2f76 332e 352e 312f 6578  e/tree/v3.5.1/ex
 00032600: 616d 706c 6573 2f77 7269 7469 6e67 5f70  amples/writing_p
 00032610: 6c75 6769 6e73 2f74 656d 706c 6174 655f  lugins/template_
 00032620: 6675 6e63 7469 6f6e 3e60 5f0d 0a0d 0a43  function>`_....C
 00032630: 7572 7265 6e74 6c79 2074 6865 206f 6e6c  urrently the onl
 00032640: 7920 696e 7465 726e 616c 2064 6972 6563  y internal direc
 00032650: 7469 7665 2074 6861 7420 6973 2069 6d70  tive that is imp
 00032660: 6c65 6d65 6e74 6564 2061 7320 6120 706c  lemented as a pl
@@ -12905,15 +12905,15 @@
 00032680: 6d61 6765 5f70 726f 6365 7373 6060 2064  mage_process`` d
 00032690: 6972 6563 7469 7665 2c0d 0a77 686f 2773  irective,..who's
 000326a0: 2073 6f75 7263 6520 6669 6c65 2060 6361   source file `ca
 000326b0: 6e20 6265 206c 6f63 6174 6564 2068 6572  n be located her
 000326c0: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
 000326d0: 622e 636f 6d2f 5465 7269 6b73 2f64 6765  b.com/Teriks/dge
 000326e0: 6e65 7261 7465 2f62 6c6f 622f 7633 2e35  nerate/blob/v3.5
-000326f0: 2e30 2f64 6765 6e65 7261 7465 2f62 6174  .0/dgenerate/bat
+000326f0: 2e31 2f64 6765 6e65 7261 7465 2f62 6174  .1/dgenerate/bat
 00032700: 6368 7072 6f63 6573 732f 696d 6167 655f  chprocess/image_
 00032710: 7072 6f63 6573 735f 6469 7265 6374 6976  process_directiv
 00032720: 652e 7079 3e60 5f2c 0d0a 7468 6520 736f  e.py>`_,..the so
 00032730: 7572 6365 2066 696c 6520 666f 7220 7468  urce file for th
 00032740: 6973 2064 6972 6563 7469 7665 2069 7320  is directive is 
 00032750: 7465 7273 6520 6173 206d 6f73 7420 6f66  terse as most of
 00032760: 2060 605c 696d 6167 655f 7072 6f63 6573   ``\image_proces
@@ -12926,15 +12926,15 @@
 000327d0: 6963 6820 6973 2061 6c73 6f20 7573 6564  ich is also used
 000327e0: 2066 6f72 2060 602d 2d73 7562 2d63 6f6d   for ``--sub-com
 000327f0: 6d61 6e64 2069 6d61 6765 2d70 726f 6365  mand image-proce
 00032800: 7373 6060 2069 730d 0a60 6973 2069 6d70  ss`` is..`is imp
 00032810: 6c65 6d65 6e74 6564 2068 6572 6520 3c68  lemented here <h
 00032820: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00032830: 6d2f 5465 7269 6b73 2f64 6765 6e65 7261  m/Teriks/dgenera
-00032840: 7465 2f62 6c6f 622f 7633 2e35 2e30 2f64  te/blob/v3.5.0/d
+00032840: 7465 2f62 6c6f 622f 7633 2e35 2e31 2f64  te/blob/v3.5.1/d
 00032850: 6765 6e65 7261 7465 2f69 6d61 6765 5f70  generate/image_p
 00032860: 726f 6365 7373 3e60 5f2e 0d0a 0d0a 4669  rocess>`_.....Fi
 00032870: 6c65 2043 6163 6865 2043 6f6e 7472 6f6c  le Cache Control
 00032880: 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..==============
 00032890: 3d3d 3d3d 0d0a 0d0a 6467 656e 6572 6174  ====....dgenerat
 000328a0: 6520 7769 6c6c 2063 6163 6865 2060 602d  e will cache ``-
 000328b0: 2d69 6d61 6765 2d73 6565 6473 6060 2066  -image-seeds`` f
```

### Comparing `dgenerate-3.5.0/README.rst` & `dgenerate-3.5.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 00000000: 2e2e 207c 446f 6375 6d65 6e74 6174 696f  .. |Documentatio
 00000010: 6e20 5374 6174 7573 7c20 696d 6167 653a  n Status| image:
 00000020: 3a20 6874 7470 733a 2f2f 7265 6164 7468  : https://readth
 00000030: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
 00000040: 7473 2f64 6765 6e65 7261 7465 2f62 6164  ts/dgenerate/bad
 00000050: 6765 2f3f 7665 7273 696f 6e3d 7633 2e35  ge/?version=v3.5
-00000060: 2e30 0d0a 2020 203a 7461 7267 6574 3a20  .0..   :target: 
+00000060: 2e31 0d0a 2020 203a 7461 7267 6574 3a20  .1..   :target: 
 00000070: 6874 7470 3a2f 2f64 6765 6e65 7261 7465  http://dgenerate
 00000080: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000090: 656e 2f76 332e 352e 302f 0d0a 0d0a 4f76  en/v3.5.0/....Ov
+00000090: 656e 2f76 332e 352e 312f 0d0a 0d0a 4f76  en/v3.5.1/....Ov
 000000a0: 6572 7669 6577 0d0a 3d3d 3d3d 3d3d 3d3d  erview..========
 000000b0: 0d0a 0d0a 7c44 6f63 756d 656e 7461 7469  ....|Documentati
 000000c0: 6f6e 2053 7461 7475 737c 0d0a 0d0a 2a2a  on Status|....**
 000000d0: 6467 656e 6572 6174 652a 2a20 6973 2061  dgenerate** is a
 000000e0: 2063 6f6d 6d61 6e64 206c 696e 6520 746f   command line to
 000000f0: 6f6c 2061 6e64 206c 6962 7261 7279 2066  ol and library f
 00000100: 6f72 2067 656e 6572 6174 696e 6720 696d  or generating im
@@ -136,15 +136,15 @@
 00000870: 696f 6e73 2062 7574 2065 7874 7261 6f72  ions but extraor
 00000880: 6469 6e61 7269 6c79 2073 6c6f 772e 0d0a  dinarily slow...
 00000890: 0d0a 466f 7220 6c69 6272 6172 7920 646f  ..For library do
 000008a0: 6375 6d65 6e74 6174 696f 6e20 7669 7369  cumentation visi
 000008b0: 7420 6072 6561 6474 6865 646f 6373 203c  t `readthedocs <
 000008c0: 6874 7470 3a2f 2f64 6765 6e65 7261 7465  http://dgenerate
 000008d0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000008e0: 656e 2f76 332e 352e 302f 3e60 5f2e 0d0a  en/v3.5.0/>`_...
+000008e0: 656e 2f76 332e 352e 312f 3e60 5f2e 0d0a  en/v3.5.1/>`_...
 000008f0: 0d0a 2d2d 2d2d 0d0a 0d0a 2a20 486f 7720  ..----....* How 
 00000900: 746f 2069 6e73 7461 6c6c 0d0a 2020 2020  to install..    
 00000910: 2a20 6057 696e 646f 7773 2049 6e73 7461  * `Windows Insta
 00000920: 6c6c 605f 0d0a 2020 2020 2a20 604c 696e  ll`_..    * `Lin
 00000930: 7578 206f 7220 5753 4c20 496e 7374 616c  ux or WSL Instal
 00000940: 6c60 5f0d 0a0d 0a2a 2055 7361 6765 2045  l`_....* Usage E
 00000950: 7861 6d70 6c65 730d 0a20 2020 202a 2060  xamples..    * `
@@ -4670,15 +4670,15 @@
 000123d0: 2020 2020 2020 2020 2022 7573 6564 5f70           "used_p
 000123e0: 6572 6365 6e74 203e 2037 3022 2046 6f72  ercent > 70" For
 000123f0: 2053 796e 7461 7820 5365 653a 205b 6874   Syntax See: [ht
 00012400: 7470 733a 2f2f 6467 656e 6572 6174 652e  tps://dgenerate.
 00012410: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
 00012420: 6e2f 760d 0a20 2020 2020 2020 2020 2020  n/v..           
 00012430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012440: 2033 2e35 2e30 2f64 6765 6e65 7261 7465   3.5.0/dgenerate
+00012440: 2033 2e35 2e31 2f64 6765 6e65 7261 7465   3.5.1/dgenerate
 00012450: 5f73 7562 6d6f 6475 6c65 732e 6874 6d6c  _submodules.html
 00012460: 2364 6765 6e65 7261 7465 2e70 6970 656c  #dgenerate.pipel
 00012470: 696e 6577 7261 7070 6572 2e43 4143 4845  inewrapper.CACHE
 00012480: 5f4d 454d 4f52 595f 434f 4e0d 0a20 2020  _MEMORY_CON..   
 00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000124a0: 2020 2020 2020 2020 2053 5452 4149 4e54           STRAINT
 000124b0: 535d 0d0a 2020 2020 2020 2d70 6d63 2045  S]..      -pmc E
@@ -4722,15 +4722,15 @@
 00012710: 2020 2270 6970 656c 696e 655f 7369 7a65    "pipeline_size
 00012720: 203e 2028 6176 6169 6c61 626c 6520 2a20   > (available * 
 00012730: 302e 3735 2922 2046 6f72 2053 796e 7461  0.75)" For Synta
 00012740: 7820 5365 653a 205b 6874 7470 733a 2f2f  x See: [https://
 00012750: 6467 656e 6572 6174 652e 7265 0d0a 2020  dgenerate.re..  
 00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012770: 2020 2020 2020 2020 2020 6164 7468 6564            adthed
-00012780: 6f63 732e 696f 2f65 6e2f 7633 2e35 2e30  ocs.io/en/v3.5.0
+00012780: 6f63 732e 696f 2f65 6e2f 7633 2e35 2e31  ocs.io/en/v3.5.1
 00012790: 2f64 6765 6e65 7261 7465 5f73 7562 6d6f  /dgenerate_submo
 000127a0: 6475 6c65 732e 6874 6d6c 2364 6765 6e65  dules.html#dgene
 000127b0: 7261 7465 2e70 6970 656c 696e 6577 7261  rate.pipelinewra
 000127c0: 7070 6572 0d0a 2020 2020 2020 2020 2020  pper..          
 000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000127e0: 2020 2e50 4950 454c 494e 455f 4341 4348    .PIPELINE_CACH
 000127f0: 455f 4d45 4d4f 5259 5f43 4f4e 5354 5241  E_MEMORY_CONSTRA
@@ -4772,15 +4772,15 @@
 00012a30: 6e65 745f 7369 7a65 203e 2028 6176 6169  net_size > (avai
 00012a40: 6c61 626c 6520 2a20 302e 3735 2922 2046  lable * 0.75)" F
 00012a50: 6f72 0d0a 2020 2020 2020 2020 2020 2020  or..            
 00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012a70: 5379 6e74 6178 2053 6565 3a20 5b68 7474  Syntax See: [htt
 00012a80: 7073 3a2f 2f64 6765 6e65 7261 7465 2e72  ps://dgenerate.r
 00012a90: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00012aa0: 2f76 332e 352e 302f 6467 656e 6572 6174  /v3.5.0/dgenerat
+00012aa0: 2f76 332e 352e 312f 6467 656e 6572 6174  /v3.5.1/dgenerat
 00012ab0: 655f 7375 626d 6f64 756c 0d0a 2020 2020  e_submodul..    
 00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012ad0: 2020 2020 2020 2020 6573 2e68 746d 6c23          es.html#
 00012ae0: 6467 656e 6572 6174 652e 7069 7065 6c69  dgenerate.pipeli
 00012af0: 6e65 7772 6170 7065 722e 554e 4554 5f43  newrapper.UNET_C
 00012b00: 4143 4845 5f4d 454d 4f52 595f 434f 4e53  ACHE_MEMORY_CONS
 00012b10: 5452 4149 4e54 535d 0d0a 2020 2020 2020  TRAINTS]..      
@@ -4821,15 +4821,15 @@
 00012d40: 655f 7369 7a65 203e 2028 6176 6169 6c61  e_size > (availa
 00012d50: 626c 6520 2a20 302e 3735 2922 2046 6f72  ble * 0.75)" For
 00012d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012d70: 2020 2020 2020 2020 2020 2020 2020 5379                Sy
 00012d80: 6e74 6178 2053 6565 3a20 5b68 7474 7073  ntax See: [https
 00012d90: 3a2f 2f64 6765 6e65 7261 7465 2e72 6561  ://dgenerate.rea
 00012da0: 6474 6865 646f 6373 2e69 6f2f 656e 2f76  dthedocs.io/en/v
-00012db0: 332e 352e 302f 6467 656e 6572 6174 655f  3.5.0/dgenerate_
+00012db0: 332e 352e 312f 6467 656e 6572 6174 655f  3.5.1/dgenerate_
 00012dc0: 7375 626d 6f64 756c 0d0a 2020 2020 2020  submodul..      
 00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012de0: 2020 2020 2020 6573 2e68 746d 6c23 6467        es.html#dg
 00012df0: 656e 6572 6174 652e 7069 7065 6c69 6e65  enerate.pipeline
 00012e00: 7772 6170 7065 722e 5641 455f 4341 4348  wrapper.VAE_CACH
 00012e10: 455f 4d45 4d4f 5259 5f43 4f4e 5354 5241  E_MEMORY_CONSTRA
 00012e20: 494e 5453 5d0d 0a20 2020 2020 202d 636d  INTS]..      -cm
@@ -4874,15 +4874,15 @@
 00013090: 2020 2020 2020 2020 2861 7661 696c 6162          (availab
 000130a0: 6c65 202a 2030 2e37 3529 2220 466f 7220  le * 0.75)" For 
 000130b0: 5379 6e74 6178 2053 6565 3a20 5b68 7474  Syntax See: [htt
 000130c0: 7073 3a2f 2f64 6765 6e65 7261 7465 2e72  ps://dgenerate.r
 000130d0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
 000130e0: 2f76 0d0a 2020 2020 2020 2020 2020 2020  /v..            
 000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013100: 332e 352e 302f 6467 656e 6572 6174 655f  3.5.0/dgenerate_
+00013100: 332e 352e 312f 6467 656e 6572 6174 655f  3.5.1/dgenerate_
 00013110: 7375 626d 6f64 756c 6573 2e68 746d 6c23  submodules.html#
 00013120: 6467 656e 6572 6174 652e 7069 7065 6c69  dgenerate.pipeli
 00013130: 6e65 7772 6170 7065 722e 434f 4e54 524f  newrapper.CONTRO
 00013140: 4c5f 4e45 545f 4341 4348 0d0a 2020 2020  L_NET_CACH..    
 00013150: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013160: 2020 2020 2020 2020 455f 4d45 4d4f 5259          E_MEMORY
 00013170: 5f43 4f4e 5354 5241 494e 5453 5d0d 0a0d  _CONSTRAINTS]...
@@ -4966,27 +4966,27 @@
 00013650: 6578 2d75 726c 2068 7474 7073 3a2f 2f64  ex-url https://d
 00013660: 6f77 6e6c 6f61 642e 7079 746f 7263 682e  ownload.pytorch.
 00013670: 6f72 672f 7768 6c2f 6375 3132 312f 220d  org/whl/cu121/".
 00013680: 0a0d 0a20 2020 2023 2049 6620 796f 7520  ...    # If you 
 00013690: 7761 6e74 2061 2073 7065 6369 6669 6320  want a specific 
 000136a0: 7665 7273 696f 6e0d 0a0d 0a20 2020 2070  version....    p
 000136b0: 6970 7820 696e 7374 616c 6c20 6467 656e  ipx install dgen
-000136c0: 6572 6174 653d 3d33 2e35 2e30 205e 0d0a  erate==3.5.0 ^..
+000136c0: 6572 6174 653d 3d33 2e35 2e31 205e 0d0a  erate==3.5.1 ^..
 000136d0: 2020 2020 2d2d 7069 702d 6172 6773 2022      --pip-args "
 000136e0: 2d2d 6578 7472 612d 696e 6465 782d 7572  --extra-index-ur
 000136f0: 6c20 6874 7470 733a 2f2f 646f 776e 6c6f  l https://downlo
 00013700: 6164 2e70 7974 6f72 6368 2e6f 7267 2f77  ad.pytorch.org/w
 00013710: 686c 2f63 7531 3231 2f22 0d0a 0d0a 2020  hl/cu121/"....  
 00013720: 2020 2320 596f 7520 6361 6e20 696e 7374    # You can inst
 00013730: 616c 6c20 7769 7468 6f75 7420 7069 7078  all without pipx
 00013740: 2069 6e74 6f20 796f 7572 206f 776e 2065   into your own e
 00013750: 6e76 6972 6f6e 6d65 6e74 206c 696b 6520  nvironment like 
 00013760: 736f 0d0a 0d0a 2020 2020 7069 7020 696e  so....    pip in
 00013770: 7374 616c 6c20 6467 656e 6572 6174 653d  stall dgenerate=
-00013780: 3d33 2e35 2e30 202d 2d65 7874 7261 2d69  =3.5.0 --extra-i
+00013780: 3d33 2e35 2e31 202d 2d65 7874 7261 2d69  =3.5.1 --extra-i
 00013790: 6e64 6578 2d75 726c 2068 7474 7073 3a2f  ndex-url https:/
 000137a0: 2f64 6f77 6e6c 6f61 642e 7079 746f 7263  /download.pytorc
 000137b0: 682e 6f72 672f 7768 6c2f 6375 3132 312f  h.org/whl/cu121/
 000137c0: 0d0a 0d0a 0d0a 4974 2069 7320 7265 636f  ......It is reco
 000137d0: 6d6d 656e 6465 6420 746f 2069 6e73 7461  mmended to insta
 000137e0: 6c6c 2064 6765 6e65 7261 7465 2077 6974  ll dgenerate wit
 000137f0: 6820 7069 7078 2069 6620 796f 7520 6172  h pipx if you ar
@@ -5168,26 +5168,26 @@
 000142f0: 676c 6561 7069 732e 636f 6d2f 6a61 782d  gleapis.com/jax-
 00014300: 7265 6c65 6173 6573 2f6a 6178 5f63 7564  releases/jax_cud
 00014310: 615f 7265 6c65 6173 6573 2e68 746d 6c22  a_releases.html"
 00014320: 0d0a 0d0a 2020 2020 2320 4966 2079 6f75  ....    # If you
 00014330: 2077 616e 7420 6120 7370 6563 6966 6963   want a specific
 00014340: 2076 6572 7369 6f6e 0d0a 0d0a 2020 2020   version....    
 00014350: 7069 7078 2069 6e73 7461 6c6c 2064 6765  pipx install dge
-00014360: 6e65 7261 7465 3d3d 332e 352e 3020 5c0d  nerate==3.5.0 \.
+00014360: 6e65 7261 7465 3d3d 332e 352e 3120 5c0d  nerate==3.5.1 \.
 00014370: 0a20 2020 202d 2d70 6970 2d61 7267 7320  .    --pip-args 
 00014380: 222d 2d65 7874 7261 2d69 6e64 6578 2d75  "--extra-index-u
 00014390: 726c 2068 7474 7073 3a2f 2f64 6f77 6e6c  rl https://downl
 000143a0: 6f61 642e 7079 746f 7263 682e 6f72 672f  oad.pytorch.org/
 000143b0: 7768 6c2f 6375 3132 312f 220d 0a0d 0a20  whl/cu121/".... 
 000143c0: 2020 2023 2053 7065 6369 6669 6320 7665     # Specific ve
 000143d0: 7273 696f 6e20 7769 7468 2066 6c61 782f  rsion with flax/
 000143e0: 6a61 7820 7375 7070 6f72 740d 0a0d 0a20  jax support.... 
 000143f0: 2020 2070 6970 7820 696e 7374 616c 6c20     pipx install 
 00014400: 6467 656e 6572 6174 655b 666c 6178 5d3d  dgenerate[flax]=
-00014410: 3d33 2e35 2e30 205c 0d0a 2020 2020 2d2d  =3.5.0 \..    --
+00014410: 3d33 2e35 2e31 205c 0d0a 2020 2020 2d2d  =3.5.1 \..    --
 00014420: 7069 702d 6172 6773 2022 2d2d 6578 7472  pip-args "--extr
 00014430: 612d 696e 6465 782d 7572 6c20 6874 7470  a-index-url http
 00014440: 733a 2f2f 646f 776e 6c6f 6164 2e70 7974  s://download.pyt
 00014450: 6f72 6368 2e6f 7267 2f77 686c 2f63 7531  orch.org/whl/cu1
 00014460: 3231 2f20 5c0d 0a20 2020 202d 6620 6874  21/ \..    -f ht
 00014470: 7470 733a 2f2f 7374 6f72 6167 652e 676f  tps://storage.go
 00014480: 6f67 6c65 6170 6973 2e63 6f6d 2f6a 6178  ogleapis.com/jax
@@ -5195,23 +5195,23 @@
 000144a0: 6461 5f72 656c 6561 7365 732e 6874 6d6c  da_releases.html
 000144b0: 220d 0a0d 0a20 2020 2023 2059 6f75 2063  "....    # You c
 000144c0: 616e 2069 6e73 7461 6c6c 2077 6974 686f  an install witho
 000144d0: 7574 2070 6970 7820 696e 746f 2079 6f75  ut pipx into you
 000144e0: 7220 6f77 6e20 656e 7669 726f 6e6d 656e  r own environmen
 000144f0: 7420 6c69 6b65 2073 6f0d 0a0d 0a20 2020  t like so....   
 00014500: 2070 6970 3320 696e 7374 616c 6c20 6467   pip3 install dg
-00014510: 656e 6572 6174 653d 3d33 2e35 2e30 202d  enerate==3.5.0 -
+00014510: 656e 6572 6174 653d 3d33 2e35 2e31 202d  enerate==3.5.1 -
 00014520: 2d65 7874 7261 2d69 6e64 6578 2d75 726c  -extra-index-url
 00014530: 2068 7474 7073 3a2f 2f64 6f77 6e6c 6f61   https://downloa
 00014540: 642e 7079 746f 7263 682e 6f72 672f 7768  d.pytorch.org/wh
 00014550: 6c2f 6375 3132 312f 0d0a 0d0a 2020 2020  l/cu121/....    
 00014560: 2320 4f72 2077 6974 6820 666c 6178 0d0a  # Or with flax..
 00014570: 0d0a 2020 2020 7069 7033 2069 6e73 7461  ..    pip3 insta
 00014580: 6c6c 2064 6765 6e65 7261 7465 5b66 6c61  ll dgenerate[fla
-00014590: 785d 3d3d 332e 352e 3020 2d2d 6578 7472  x]==3.5.0 --extr
+00014590: 785d 3d3d 332e 352e 3120 2d2d 6578 7472  x]==3.5.1 --extr
 000145a0: 612d 696e 6465 782d 7572 6c20 6874 7470  a-index-url http
 000145b0: 733a 2f2f 646f 776e 6c6f 6164 2e70 7974  s://download.pyt
 000145c0: 6f72 6368 2e6f 7267 2f77 686c 2f63 7531  orch.org/whl/cu1
 000145d0: 3231 2f20 5c0d 0a20 2020 202d 6620 6874  21/ \..    -f ht
 000145e0: 7470 733a 2f2f 7374 6f72 6167 652e 676f  tps://storage.go
 000145f0: 6f67 6c65 6170 6973 2e63 6f6d 2f6a 6178  ogleapis.com/jax
 00014600: 2d72 656c 6561 7365 732f 6a61 785f 6375  -releases/jax_cu
@@ -5757,22 +5757,22 @@
 000167c0: 792e 0d0a 0d0a 596f 7520 6361 6e20 646f  y.....You can do
 000167d0: 776e 6c6f 6164 2074 6865 6d20 6865 7265  wnload them here
 000167e0: 3a0d 0a0d 0a20 2a20 606d 792d 696d 6167  :.... * `my-imag
 000167f0: 652d 7365 6564 2e70 6e67 203c 6874 7470  e-seed.png <http
 00016800: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
 00016810: 6572 636f 6e74 656e 742e 636f 6d2f 5465  ercontent.com/Te
 00016820: 7269 6b73 2f64 6765 6e65 7261 7465 2f76  riks/dgenerate/v
-00016830: 332e 352e 302f 6578 616d 706c 6573 2f6d  3.5.0/examples/m
+00016830: 332e 352e 312f 6578 616d 706c 6573 2f6d  3.5.1/examples/m
 00016840: 6564 6961 2f64 6f67 2d6f 6e2d 6265 6e63  edia/dog-on-benc
 00016850: 682e 706e 673e 605f 0d0a 202a 2060 6d79  h.png>`_.. * `my
 00016860: 2d6d 6173 6b2d 696d 6167 652e 706e 6720  -mask-image.png 
 00016870: 3c68 7474 7073 3a2f 2f72 6177 2e67 6974  <https://raw.git
 00016880: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
 00016890: 6f6d 2f54 6572 696b 732f 6467 656e 6572  om/Teriks/dgener
-000168a0: 6174 652f 7633 2e35 2e30 2f65 7861 6d70  ate/v3.5.0/examp
+000168a0: 6174 652f 7633 2e35 2e31 2f65 7861 6d70  ate/v3.5.1/examp
 000168b0: 6c65 732f 6d65 6469 612f 646f 672d 6f6e  les/media/dog-on
 000168c0: 2d62 656e 6368 2d6d 6173 6b2e 706e 673e  -bench-mask.png>
 000168d0: 605f 0d0a 0d0a 5468 6520 636f 6d6d 616e  `_....The comman
 000168e0: 6420 6265 6c6f 7720 6765 6e65 7261 7465  d below generate
 000168f0: 7320 6120 6361 7420 7369 7474 696e 6720  s a cat sitting 
 00016900: 6f6e 2061 2062 656e 6368 2077 6974 6820  on a bench with 
 00016910: 7468 6520 696d 6167 6573 2066 726f 6d20  the images from 
@@ -8473,15 +8473,15 @@
 00021180: 696e 6665 7265 6e63 6520 7374 6570 2e0d  inference step..
 00021190: 0a0d 0a0d 0a54 6865 7365 2065 7861 6d70  .....These examp
 000211a0: 6c65 7320 7573 653a 2060 7665 726d 6565  les use: `vermee
 000211b0: 725f 6361 6e6e 795f 6564 6765 642e 706e  r_canny_edged.pn
 000211c0: 6720 3c68 7474 7073 3a2f 2f72 6177 2e67  g <https://raw.g
 000211d0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
 000211e0: 2e63 6f6d 2f54 6572 696b 732f 6467 656e  .com/Teriks/dgen
-000211f0: 6572 6174 652f 7633 2e35 2e30 2f65 7861  erate/v3.5.0/exa
+000211f0: 6572 6174 652f 7633 2e35 2e31 2f65 7861  erate/v3.5.1/exa
 00021200: 6d70 6c65 732f 6d65 6469 612f 7665 726d  mples/media/verm
 00021210: 6565 725f 6361 6e6e 795f 6564 6765 642e  eer_canny_edged.
 00021220: 706e 673e 605f 0d0a 0d0a 0d0a 2e2e 2063  png>`_........ c
 00021230: 6f64 652d 626c 6f63 6b3a 3a20 6261 7368  ode-block:: bash
 00021240: 0d0a 0d0a 2020 2020 2320 546f 7263 6820  ....    # Torch 
 00021250: 6578 616d 706c 652c 2075 7365 2022 7665  example, use "ve
 00021260: 726d 6565 725f 6361 6e6e 795f 6564 6765  rmeer_canny_edge
@@ -9060,15 +9060,15 @@
 00023630: 7220 6765 6e65 7261 7469 6f6e 2077 6974  r generation wit
 00023640: 6820 6120 6d6f 6465 6c20 2b20 6120 436f  h a model + a Co
 00023650: 6e74 726f 6c4e 6574 2e0d 0a0d 0a54 6869  ntrolNet.....Thi
 00023660: 7320 696d 6167 6520 6f66 2061 2060 686f  s image of a `ho
 00023670: 7273 6520 3c68 7474 7073 3a2f 2f72 6177  rse <https://raw
 00023680: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
 00023690: 6e74 2e63 6f6d 2f54 6572 696b 732f 6467  nt.com/Teriks/dg
-000236a0: 656e 6572 6174 652f 7633 2e35 2e30 2f65  enerate/v3.5.0/e
+000236a0: 656e 6572 6174 652f 7633 2e35 2e31 2f65  enerate/v3.5.1/e
 000236b0: 7861 6d70 6c65 732f 6d65 6469 612f 686f  xamples/media/ho
 000236c0: 7273 6532 2e6a 7065 673e 605f 0d0a 6973  rse2.jpeg>`_..is
 000236d0: 2075 7365 6420 696e 2074 6865 2065 7861   used in the exa
 000236e0: 6d70 6c65 2062 656c 6f77 2077 6974 6820  mple below with 
 000236f0: 6120 436f 6e74 726f 6c4e 6574 2074 6861  a ControlNet tha
 00023700: 7420 6973 2074 7261 696e 6564 2074 6f20  t is trained to 
 00023710: 6765 6e65 7261 7465 2069 6d61 6765 7320  generate images 
@@ -9300,15 +9300,15 @@
 00024530: 2069 6d61 6765 2075 7365 6420 696e 2074   image used in t
 00024540: 6865 2065 7861 6d70 6c65 2062 656c 6f77  he example below
 00024550: 2069 7320 7468 6973 2060 6c6f 7720 7265   is this `low re
 00024560: 736f 6c75 7469 6f6e 2063 6174 203c 6874  solution cat <ht
 00024570: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
 00024580: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
 00024590: 5465 7269 6b73 2f64 6765 6e65 7261 7465  Teriks/dgenerate
-000245a0: 2f76 332e 352e 302f 6578 616d 706c 6573  /v3.5.0/examples
+000245a0: 2f76 332e 352e 312f 6578 616d 706c 6573  /v3.5.1/examples
 000245b0: 2f6d 6564 6961 2f6c 6f77 5f72 6573 5f63  /media/low_res_c
 000245c0: 6174 2e70 6e67 3e60 5f0d 0a0d 0a2e 2e20  at.png>`_...... 
 000245d0: 636f 6465 2d62 6c6f 636b 3a3a 2062 6173  code-block:: bas
 000245e0: 680d 0a0d 0a20 2020 2023 2054 6865 2069  h....    # The i
 000245f0: 6d61 6765 2070 726f 6475 6365 6420 7769  mage produced wi
 00024600: 7468 2074 6869 7320 6d6f 6465 6c20 7769  th this model wi
 00024610: 6c6c 2062 650d 0a20 2020 2023 2074 776f  ll be..    # two
@@ -10351,15 +10351,15 @@
 000286e0: 7769 6e67 2069 7320 6120 636f 6e66 6967  wing is a config
 000286f0: 2066 696c 6520 6578 616d 706c 6520 7468   file example th
 00028700: 6174 2063 6f76 6572 7320 7665 7279 2062  at covers very b
 00028710: 6173 6963 2073 796e 7461 7820 636f 6e63  asic syntax conc
 00028720: 6570 7473 3a0d 0a0d 0a2e 2e20 636f 6465  epts:...... code
 00028730: 2d62 6c6f 636b 3a3a 206a 696e 6a61 0d0a  -block:: jinja..
 00028740: 0d0a 2020 2020 2321 2064 6765 6e65 7261  ..    #! dgenera
-00028750: 7465 2033 2e35 2e30 0d0a 0d0a 2020 2020  te 3.5.0....    
+00028750: 7465 2033 2e35 2e31 0d0a 0d0a 2020 2020  te 3.5.1....    
 00028760: 2320 4966 2061 2068 6173 682d 6261 6e67  # If a hash-bang
 00028770: 2076 6572 7369 6f6e 2069 7320 7072 6f76   version is prov
 00028780: 6964 6564 2069 6e20 7468 6520 666f 726d  ided in the form
 00028790: 6174 2061 626f 7665 0d0a 2020 2020 2320  at above..    # 
 000287a0: 6120 7761 726e 696e 6720 7769 6c6c 2062  a warning will b
 000287b0: 6520 7072 6f64 7563 6564 2069 6620 7468  e produced if th
 000287c0: 6520 7665 7273 696f 6e20 796f 7520 6172  e version you ar
@@ -10619,15 +10619,15 @@
 000297a0: 6060 5c73 6574 6060 2061 6e64 2060 605c  ``\set`` and ``\
 000297b0: 7365 7470 6060 2064 6972 6563 7469 7665  setp`` directive
 000297c0: 2077 696c 6c20 616c 736f 2062 6520 6d65   will also be me
 000297d0: 6e74 696f 6e65 6420 696e 2074 6869 7320  ntioned in this 
 000297e0: 6f75 7470 7574 2e0d 0a0d 0a2e 2e20 636f  output....... co
 000297f0: 6465 2d62 6c6f 636b 3a3a 206a 696e 6a61  de-block:: jinja
 00029800: 0d0a 0d0a 2020 2020 2321 2064 6765 6e65  ....    #! dgene
-00029810: 7261 7465 2033 2e35 2e30 0d0a 0d0a 2020  rate 3.5.0....  
+00029810: 7261 7465 2033 2e35 2e31 0d0a 0d0a 2020  rate 3.5.1....  
 00029820: 2020 2320 496e 766f 6361 7469 6f6e 2077    # Invocation w
 00029830: 696c 6c20 7072 6f63 6565 6420 6173 206e  ill proceed as n
 00029840: 6f72 6d61 6c0d 0a0d 0a20 2020 2073 7461  ormal....    sta
 00029850: 6269 6c69 7479 6169 2f73 7461 626c 652d  bilityai/stable-
 00029860: 6469 6666 7573 696f 6e2d 322d 3120 2d2d  diffusion-2-1 --
 00029870: 7072 6f6d 7074 7320 2261 206d 616e 2077  prompts "a man w
 00029880: 616c 6b69 6e67 206f 6e20 7468 6520 6d6f  alking on the mo
@@ -11530,15 +11530,15 @@
 0002d090: 730d 0a73 7563 6820 6173 2056 4145 7320  s..such as VAEs 
 0002d0a0: 6574 632e 206f 7574 7369 6465 206f 6620  etc. outside of 
 0002d0b0: 7265 6c79 696e 6720 6f6e 2074 6865 2063  relying on the c
 0002d0c0: 6163 6869 6e67 2073 7973 7465 6d2e 0d0a  aching system...
 0002d0d0: 0d0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
 0002d0e0: 3a20 6a69 6e6a 610d 0a0d 0a20 2020 2023  : jinja....    #
 0002d0f0: 2120 6467 656e 6572 6174 6520 332e 352e  ! dgenerate 3.5.
-0002d100: 300d 0a0d 0a20 2020 2023 2059 6f75 2063  0....    # You c
+0002d100: 310d 0a0d 0a20 2020 2023 2059 6f75 2063  1....    # You c
 0002d110: 616e 2064 6566 696e 6520 796f 7572 206f  an define your o
 0002d120: 776e 2074 656d 706c 6174 6520 7661 7269  wn template vari
 0002d130: 6162 6c65 7320 7769 7468 2074 6865 205c  ables with the \
 0002d140: 7365 7420 6469 7265 6374 6976 650d 0a20  set directive.. 
 0002d150: 2020 2023 2074 6865 205c 7365 7420 6469     # the \set di
 0002d160: 7265 6374 6976 6520 646f 6573 206e 6f74  rective does not
 0002d170: 2064 6f20 616e 7920 7368 656c 6c20 6172   do any shell ar
@@ -12017,15 +12017,15 @@
 0002ef00: 676c 6f62 206d 6f64 756c 652c 2079 6f75  glob module, you
 0002ef10: 2063 616e 2061 6c73 6f20 676c 6f62 2064   can also glob d
 0002ef20: 6972 6563 746f 7279 2773 2075 7369 6e67  irectory's using
 0002ef30: 2073 6865 6c6c 0d0a 676c 6f62 6269 6e67   shell..globbing
 0002ef40: 2e0d 0a0d 0a2e 2e20 636f 6465 2d62 6c6f  ....... code-blo
 0002ef50: 636b 3a3a 206a 696e 6a61 0d0a 0d0a 2020  ck:: jinja....  
 0002ef60: 2020 2321 2064 6765 6e65 7261 7465 2033    #! dgenerate 3
-0002ef70: 2e35 2e30 0d0a 0d0a 2020 2020 2320 676c  .5.0....    # gl
+0002ef70: 2e35 2e31 0d0a 0d0a 2020 2020 2320 676c  .5.1....    # gl
 0002ef80: 6f62 6269 6e67 2063 616e 2062 6520 7072  obbing can be pr
 0002ef90: 6566 6f72 6d65 6420 7669 6120 7368 656c  eformed via shel
 0002efa0: 6c20 6578 7061 6e73 696f 6e20 6f72 2075  l expansion or u
 0002efb0: 7369 6e67 0d0a 2020 2020 2320 7468 6520  sing..    # the 
 0002efc0: 676c 6f62 206d 6f64 756c 6520 696e 7369  glob module insi
 0002efd0: 6465 206a 696e 6a61 2074 656d 706c 6174  de jinja templat
 0002efe0: 6573 0d0a 0d0a 2020 2020 2320 6e6f 7465  es....    # note
@@ -12116,15 +12116,15 @@
 0002f530: 2d63 6f6d 6d61 6e64 2060 6069 6d61 6765  -command ``image
 0002f540: 2d70 726f 6365 7373 6060 2068 6173 2061  -process`` has a
 0002f550: 2063 6f6e 6669 6720 6469 7265 6374 6976   config directiv
 0002f560: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
 0002f570: 2e0d 0a0d 0a0d 0a2e 2e20 636f 6465 2d62  ......... code-b
 0002f580: 6c6f 636b 3a3a 206a 696e 6a61 0d0a 0d0a  lock:: jinja....
 0002f590: 2020 2020 2321 2064 6765 6e65 7261 7465      #! dgenerate
-0002f5a0: 2033 2e35 2e30 0d0a 0d0a 2020 2020 2320   3.5.0....    # 
+0002f5a0: 2033 2e35 2e31 0d0a 0d0a 2020 2020 2320   3.5.1....    # 
 0002f5b0: 7072 696e 7420 7468 6520 6865 6c70 206d  print the help m
 0002f5c0: 6573 7361 6765 206f 6620 2d2d 7375 622d  essage of --sub-
 0002f5d0: 636f 6d6d 616e 6420 696d 6167 652d 7072  command image-pr
 0002f5e0: 6f63 6573 732c 2074 6869 7320 646f 6573  ocess, this does
 0002f5f0: 0d0a 2020 2020 2320 6e6f 7420 6361 7573  ..    # not caus
 0002f600: 6520 7468 6520 636f 6e66 6967 2074 6f20  e the config to 
 0002f610: 6578 6974 0d0a 0d0a 2020 2020 5c69 6d61  exit....    \ima
@@ -12192,15 +12192,15 @@
 0002f9f0: 696d 6167 6520 7072 6f63 6573 7369 6e67  image processing
 0002fa00: 2075 7469 6c69 7469 6573 2061 7320 7375   utilities as su
 0002fa10: 6270 726f 6365 7373 6573 2066 726f 6d20  bprocesses from 
 0002fa20: 7769 7468 696e 2061 0d0a 636f 6e66 6967  within a..config
 0002fa30: 2073 6372 6970 742e 0d0a 0d0a 0d0a 2e2e   script.........
 0002fa40: 2063 6f64 652d 626c 6f63 6b3a 3a0d 0a0d   code-block::...
 0002fa50: 0a20 2020 2023 2120 6467 656e 6572 6174  .    #! dgenerat
-0002fa60: 6520 332e 352e 300d 0a0d 0a20 2020 2023  e 3.5.0....    #
+0002fa60: 6520 332e 352e 310d 0a0d 0a20 2020 2023  e 3.5.1....    #
 0002fa70: 2072 756e 2064 6765 6e65 7261 7465 2061   run dgenerate a
 0002fa80: 7320 6120 7375 6270 726f 6365 7373 2c20  s a subprocess, 
 0002fa90: 7265 6164 2061 2063 6f6e 6669 670d 0a20  read a config.. 
 0002faa0: 2020 2023 2061 6e64 2073 656e 6420 7374     # and send st
 0002fab0: 646f 7574 2061 6e64 2073 7464 6572 7220  dout and stderr 
 0002fac0: 746f 2061 2066 696c 650d 0a0d 0a20 2020  to a file....   
 0002fad0: 205c 6578 6563 2064 6765 6e65 7261 7465   \exec dgenerate
@@ -12227,15 +12227,15 @@
 0002fc20: 0a59 6f75 2063 616e 2065 7869 7420 6120  .You can exit a 
 0002fc30: 636f 6e66 6967 2065 6172 6c79 2069 6620  config early if 
 0002fc40: 6e65 6564 2062 6520 7573 696e 6720 7468  need be using th
 0002fc50: 6520 6060 5c65 7869 7460 6020 6469 7265  e ``\exit`` dire
 0002fc60: 6374 6976 650d 0a0d 0a0d 0a2e 2e20 636f  ctive........ co
 0002fc70: 6465 2d62 6c6f 636b 3a3a 206a 696e 6a61  de-block:: jinja
 0002fc80: 0d0a 0d0a 2020 2020 2321 2064 6765 6e65  ....    #! dgene
-0002fc90: 7261 7465 2033 2e35 2e30 0d0a 0d0a 2020  rate 3.5.0....  
+0002fc90: 7261 7465 2033 2e35 2e31 0d0a 0d0a 2020  rate 3.5.1....  
 0002fca0: 2020 2320 6578 6974 2074 6865 2070 726f    # exit the pro
 0002fcb0: 6365 7373 2077 6974 6820 7265 7475 726e  cess with return
 0002fcc0: 2063 6f64 6520 312c 2077 6869 6368 2069   code 1, which i
 0002fcd0: 6e64 6963 6174 6573 2061 6e20 6572 726f  ndicates an erro
 0002fce0: 720d 0a0d 0a20 2020 205c 7072 696e 7420  r....    \print 
 0002fcf0: 2273 6f6d 6520 6572 726f 7220 6f63 6375  "some error occu
 0002fd00: 7272 6564 220d 0a20 2020 205c 6578 6974  rred"..    \exit
@@ -12357,15 +12357,15 @@
 00030440: 6564 5f70 6c75 6769 6e5f 6d6f 6475 6c65  ed_plugin_module
 00030450: 7320 656c 7365 2027 2720 7d7d 0d0a 0d0a  s else '' }}....
 00030460: 436f 6e73 6f6c 6520 5549 0d0a 3d3d 3d3d  Console UI..====
 00030470: 3d3d 3d3d 3d3d 0d0a 0d0a 2e2e 2069 6d61  ======...... ima
 00030480: 6765 3a3a 2068 7474 7073 3a2f 2f72 6177  ge:: https://raw
 00030490: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
 000304a0: 6e74 2e63 6f6d 2f54 6572 696b 732f 6467  nt.com/Teriks/dg
-000304b0: 656e 6572 6174 652f 7633 2e35 2e30 2f65  enerate/v3.5.0/e
+000304b0: 656e 6572 6174 652f 7633 2e35 2e31 2f65  enerate/v3.5.1/e
 000304c0: 7861 6d70 6c65 732f 6d65 6469 612f 7569  xamples/media/ui
 000304d0: 2e67 6966 0d0a 2020 203a 616c 743a 2063  .gif..   :alt: c
 000304e0: 6f6e 736f 6c65 2075 690d 0a0d 0a59 6f75  onsole ui....You
 000304f0: 2063 616e 206c 6175 6e63 6820 6120 6372   can launch a cr
 00030500: 6f73 7320 706c 6174 666f 726d 2054 6b69  oss platform Tki
 00030510: 6e74 6572 2047 5549 2066 6f72 2069 6e74  nter GUI for int
 00030520: 6572 6163 7469 6e67 2077 6974 6820 610d  eracting with a.
@@ -12581,41 +12581,41 @@
 00031240: 2070 6c75 6769 6e73 2063 616e 2062 6520   plugins can be 
 00031250: 666f 756e 640d 0a69 6e20 7468 6520 6022  found..in the `"
 00031260: 7772 6974 696e 675f 706c 7567 696e 732f  writing_plugins/
 00031270: 696d 6167 655f 7072 6f63 6573 736f 7222  image_processor"
 00031280: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
 00031290: 2e63 6f6d 2f54 6572 696b 732f 6467 656e  .com/Teriks/dgen
 000312a0: 6572 6174 652f 7472 6565 2f76 332e 352e  erate/tree/v3.5.
-000312b0: 302f 6578 616d 706c 6573 2f77 7269 7469  0/examples/writi
+000312b0: 312f 6578 616d 706c 6573 2f77 7269 7469  1/examples/writi
 000312c0: 6e67 5f70 6c75 6769 6e73 2f69 6d61 6765  ng_plugins/image
 000312d0: 5f70 726f 6365 7373 6f72 3e60 5f0d 0a66  _processor>`_..f
 000312e0: 6f6c 6465 7220 6f66 2074 6865 2065 7861  older of the exa
 000312f0: 6d70 6c65 7320 666f 6c64 6572 2e0d 0a0d  mples folder....
 00031300: 0a54 6865 2073 6f75 7263 6520 636f 6465  .The source code
 00031310: 2066 6f72 2074 6865 2062 7569 6c74 2069   for the built i
 00031320: 6e20 6063 616e 6e79 203c 6874 7470 733a  n `canny <https:
 00031330: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6572  //github.com/Ter
 00031340: 696b 732f 6467 656e 6572 6174 652f 626c  iks/dgenerate/bl
-00031350: 6f62 2f76 332e 352e 302f 6467 656e 6572  ob/v3.5.0/dgener
+00031350: 6f62 2f76 332e 352e 312f 6467 656e 6572  ob/v3.5.1/dgener
 00031360: 6174 652f 696d 6167 6570 726f 6365 7373  ate/imageprocess
 00031370: 6f72 732f 6361 6e6e 792e 7079 3e60 5f20  ors/canny.py>`_ 
 00031380: 7072 6f63 6573 736f 722c 0d0a 7468 6520  processor,..the 
 00031390: 606f 7065 6e70 6f73 6520 3c68 7474 7073  `openpose <https
 000313a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5465  ://github.com/Te
 000313b0: 7269 6b73 2f64 6765 6e65 7261 7465 2f62  riks/dgenerate/b
-000313c0: 6c6f 622f 7633 2e35 2e30 2f64 6765 6e65  lob/v3.5.0/dgene
+000313c0: 6c6f 622f 7633 2e35 2e31 2f64 6765 6e65  lob/v3.5.1/dgene
 000313d0: 7261 7465 2f69 6d61 6765 7072 6f63 6573  rate/imageproces
 000313e0: 736f 7273 2f6f 7065 6e70 6f73 652e 7079  sors/openpose.py
 000313f0: 3e60 5f20 7072 6f63 6573 736f 722c 2061  >`_ processor, a
 00031400: 6e64 2074 6865 2073 696d 706c 650d 0a60  nd the simple..`
 00031410: 7069 6c6c 6f77 2069 6d61 6765 206f 7065  pillow image ope
 00031420: 7261 7469 6f6e 7320 3c68 7474 7073 3a2f  rations <https:/
 00031430: 2f67 6974 6875 622e 636f 6d2f 5465 7269  /github.com/Teri
 00031440: 6b73 2f64 6765 6e65 7261 7465 2f62 6c6f  ks/dgenerate/blo
-00031450: 622f 7633 2e35 2e30 2f64 6765 6e65 7261  b/v3.5.0/dgenera
+00031450: 622f 7633 2e35 2e31 2f64 6765 6e65 7261  b/v3.5.1/dgenera
 00031460: 7465 2f69 6d61 6765 7072 6f63 6573 736f  te/imageprocesso
 00031470: 7273 2f69 6d61 6765 6f70 732e 7079 3e60  rs/imageops.py>`
 00031480: 5f20 7072 6f63 6573 736f 7273 2063 616e  _ processors can
 00031490: 2061 6c73 6f0d 0a62 6520 6f66 2072 6566   also..be of ref
 000314a0: 6572 656e 6365 2061 7320 7468 6579 2061  erence as they a
 000314b0: 7265 2077 7269 7474 656e 2061 7320 696e  re written as in
 000314c0: 7465 726e 616c 2069 6d61 6765 2070 726f  ternal image pro
@@ -12625,29 +12625,29 @@
 00031500: 2064 6972 6563 7469 7665 7320 6361 6e20   directives can 
 00031510: 6265 2066 6f75 6e64 2069 6e20 7468 650d  be found in the.
 00031520: 0a60 2277 7269 7469 6e67 5f70 6c75 6769  .`"writing_plugi
 00031530: 6e73 2f63 6f6e 6669 675f 6469 7265 6374  ns/config_direct
 00031540: 6976 6522 203c 6874 7470 733a 2f2f 6769  ive" <https://gi
 00031550: 7468 7562 2e63 6f6d 2f54 6572 696b 732f  thub.com/Teriks/
 00031560: 6467 656e 6572 6174 652f 7472 6565 2f76  dgenerate/tree/v
-00031570: 332e 352e 302f 6578 616d 706c 6573 2f77  3.5.0/examples/w
+00031570: 332e 352e 312f 6578 616d 706c 6573 2f77  3.5.1/examples/w
 00031580: 7269 7469 6e67 5f70 6c75 6769 6e73 2f63  riting_plugins/c
 00031590: 6f6e 6669 675f 6469 7265 6374 6976 653e  onfig_directive>
 000315a0: 605f 2066 6f6c 6465 720d 0a6f 6620 7468  `_ folder..of th
 000315b0: 6520 6578 616d 706c 6573 2066 6f6c 6465  e examples folde
 000315c0: 722e 2043 6f6e 6669 6720 7465 6d70 6c61  r. Config templa
 000315d0: 7465 2066 756e 6374 696f 6e73 2063 616e  te functions can
 000315e0: 2061 6c73 6f20 6265 2069 6d70 6c65 6d65   also be impleme
 000315f0: 6e74 6564 2062 7920 706c 7567 696e 732c  nted by plugins,
 00031600: 0d0a 7365 653a 2060 2277 7269 7469 6e67  ..see: `"writing
 00031610: 5f70 6c75 6769 6e73 2f74 656d 706c 6174  _plugins/templat
 00031620: 655f 6675 6e63 7469 6f6e 2220 3c68 7474  e_function" <htt
 00031630: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00031640: 5465 7269 6b73 2f64 6765 6e65 7261 7465  Teriks/dgenerate
-00031650: 2f74 7265 652f 7633 2e35 2e30 2f65 7861  /tree/v3.5.0/exa
+00031650: 2f74 7265 652f 7633 2e35 2e31 2f65 7861  /tree/v3.5.1/exa
 00031660: 6d70 6c65 732f 7772 6974 696e 675f 706c  mples/writing_pl
 00031670: 7567 696e 732f 7465 6d70 6c61 7465 5f66  ugins/template_f
 00031680: 756e 6374 696f 6e3e 605f 0d0a 0d0a 4375  unction>`_....Cu
 00031690: 7272 656e 746c 7920 7468 6520 6f6e 6c79  rrently the only
 000316a0: 2069 6e74 6572 6e61 6c20 6469 7265 6374   internal direct
 000316b0: 6976 6520 7468 6174 2069 7320 696d 706c  ive that is impl
 000316c0: 656d 656e 7465 6420 6173 2061 2070 6c75  emented as a plu
@@ -12655,15 +12655,15 @@
 000316e0: 6167 655f 7072 6f63 6573 7360 6020 6469  age_process`` di
 000316f0: 7265 6374 6976 652c 0d0a 7768 6f27 7320  rective,..who's 
 00031700: 736f 7572 6365 2066 696c 6520 6063 616e  source file `can
 00031710: 2062 6520 6c6f 6361 7465 6420 6865 7265   be located here
 00031720: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
 00031730: 2e63 6f6d 2f54 6572 696b 732f 6467 656e  .com/Teriks/dgen
 00031740: 6572 6174 652f 626c 6f62 2f76 332e 352e  erate/blob/v3.5.
-00031750: 302f 6467 656e 6572 6174 652f 6261 7463  0/dgenerate/batc
+00031750: 312f 6467 656e 6572 6174 652f 6261 7463  1/dgenerate/batc
 00031760: 6870 726f 6365 7373 2f69 6d61 6765 5f70  hprocess/image_p
 00031770: 726f 6365 7373 5f64 6972 6563 7469 7665  rocess_directive
 00031780: 2e70 793e 605f 2c0d 0a74 6865 2073 6f75  .py>`_,..the sou
 00031790: 7263 6520 6669 6c65 2066 6f72 2074 6869  rce file for thi
 000317a0: 7320 6469 7265 6374 6976 6520 6973 2074  s directive is t
 000317b0: 6572 7365 2061 7320 6d6f 7374 206f 6620  erse as most of 
 000317c0: 6060 5c69 6d61 6765 5f70 726f 6365 7373  ``\image_process
@@ -12676,15 +12676,15 @@
 00031830: 6368 2069 7320 616c 736f 2075 7365 6420  ch is also used 
 00031840: 666f 7220 6060 2d2d 7375 622d 636f 6d6d  for ``--sub-comm
 00031850: 616e 6420 696d 6167 652d 7072 6f63 6573  and image-proces
 00031860: 7360 6020 6973 0d0a 6069 7320 696d 706c  s`` is..`is impl
 00031870: 656d 656e 7465 6420 6865 7265 203c 6874  emented here <ht
 00031880: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00031890: 2f54 6572 696b 732f 6467 656e 6572 6174  /Teriks/dgenerat
-000318a0: 652f 626c 6f62 2f76 332e 352e 302f 6467  e/blob/v3.5.0/dg
+000318a0: 652f 626c 6f62 2f76 332e 352e 312f 6467  e/blob/v3.5.1/dg
 000318b0: 656e 6572 6174 652f 696d 6167 655f 7072  enerate/image_pr
 000318c0: 6f63 6573 733e 605f 2e0d 0a0d 0a46 696c  ocess>`_.....Fil
 000318d0: 6520 4361 6368 6520 436f 6e74 726f 6c0d  e Cache Control.
 000318e0: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .===============
 000318f0: 3d3d 3d0d 0a0d 0a64 6765 6e65 7261 7465  ===....dgenerate
 00031900: 2077 696c 6c20 6361 6368 6520 6060 2d2d   will cache ``--
 00031910: 696d 6167 652d 7365 6564 7360 6020 6669  image-seeds`` fi
```

### Comparing `dgenerate-3.5.0/dgenerate/__init__.py` & `dgenerate-3.5.1/dgenerate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
 # LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
 # HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 # LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '3.5.0'
+__version__ = '3.5.1'
 
 import os
 import sys
 
 __am_dgenerate_app = \
     os.path.splitext(
         os.path.basename(os.path.realpath(sys.argv[0])))[0] in {'dgenerate', 'dgenerate_windowed'}
```

### Comparing `dgenerate-3.5.0/dgenerate/arguments.py` & `dgenerate-3.5.1/dgenerate/arguments.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/batchprocess/__init__.py` & `dgenerate-3.5.1/dgenerate/batchprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/batchprocess/batchprocessor.py` & `dgenerate-3.5.1/dgenerate/batchprocess/batchprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,22 +325,24 @@
             jinja_env.globals[name] = func
 
             if len(inspect.signature(func).parameters) > 0:
                 jinja_env.filters[name] = func
 
         if stream:
             def stream_generator():
-                buffer = ""
+                buffer = ''
                 try:
                     for piece in jinja_env.from_string(string). \
                             stream(**self.template_variables):
                         buffer += piece
                         while '\n' in buffer:
                             line, buffer = buffer.split('\n', 1)
                             yield os.path.expandvars(line)
+                    if buffer:
+                        yield os.path.expandvars(buffer)
                 except Exception as e:
                     raise BatchProcessError(f'Template Render Error: {str(e).strip()}')
 
             return stream_generator()
         else:
             try:
                 return self.expand_vars(
```

### Comparing `dgenerate-3.5.0/dgenerate/batchprocess/configrunner.py` & `dgenerate-3.5.1/dgenerate/batchprocess/configrunner.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/batchprocess/configrunnerplugin.py` & `dgenerate-3.5.1/dgenerate/batchprocess/configrunnerplugin.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/batchprocess/configrunnerpluginloader.py` & `dgenerate-3.5.1/dgenerate/batchprocess/configrunnerpluginloader.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/batchprocess/image_process_directive.py` & `dgenerate-3.5.1/dgenerate/batchprocess/image_process_directive.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/console/__init__.py` & `dgenerate-3.5.1/dgenerate/console/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/console/console.py` & `dgenerate-3.5.1/dgenerate/console/console.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/console/filedialog.py` & `dgenerate-3.5.1/dgenerate/console/filedialog.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/console/finddialog.py` & `dgenerate-3.5.1/dgenerate/console/finddialog.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/console/karrasschedulerselect.py` & `dgenerate-3.5.1/dgenerate/console/karrasschedulerselect.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/console/recipes.py` & `dgenerate-3.5.1/dgenerate/console/recipes.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/console/recipesform.py` & `dgenerate-3.5.1/dgenerate/console/recipesform.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/console/resources.py` & `dgenerate-3.5.1/dgenerate/console/resources.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/console/scrolledtext.py` & `dgenerate-3.5.1/dgenerate/console/scrolledtext.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/dgenerate.py` & `dgenerate-3.5.1/dgenerate/dgenerate.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/events.py` & `dgenerate-3.5.1/dgenerate/events.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/canny/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/canny/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/util.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/wholebody.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/wholebody.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/hed/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/Resnet.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/Resnext_torch.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/depthmap.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/multi_depth_model_woauxi.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/net_tools.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/leres/network_auxi.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model_hg.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/networks.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/options/base_options.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/options/test_options.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/leres/pix2pix/util/util.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/lineart/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/lineart/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/lineart_anime/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/lineart_anime/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mediapipe_face/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mediapipe_face/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mediapipe_face/mediapipe_face_common.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mediapipe_face/mediapipe_face_common.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/api.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/api.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/blocks.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/dpt_depth.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/midas_net.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/midas_net_custom.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/transforms.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/midas/vit.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/midas/utils.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/midas/utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/mlsd/utils.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/NNET.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/NNET.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/baseline.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/baseline.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/decoder.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/decoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/encoder.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/encoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/submodules.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/submodules.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/body.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/body.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/face.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/face.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/hand.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/hand.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/model.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/open_pose/util.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/open_pose/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/pidi/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/pidi/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/pidi/model.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/pidi/model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/processor.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/processor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/automatic_mask_generator.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/build_sam.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/common.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/image_encoder.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/mask_decoder.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/prompt_encoder.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/sam.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/modeling/transformer.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/predictor.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/utils/amg.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/utils/onnx.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/segment_anything/utils/transforms.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/shuffle/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/tests/test_processor.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/tests/test_processor_pytest.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/tests/test_processor_pytest.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/util.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/builder.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/builder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/depth_model.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/depth_model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/attractor.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/attractor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/model_io.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/model_io.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/arg_utils.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/config.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/config.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py` & `dgenerate-3.5.1/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/filecache.py` & `dgenerate-3.5.1/dgenerate/filecache.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/filelock.py` & `dgenerate-3.5.1/dgenerate/filelock.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/files.py` & `dgenerate-3.5.1/dgenerate/files.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/icon.ico` & `dgenerate-3.5.1/dgenerate/icon.ico`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/image.py` & `dgenerate-3.5.1/dgenerate/image.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/image_process/__init__.py` & `dgenerate-3.5.1/dgenerate/image_process/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/image_process/arguments.py` & `dgenerate-3.5.1/dgenerate/image_process/arguments.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/image_process/invoker.py` & `dgenerate-3.5.1/dgenerate/image_process/invoker.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/image_process/renderloop.py` & `dgenerate-3.5.1/dgenerate/image_process/renderloop.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/image_process/renderloopconfig.py` & `dgenerate-3.5.1/dgenerate/image_process/renderloopconfig.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/__init__.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/canny.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/canny.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/exceptions.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/exceptions.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/hed.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/hed.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/imageops.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/imageops.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/imageprocessor.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/imageprocessor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/imageprocessorchain.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/imageprocessorchain.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/imageprocessorloader.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/imageprocessorloader.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/imageprocessormixin.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/imageprocessormixin.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/leres.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/leres.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/linart_anime.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/linart_anime.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/lineart.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/lineart.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/midas.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/midas.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/mlsd.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/mlsd.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/normal_bae.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/normal_bae.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/openpose.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/openpose.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/pidi.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/pidi.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/sam.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/sam.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/imageprocessors/upscaler.py` & `dgenerate-3.5.1/dgenerate/imageprocessors/upscaler.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/invoker.py` & `dgenerate-3.5.1/dgenerate/invoker.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/mediainput.py` & `dgenerate-3.5.1/dgenerate/mediainput.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/mediaoutput.py` & `dgenerate-3.5.1/dgenerate/mediaoutput.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/memoize.py` & `dgenerate-3.5.1/dgenerate/memoize.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/memory.py` & `dgenerate-3.5.1/dgenerate/memory.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/messages.py` & `dgenerate-3.5.1/dgenerate/messages.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/pipelinewrapper/__init__.py` & `dgenerate-3.5.1/dgenerate/pipelinewrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/pipelinewrapper/cache.py` & `dgenerate-3.5.1/dgenerate/pipelinewrapper/cache.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/pipelinewrapper/constants.py` & `dgenerate-3.5.1/dgenerate/pipelinewrapper/constants.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/pipelinewrapper/enums.py` & `dgenerate-3.5.1/dgenerate/pipelinewrapper/enums.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/pipelinewrapper/hfutil.py` & `dgenerate-3.5.1/dgenerate/pipelinewrapper/hfutil.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/pipelinewrapper/pipelines.py` & `dgenerate-3.5.1/dgenerate/pipelinewrapper/pipelines.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/pipelinewrapper/uris.py` & `dgenerate-3.5.1/dgenerate/pipelinewrapper/uris.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/pipelinewrapper/util.py` & `dgenerate-3.5.1/dgenerate/pipelinewrapper/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/pipelinewrapper/wrapper.py` & `dgenerate-3.5.1/dgenerate/pipelinewrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/plugin.py` & `dgenerate-3.5.1/dgenerate/plugin.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/prompt.py` & `dgenerate-3.5.1/dgenerate/prompt.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/renderloop.py` & `dgenerate-3.5.1/dgenerate/renderloop.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/renderloopconfig.py` & `dgenerate-3.5.1/dgenerate/renderloopconfig.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/subcommands/__init__.py` & `dgenerate-3.5.1/dgenerate/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/subcommands/exceptions.py` & `dgenerate-3.5.1/dgenerate/subcommands/exceptions.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/subcommands/image_process.py` & `dgenerate-3.5.1/dgenerate/subcommands/image_process.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/subcommands/subcommand.py` & `dgenerate-3.5.1/dgenerate/subcommands/subcommand.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/subcommands/subcommandloader.py` & `dgenerate-3.5.1/dgenerate/subcommands/subcommandloader.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/textprocessing.py` & `dgenerate-3.5.1/dgenerate/textprocessing.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate/types.py` & `dgenerate-3.5.1/dgenerate/types.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate.egg-info/PKG-INFO` & `dgenerate-3.5.1/dgenerate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2064 6765  : 2.1..Name: dge
 00000020: 6e65 7261 7465 0d0a 5665 7273 696f 6e3a  nerate..Version:
-00000030: 2033 2e35 2e30 0d0a 5375 6d6d 6172 793a   3.5.0..Summary:
+00000030: 2033 2e35 2e31 0d0a 5375 6d6d 6172 793a   3.5.1..Summary:
 00000040: 2042 6174 6368 2069 6d61 6765 2067 656e   Batch image gen
 00000050: 6572 6174 696f 6e20 616e 6420 6d61 6e69  eration and mani
 00000060: 7075 6c61 7469 6f6e 2074 6f6f 6c20 7375  pulation tool su
 00000070: 7070 6f72 7469 6e67 2053 7461 626c 6520  pporting Stable 
 00000080: 4469 6666 7573 696f 6e20 616e 6420 7265  Diffusion and re
 00000090: 6c61 7465 6420 7465 6368 6e69 7175 6573  lated techniques
 000000a0: 202f 2061 6c67 6f72 6974 686d 732c 2077   / algorithms, w
@@ -250,18 +250,18 @@
 00000f90: 2272 6561 6474 6865 646f 6373 220d 0a0d  "readthedocs"...
 00000fa0: 0a2e 2e20 7c44 6f63 756d 656e 7461 7469  ... |Documentati
 00000fb0: 6f6e 2053 7461 7475 737c 2069 6d61 6765  on Status| image
 00000fc0: 3a3a 2068 7474 7073 3a2f 2f72 6561 6474  :: https://readt
 00000fd0: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
 00000fe0: 6374 732f 6467 656e 6572 6174 652f 6261  cts/dgenerate/ba
 00000ff0: 6467 652f 3f76 6572 7369 6f6e 3d76 332e  dge/?version=v3.
-00001000: 352e 300d 0a20 2020 3a74 6172 6765 743a  5.0..   :target:
+00001000: 352e 310d 0a20 2020 3a74 6172 6765 743a  5.1..   :target:
 00001010: 2068 7474 703a 2f2f 6467 656e 6572 6174   http://dgenerat
 00001020: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00001030: 2f65 6e2f 7633 2e35 2e30 2f0d 0a0d 0a4f  /en/v3.5.0/....O
+00001030: 2f65 6e2f 7633 2e35 2e31 2f0d 0a0d 0a4f  /en/v3.5.1/....O
 00001040: 7665 7276 6965 770d 0a3d 3d3d 3d3d 3d3d  verview..=======
 00001050: 3d0d 0a0d 0a7c 446f 6375 6d65 6e74 6174  =....|Documentat
 00001060: 696f 6e20 5374 6174 7573 7c0d 0a0d 0a2a  ion Status|....*
 00001070: 2a64 6765 6e65 7261 7465 2a2a 2069 7320  *dgenerate** is 
 00001080: 6120 636f 6d6d 616e 6420 6c69 6e65 2074  a command line t
 00001090: 6f6f 6c20 616e 6420 6c69 6272 6172 7920  ool and library 
 000010a0: 666f 7220 6765 6e65 7261 7469 6e67 2069  for generating i
@@ -386,15 +386,15 @@
 00001810: 7469 6f6e 7320 6275 7420 6578 7472 616f  tions but extrao
 00001820: 7264 696e 6172 696c 7920 736c 6f77 2e0d  rdinarily slow..
 00001830: 0a0d 0a46 6f72 206c 6962 7261 7279 2064  ...For library d
 00001840: 6f63 756d 656e 7461 7469 6f6e 2076 6973  ocumentation vis
 00001850: 6974 2060 7265 6164 7468 6564 6f63 7320  it `readthedocs 
 00001860: 3c68 7474 703a 2f2f 6467 656e 6572 6174  <http://dgenerat
 00001870: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00001880: 2f65 6e2f 7633 2e35 2e30 2f3e 605f 2e0d  /en/v3.5.0/>`_..
+00001880: 2f65 6e2f 7633 2e35 2e31 2f3e 605f 2e0d  /en/v3.5.1/>`_..
 00001890: 0a0d 0a2d 2d2d 2d0d 0a0d 0a2a 2048 6f77  ...----....* How
 000018a0: 2074 6f20 696e 7374 616c 6c0d 0a20 2020   to install..   
 000018b0: 202a 2060 5769 6e64 6f77 7320 496e 7374   * `Windows Inst
 000018c0: 616c 6c60 5f0d 0a20 2020 202a 2060 4c69  all`_..    * `Li
 000018d0: 6e75 7820 6f72 2057 534c 2049 6e73 7461  nux or WSL Insta
 000018e0: 6c6c 605f 0d0a 0d0a 2a20 5573 6167 6520  ll`_....* Usage 
 000018f0: 4578 616d 706c 6573 0d0a 2020 2020 2a20  Examples..    * 
@@ -4920,15 +4920,15 @@
 00013370: 2020 2020 2020 2020 2020 2275 7365 645f            "used_
 00013380: 7065 7263 656e 7420 3e20 3730 2220 466f  percent > 70" Fo
 00013390: 7220 5379 6e74 6178 2053 6565 3a20 5b68  r Syntax See: [h
 000133a0: 7474 7073 3a2f 2f64 6765 6e65 7261 7465  ttps://dgenerate
 000133b0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
 000133c0: 656e 2f76 0d0a 2020 2020 2020 2020 2020  en/v..          
 000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 2020 332e 352e 302f 6467 656e 6572 6174    3.5.0/dgenerat
+000133e0: 2020 332e 352e 312f 6467 656e 6572 6174    3.5.1/dgenerat
 000133f0: 655f 7375 626d 6f64 756c 6573 2e68 746d  e_submodules.htm
 00013400: 6c23 6467 656e 6572 6174 652e 7069 7065  l#dgenerate.pipe
 00013410: 6c69 6e65 7772 6170 7065 722e 4341 4348  linewrapper.CACH
 00013420: 455f 4d45 4d4f 5259 5f43 4f4e 0d0a 2020  E_MEMORY_CON..  
 00013430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013440: 2020 2020 2020 2020 2020 5354 5241 494e            STRAIN
 00013450: 5453 5d0d 0a20 2020 2020 202d 706d 6320  TS]..      -pmc 
@@ -4973,15 +4973,15 @@
 000136c0: 6520 3e20 2861 7661 696c 6162 6c65 202a  e > (available *
 000136d0: 2030 2e37 3529 2220 466f 7220 5379 6e74   0.75)" For Synt
 000136e0: 6178 2053 6565 3a20 5b68 7474 7073 3a2f  ax See: [https:/
 000136f0: 2f64 6765 6e65 7261 7465 2e72 650d 0a20  /dgenerate.re.. 
 00013700: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013710: 2020 2020 2020 2020 2020 2061 6474 6865             adthe
 00013720: 646f 6373 2e69 6f2f 656e 2f76 332e 352e  docs.io/en/v3.5.
-00013730: 302f 6467 656e 6572 6174 655f 7375 626d  0/dgenerate_subm
+00013730: 312f 6467 656e 6572 6174 655f 7375 626d  1/dgenerate_subm
 00013740: 6f64 756c 6573 2e68 746d 6c23 6467 656e  odules.html#dgen
 00013750: 6572 6174 652e 7069 7065 6c69 6e65 7772  erate.pipelinewr
 00013760: 6170 7065 720d 0a20 2020 2020 2020 2020  apper..         
 00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013780: 2020 202e 5049 5045 4c49 4e45 5f43 4143     .PIPELINE_CAC
 00013790: 4845 5f4d 454d 4f52 595f 434f 4e53 5452  HE_MEMORY_CONSTR
 000137a0: 4149 4e54 535d 0d0a 2020 2020 2020 2d75  AINTS]..      -u
@@ -5022,15 +5022,15 @@
 000139d0: 756e 6574 5f73 697a 6520 3e20 2861 7661  unet_size > (ava
 000139e0: 696c 6162 6c65 202a 2030 2e37 3529 2220  ilable * 0.75)" 
 000139f0: 466f 720d 0a20 2020 2020 2020 2020 2020  For..           
 00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a10: 2053 796e 7461 7820 5365 653a 205b 6874   Syntax See: [ht
 00013a20: 7470 733a 2f2f 6467 656e 6572 6174 652e  tps://dgenerate.
 00013a30: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00013a40: 6e2f 7633 2e35 2e30 2f64 6765 6e65 7261  n/v3.5.0/dgenera
+00013a40: 6e2f 7633 2e35 2e31 2f64 6765 6e65 7261  n/v3.5.1/dgenera
 00013a50: 7465 5f73 7562 6d6f 6475 6c0d 0a20 2020  te_submodul..   
 00013a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a70: 2020 2020 2020 2020 2065 732e 6874 6d6c           es.html
 00013a80: 2364 6765 6e65 7261 7465 2e70 6970 656c  #dgenerate.pipel
 00013a90: 696e 6577 7261 7070 6572 2e55 4e45 545f  inewrapper.UNET_
 00013aa0: 4341 4348 455f 4d45 4d4f 5259 5f43 4f4e  CACHE_MEMORY_CON
 00013ab0: 5354 5241 494e 5453 5d0d 0a20 2020 2020  STRAINTS]..     
@@ -5071,15 +5071,15 @@
 00013ce0: 6165 5f73 697a 6520 3e20 2861 7661 696c  ae_size > (avail
 00013cf0: 6162 6c65 202a 2030 2e37 3529 2220 466f  able * 0.75)" Fo
 00013d00: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
 00013d10: 2020 2020 2020 2020 2020 2020 2020 2053                 S
 00013d20: 796e 7461 7820 5365 653a 205b 6874 7470  yntax See: [http
 00013d30: 733a 2f2f 6467 656e 6572 6174 652e 7265  s://dgenerate.re
 00013d40: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00013d50: 7633 2e35 2e30 2f64 6765 6e65 7261 7465  v3.5.0/dgenerate
+00013d50: 7633 2e35 2e31 2f64 6765 6e65 7261 7465  v3.5.1/dgenerate
 00013d60: 5f73 7562 6d6f 6475 6c0d 0a20 2020 2020  _submodul..     
 00013d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013d80: 2020 2020 2020 2065 732e 6874 6d6c 2364         es.html#d
 00013d90: 6765 6e65 7261 7465 2e70 6970 656c 696e  generate.pipelin
 00013da0: 6577 7261 7070 6572 2e56 4145 5f43 4143  ewrapper.VAE_CAC
 00013db0: 4845 5f4d 454d 4f52 595f 434f 4e53 5452  HE_MEMORY_CONSTR
 00013dc0: 4149 4e54 535d 0d0a 2020 2020 2020 2d63  AINTS]..      -c
@@ -5124,15 +5124,15 @@
 00014030: 2020 2020 2020 2020 2028 6176 6169 6c61           (availa
 00014040: 626c 6520 2a20 302e 3735 2922 2046 6f72  ble * 0.75)" For
 00014050: 2053 796e 7461 7820 5365 653a 205b 6874   Syntax See: [ht
 00014060: 7470 733a 2f2f 6467 656e 6572 6174 652e  tps://dgenerate.
 00014070: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
 00014080: 6e2f 760d 0a20 2020 2020 2020 2020 2020  n/v..           
 00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140a0: 2033 2e35 2e30 2f64 6765 6e65 7261 7465   3.5.0/dgenerate
+000140a0: 2033 2e35 2e31 2f64 6765 6e65 7261 7465   3.5.1/dgenerate
 000140b0: 5f73 7562 6d6f 6475 6c65 732e 6874 6d6c  _submodules.html
 000140c0: 2364 6765 6e65 7261 7465 2e70 6970 656c  #dgenerate.pipel
 000140d0: 696e 6577 7261 7070 6572 2e43 4f4e 5452  inewrapper.CONTR
 000140e0: 4f4c 5f4e 4554 5f43 4143 480d 0a20 2020  OL_NET_CACH..   
 000140f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014100: 2020 2020 2020 2020 2045 5f4d 454d 4f52           E_MEMOR
 00014110: 595f 434f 4e53 5452 4149 4e54 535d 0d0a  Y_CONSTRAINTS]..
@@ -5216,27 +5216,27 @@
 000145f0: 6465 782d 7572 6c20 6874 7470 733a 2f2f  dex-url https://
 00014600: 646f 776e 6c6f 6164 2e70 7974 6f72 6368  download.pytorch
 00014610: 2e6f 7267 2f77 686c 2f63 7531 3231 2f22  .org/whl/cu121/"
 00014620: 0d0a 0d0a 2020 2020 2320 4966 2079 6f75  ....    # If you
 00014630: 2077 616e 7420 6120 7370 6563 6966 6963   want a specific
 00014640: 2076 6572 7369 6f6e 0d0a 0d0a 2020 2020   version....    
 00014650: 7069 7078 2069 6e73 7461 6c6c 2064 6765  pipx install dge
-00014660: 6e65 7261 7465 3d3d 332e 352e 3020 5e0d  nerate==3.5.0 ^.
+00014660: 6e65 7261 7465 3d3d 332e 352e 3120 5e0d  nerate==3.5.1 ^.
 00014670: 0a20 2020 202d 2d70 6970 2d61 7267 7320  .    --pip-args 
 00014680: 222d 2d65 7874 7261 2d69 6e64 6578 2d75  "--extra-index-u
 00014690: 726c 2068 7474 7073 3a2f 2f64 6f77 6e6c  rl https://downl
 000146a0: 6f61 642e 7079 746f 7263 682e 6f72 672f  oad.pytorch.org/
 000146b0: 7768 6c2f 6375 3132 312f 220d 0a0d 0a20  whl/cu121/".... 
 000146c0: 2020 2023 2059 6f75 2063 616e 2069 6e73     # You can ins
 000146d0: 7461 6c6c 2077 6974 686f 7574 2070 6970  tall without pip
 000146e0: 7820 696e 746f 2079 6f75 7220 6f77 6e20  x into your own 
 000146f0: 656e 7669 726f 6e6d 656e 7420 6c69 6b65  environment like
 00014700: 2073 6f0d 0a0d 0a20 2020 2070 6970 2069   so....    pip i
 00014710: 6e73 7461 6c6c 2064 6765 6e65 7261 7465  nstall dgenerate
-00014720: 3d3d 332e 352e 3020 2d2d 6578 7472 612d  ==3.5.0 --extra-
+00014720: 3d3d 332e 352e 3120 2d2d 6578 7472 612d  ==3.5.1 --extra-
 00014730: 696e 6465 782d 7572 6c20 6874 7470 733a  index-url https:
 00014740: 2f2f 646f 776e 6c6f 6164 2e70 7974 6f72  //download.pytor
 00014750: 6368 2e6f 7267 2f77 686c 2f63 7531 3231  ch.org/whl/cu121
 00014760: 2f0d 0a0d 0a0d 0a49 7420 6973 2072 6563  /......It is rec
 00014770: 6f6d 6d65 6e64 6564 2074 6f20 696e 7374  ommended to inst
 00014780: 616c 6c20 6467 656e 6572 6174 6520 7769  all dgenerate wi
 00014790: 7468 2070 6970 7820 6966 2079 6f75 2061  th pipx if you a
@@ -5418,26 +5418,26 @@
 00015290: 6f67 6c65 6170 6973 2e63 6f6d 2f6a 6178  ogleapis.com/jax
 000152a0: 2d72 656c 6561 7365 732f 6a61 785f 6375  -releases/jax_cu
 000152b0: 6461 5f72 656c 6561 7365 732e 6874 6d6c  da_releases.html
 000152c0: 220d 0a0d 0a20 2020 2023 2049 6620 796f  "....    # If yo
 000152d0: 7520 7761 6e74 2061 2073 7065 6369 6669  u want a specifi
 000152e0: 6320 7665 7273 696f 6e0d 0a0d 0a20 2020  c version....   
 000152f0: 2070 6970 7820 696e 7374 616c 6c20 6467   pipx install dg
-00015300: 656e 6572 6174 653d 3d33 2e35 2e30 205c  enerate==3.5.0 \
+00015300: 656e 6572 6174 653d 3d33 2e35 2e31 205c  enerate==3.5.1 \
 00015310: 0d0a 2020 2020 2d2d 7069 702d 6172 6773  ..    --pip-args
 00015320: 2022 2d2d 6578 7472 612d 696e 6465 782d   "--extra-index-
 00015330: 7572 6c20 6874 7470 733a 2f2f 646f 776e  url https://down
 00015340: 6c6f 6164 2e70 7974 6f72 6368 2e6f 7267  load.pytorch.org
 00015350: 2f77 686c 2f63 7531 3231 2f22 0d0a 0d0a  /whl/cu121/"....
 00015360: 2020 2020 2320 5370 6563 6966 6963 2076      # Specific v
 00015370: 6572 7369 6f6e 2077 6974 6820 666c 6178  ersion with flax
 00015380: 2f6a 6178 2073 7570 706f 7274 0d0a 0d0a  /jax support....
 00015390: 2020 2020 7069 7078 2069 6e73 7461 6c6c      pipx install
 000153a0: 2064 6765 6e65 7261 7465 5b66 6c61 785d   dgenerate[flax]
-000153b0: 3d3d 332e 352e 3020 5c0d 0a20 2020 202d  ==3.5.0 \..    -
+000153b0: 3d3d 332e 352e 3120 5c0d 0a20 2020 202d  ==3.5.1 \..    -
 000153c0: 2d70 6970 2d61 7267 7320 222d 2d65 7874  -pip-args "--ext
 000153d0: 7261 2d69 6e64 6578 2d75 726c 2068 7474  ra-index-url htt
 000153e0: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
 000153f0: 746f 7263 682e 6f72 672f 7768 6c2f 6375  torch.org/whl/cu
 00015400: 3132 312f 205c 0d0a 2020 2020 2d66 2068  121/ \..    -f h
 00015410: 7474 7073 3a2f 2f73 746f 7261 6765 2e67  ttps://storage.g
 00015420: 6f6f 676c 6561 7069 732e 636f 6d2f 6a61  oogleapis.com/ja
@@ -5445,23 +5445,23 @@
 00015440: 7564 615f 7265 6c65 6173 6573 2e68 746d  uda_releases.htm
 00015450: 6c22 0d0a 0d0a 2020 2020 2320 596f 7520  l"....    # You 
 00015460: 6361 6e20 696e 7374 616c 6c20 7769 7468  can install with
 00015470: 6f75 7420 7069 7078 2069 6e74 6f20 796f  out pipx into yo
 00015480: 7572 206f 776e 2065 6e76 6972 6f6e 6d65  ur own environme
 00015490: 6e74 206c 696b 6520 736f 0d0a 0d0a 2020  nt like so....  
 000154a0: 2020 7069 7033 2069 6e73 7461 6c6c 2064    pip3 install d
-000154b0: 6765 6e65 7261 7465 3d3d 332e 352e 3020  generate==3.5.0 
+000154b0: 6765 6e65 7261 7465 3d3d 332e 352e 3120  generate==3.5.1 
 000154c0: 2d2d 6578 7472 612d 696e 6465 782d 7572  --extra-index-ur
 000154d0: 6c20 6874 7470 733a 2f2f 646f 776e 6c6f  l https://downlo
 000154e0: 6164 2e70 7974 6f72 6368 2e6f 7267 2f77  ad.pytorch.org/w
 000154f0: 686c 2f63 7531 3231 2f0d 0a0d 0a20 2020  hl/cu121/....   
 00015500: 2023 204f 7220 7769 7468 2066 6c61 780d   # Or with flax.
 00015510: 0a0d 0a20 2020 2070 6970 3320 696e 7374  ...    pip3 inst
 00015520: 616c 6c20 6467 656e 6572 6174 655b 666c  all dgenerate[fl
-00015530: 6178 5d3d 3d33 2e35 2e30 202d 2d65 7874  ax]==3.5.0 --ext
+00015530: 6178 5d3d 3d33 2e35 2e31 202d 2d65 7874  ax]==3.5.1 --ext
 00015540: 7261 2d69 6e64 6578 2d75 726c 2068 7474  ra-index-url htt
 00015550: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
 00015560: 746f 7263 682e 6f72 672f 7768 6c2f 6375  torch.org/whl/cu
 00015570: 3132 312f 205c 0d0a 2020 2020 2d66 2068  121/ \..    -f h
 00015580: 7474 7073 3a2f 2f73 746f 7261 6765 2e67  ttps://storage.g
 00015590: 6f6f 676c 6561 7069 732e 636f 6d2f 6a61  oogleapis.com/ja
 000155a0: 782d 7265 6c65 6173 6573 2f6a 6178 5f63  x-releases/jax_c
@@ -6007,22 +6007,22 @@
 00017760: 7479 2e0d 0a0d 0a59 6f75 2063 616e 2064  ty.....You can d
 00017770: 6f77 6e6c 6f61 6420 7468 656d 2068 6572  ownload them her
 00017780: 653a 0d0a 0d0a 202a 2060 6d79 2d69 6d61  e:.... * `my-ima
 00017790: 6765 2d73 6565 642e 706e 6720 3c68 7474  ge-seed.png <htt
 000177a0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
 000177b0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f54  sercontent.com/T
 000177c0: 6572 696b 732f 6467 656e 6572 6174 652f  eriks/dgenerate/
-000177d0: 7633 2e35 2e30 2f65 7861 6d70 6c65 732f  v3.5.0/examples/
+000177d0: 7633 2e35 2e31 2f65 7861 6d70 6c65 732f  v3.5.1/examples/
 000177e0: 6d65 6469 612f 646f 672d 6f6e 2d62 656e  media/dog-on-ben
 000177f0: 6368 2e70 6e67 3e60 5f0d 0a20 2a20 606d  ch.png>`_.. * `m
 00017800: 792d 6d61 736b 2d69 6d61 6765 2e70 6e67  y-mask-image.png
 00017810: 203c 6874 7470 733a 2f2f 7261 772e 6769   <https://raw.gi
 00017820: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
 00017830: 636f 6d2f 5465 7269 6b73 2f64 6765 6e65  com/Teriks/dgene
-00017840: 7261 7465 2f76 332e 352e 302f 6578 616d  rate/v3.5.0/exam
+00017840: 7261 7465 2f76 332e 352e 312f 6578 616d  rate/v3.5.1/exam
 00017850: 706c 6573 2f6d 6564 6961 2f64 6f67 2d6f  ples/media/dog-o
 00017860: 6e2d 6265 6e63 682d 6d61 736b 2e70 6e67  n-bench-mask.png
 00017870: 3e60 5f0d 0a0d 0a54 6865 2063 6f6d 6d61  >`_....The comma
 00017880: 6e64 2062 656c 6f77 2067 656e 6572 6174  nd below generat
 00017890: 6573 2061 2063 6174 2073 6974 7469 6e67  es a cat sitting
 000178a0: 206f 6e20 6120 6265 6e63 6820 7769 7468   on a bench with
 000178b0: 2074 6865 2069 6d61 6765 7320 6672 6f6d   the images from
@@ -8723,15 +8723,15 @@
 00022120: 2069 6e66 6572 656e 6365 2073 7465 702e   inference step.
 00022130: 0d0a 0d0a 0d0a 5468 6573 6520 6578 616d  ......These exam
 00022140: 706c 6573 2075 7365 3a20 6076 6572 6d65  ples use: `verme
 00022150: 6572 5f63 616e 6e79 5f65 6467 6564 2e70  er_canny_edged.p
 00022160: 6e67 203c 6874 7470 733a 2f2f 7261 772e  ng <https://raw.
 00022170: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
 00022180: 742e 636f 6d2f 5465 7269 6b73 2f64 6765  t.com/Teriks/dge
-00022190: 6e65 7261 7465 2f76 332e 352e 302f 6578  nerate/v3.5.0/ex
+00022190: 6e65 7261 7465 2f76 332e 352e 312f 6578  nerate/v3.5.1/ex
 000221a0: 616d 706c 6573 2f6d 6564 6961 2f76 6572  amples/media/ver
 000221b0: 6d65 6572 5f63 616e 6e79 5f65 6467 6564  meer_canny_edged
 000221c0: 2e70 6e67 3e60 5f0d 0a0d 0a0d 0a2e 2e20  .png>`_........ 
 000221d0: 636f 6465 2d62 6c6f 636b 3a3a 2062 6173  code-block:: bas
 000221e0: 680d 0a0d 0a20 2020 2023 2054 6f72 6368  h....    # Torch
 000221f0: 2065 7861 6d70 6c65 2c20 7573 6520 2276   example, use "v
 00022200: 6572 6d65 6572 5f63 616e 6e79 5f65 6467  ermeer_canny_edg
@@ -9310,15 +9310,15 @@
 000245d0: 6f72 2067 656e 6572 6174 696f 6e20 7769  or generation wi
 000245e0: 7468 2061 206d 6f64 656c 202b 2061 2043  th a model + a C
 000245f0: 6f6e 7472 6f6c 4e65 742e 0d0a 0d0a 5468  ontrolNet.....Th
 00024600: 6973 2069 6d61 6765 206f 6620 6120 6068  is image of a `h
 00024610: 6f72 7365 203c 6874 7470 733a 2f2f 7261  orse <https://ra
 00024620: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
 00024630: 656e 742e 636f 6d2f 5465 7269 6b73 2f64  ent.com/Teriks/d
-00024640: 6765 6e65 7261 7465 2f76 332e 352e 302f  generate/v3.5.0/
+00024640: 6765 6e65 7261 7465 2f76 332e 352e 312f  generate/v3.5.1/
 00024650: 6578 616d 706c 6573 2f6d 6564 6961 2f68  examples/media/h
 00024660: 6f72 7365 322e 6a70 6567 3e60 5f0d 0a69  orse2.jpeg>`_..i
 00024670: 7320 7573 6564 2069 6e20 7468 6520 6578  s used in the ex
 00024680: 616d 706c 6520 6265 6c6f 7720 7769 7468  ample below with
 00024690: 2061 2043 6f6e 7472 6f6c 4e65 7420 7468   a ControlNet th
 000246a0: 6174 2069 7320 7472 6169 6e65 6420 746f  at is trained to
 000246b0: 2067 656e 6572 6174 6520 696d 6167 6573   generate images
@@ -9550,15 +9550,15 @@
 000254d0: 6520 696d 6167 6520 7573 6564 2069 6e20  e image used in 
 000254e0: 7468 6520 6578 616d 706c 6520 6265 6c6f  the example belo
 000254f0: 7720 6973 2074 6869 7320 606c 6f77 2072  w is this `low r
 00025500: 6573 6f6c 7574 696f 6e20 6361 7420 3c68  esolution cat <h
 00025510: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
 00025520: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
 00025530: 2f54 6572 696b 732f 6467 656e 6572 6174  /Teriks/dgenerat
-00025540: 652f 7633 2e35 2e30 2f65 7861 6d70 6c65  e/v3.5.0/example
+00025540: 652f 7633 2e35 2e31 2f65 7861 6d70 6c65  e/v3.5.1/example
 00025550: 732f 6d65 6469 612f 6c6f 775f 7265 735f  s/media/low_res_
 00025560: 6361 742e 706e 673e 605f 0d0a 0d0a 2e2e  cat.png>`_......
 00025570: 2063 6f64 652d 626c 6f63 6b3a 3a20 6261   code-block:: ba
 00025580: 7368 0d0a 0d0a 2020 2020 2320 5468 6520  sh....    # The 
 00025590: 696d 6167 6520 7072 6f64 7563 6564 2077  image produced w
 000255a0: 6974 6820 7468 6973 206d 6f64 656c 2077  ith this model w
 000255b0: 696c 6c20 6265 0d0a 2020 2020 2320 7477  ill be..    # tw
@@ -10601,15 +10601,15 @@
 00029680: 6f77 696e 6720 6973 2061 2063 6f6e 6669  owing is a confi
 00029690: 6720 6669 6c65 2065 7861 6d70 6c65 2074  g file example t
 000296a0: 6861 7420 636f 7665 7273 2076 6572 7920  hat covers very 
 000296b0: 6261 7369 6320 7379 6e74 6178 2063 6f6e  basic syntax con
 000296c0: 6365 7074 733a 0d0a 0d0a 2e2e 2063 6f64  cepts:...... cod
 000296d0: 652d 626c 6f63 6b3a 3a20 6a69 6e6a 610d  e-block:: jinja.
 000296e0: 0a0d 0a20 2020 2023 2120 6467 656e 6572  ...    #! dgener
-000296f0: 6174 6520 332e 352e 300d 0a0d 0a20 2020  ate 3.5.0....   
+000296f0: 6174 6520 332e 352e 310d 0a0d 0a20 2020  ate 3.5.1....   
 00029700: 2023 2049 6620 6120 6861 7368 2d62 616e   # If a hash-ban
 00029710: 6720 7665 7273 696f 6e20 6973 2070 726f  g version is pro
 00029720: 7669 6465 6420 696e 2074 6865 2066 6f72  vided in the for
 00029730: 6d61 7420 6162 6f76 650d 0a20 2020 2023  mat above..    #
 00029740: 2061 2077 6172 6e69 6e67 2077 696c 6c20   a warning will 
 00029750: 6265 2070 726f 6475 6365 6420 6966 2074  be produced if t
 00029760: 6865 2076 6572 7369 6f6e 2079 6f75 2061  he version you a
@@ -10869,15 +10869,15 @@
 0002a740: 2060 605c 7365 7460 6020 616e 6420 6060   ``\set`` and ``
 0002a750: 5c73 6574 7060 6020 6469 7265 6374 6976  \setp`` directiv
 0002a760: 6520 7769 6c6c 2061 6c73 6f20 6265 206d  e will also be m
 0002a770: 656e 7469 6f6e 6564 2069 6e20 7468 6973  entioned in this
 0002a780: 206f 7574 7075 742e 0d0a 0d0a 2e2e 2063   output....... c
 0002a790: 6f64 652d 626c 6f63 6b3a 3a20 6a69 6e6a  ode-block:: jinj
 0002a7a0: 610d 0a0d 0a20 2020 2023 2120 6467 656e  a....    #! dgen
-0002a7b0: 6572 6174 6520 332e 352e 300d 0a0d 0a20  erate 3.5.0.... 
+0002a7b0: 6572 6174 6520 332e 352e 310d 0a0d 0a20  erate 3.5.1.... 
 0002a7c0: 2020 2023 2049 6e76 6f63 6174 696f 6e20     # Invocation 
 0002a7d0: 7769 6c6c 2070 726f 6365 6564 2061 7320  will proceed as 
 0002a7e0: 6e6f 726d 616c 0d0a 0d0a 2020 2020 7374  normal....    st
 0002a7f0: 6162 696c 6974 7961 692f 7374 6162 6c65  abilityai/stable
 0002a800: 2d64 6966 6675 7369 6f6e 2d32 2d31 202d  -diffusion-2-1 -
 0002a810: 2d70 726f 6d70 7473 2022 6120 6d61 6e20  -prompts "a man 
 0002a820: 7761 6c6b 696e 6720 6f6e 2074 6865 206d  walking on the m
@@ -11780,15 +11780,15 @@
 0002e030: 6573 0d0a 7375 6368 2061 7320 5641 4573  es..such as VAEs
 0002e040: 2065 7463 2e20 6f75 7473 6964 6520 6f66   etc. outside of
 0002e050: 2072 656c 7969 6e67 206f 6e20 7468 6520   relying on the 
 0002e060: 6361 6368 696e 6720 7379 7374 656d 2e0d  caching system..
 0002e070: 0a0d 0a2e 2e20 636f 6465 2d62 6c6f 636b  ..... code-block
 0002e080: 3a3a 206a 696e 6a61 0d0a 0d0a 2020 2020  :: jinja....    
 0002e090: 2321 2064 6765 6e65 7261 7465 2033 2e35  #! dgenerate 3.5
-0002e0a0: 2e30 0d0a 0d0a 2020 2020 2320 596f 7520  .0....    # You 
+0002e0a0: 2e31 0d0a 0d0a 2020 2020 2320 596f 7520  .1....    # You 
 0002e0b0: 6361 6e20 6465 6669 6e65 2079 6f75 7220  can define your 
 0002e0c0: 6f77 6e20 7465 6d70 6c61 7465 2076 6172  own template var
 0002e0d0: 6961 626c 6573 2077 6974 6820 7468 6520  iables with the 
 0002e0e0: 5c73 6574 2064 6972 6563 7469 7665 0d0a  \set directive..
 0002e0f0: 2020 2020 2320 7468 6520 5c73 6574 2064      # the \set d
 0002e100: 6972 6563 7469 7665 2064 6f65 7320 6e6f  irective does no
 0002e110: 7420 646f 2061 6e79 2073 6865 6c6c 2061  t do any shell a
@@ -12267,15 +12267,15 @@
 0002fea0: 2067 6c6f 6220 6d6f 6475 6c65 2c20 796f   glob module, yo
 0002feb0: 7520 6361 6e20 616c 736f 2067 6c6f 6220  u can also glob 
 0002fec0: 6469 7265 6374 6f72 7927 7320 7573 696e  directory's usin
 0002fed0: 6720 7368 656c 6c0d 0a67 6c6f 6262 696e  g shell..globbin
 0002fee0: 672e 0d0a 0d0a 2e2e 2063 6f64 652d 626c  g....... code-bl
 0002fef0: 6f63 6b3a 3a20 6a69 6e6a 610d 0a0d 0a20  ock:: jinja.... 
 0002ff00: 2020 2023 2120 6467 656e 6572 6174 6520     #! dgenerate 
-0002ff10: 332e 352e 300d 0a0d 0a20 2020 2023 2067  3.5.0....    # g
+0002ff10: 332e 352e 310d 0a0d 0a20 2020 2023 2067  3.5.1....    # g
 0002ff20: 6c6f 6262 696e 6720 6361 6e20 6265 2070  lobbing can be p
 0002ff30: 7265 666f 726d 6564 2076 6961 2073 6865  reformed via she
 0002ff40: 6c6c 2065 7870 616e 7369 6f6e 206f 7220  ll expansion or 
 0002ff50: 7573 696e 670d 0a20 2020 2023 2074 6865  using..    # the
 0002ff60: 2067 6c6f 6220 6d6f 6475 6c65 2069 6e73   glob module ins
 0002ff70: 6964 6520 6a69 6e6a 6120 7465 6d70 6c61  ide jinja templa
 0002ff80: 7465 730d 0a0d 0a20 2020 2023 206e 6f74  tes....    # not
@@ -12366,15 +12366,15 @@
 000304d0: 622d 636f 6d6d 616e 6420 6060 696d 6167  b-command ``imag
 000304e0: 652d 7072 6f63 6573 7360 6020 6861 7320  e-process`` has 
 000304f0: 6120 636f 6e66 6967 2064 6972 6563 7469  a config directi
 00030500: 7665 2069 6d70 6c65 6d65 6e74 6174 696f  ve implementatio
 00030510: 6e2e 0d0a 0d0a 0d0a 2e2e 2063 6f64 652d  n......... code-
 00030520: 626c 6f63 6b3a 3a20 6a69 6e6a 610d 0a0d  block:: jinja...
 00030530: 0a20 2020 2023 2120 6467 656e 6572 6174  .    #! dgenerat
-00030540: 6520 332e 352e 300d 0a0d 0a20 2020 2023  e 3.5.0....    #
+00030540: 6520 332e 352e 310d 0a0d 0a20 2020 2023  e 3.5.1....    #
 00030550: 2070 7269 6e74 2074 6865 2068 656c 7020   print the help 
 00030560: 6d65 7373 6167 6520 6f66 202d 2d73 7562  message of --sub
 00030570: 2d63 6f6d 6d61 6e64 2069 6d61 6765 2d70  -command image-p
 00030580: 726f 6365 7373 2c20 7468 6973 2064 6f65  rocess, this doe
 00030590: 730d 0a20 2020 2023 206e 6f74 2063 6175  s..    # not cau
 000305a0: 7365 2074 6865 2063 6f6e 6669 6720 746f  se the config to
 000305b0: 2065 7869 740d 0a0d 0a20 2020 205c 696d   exit....    \im
@@ -12442,15 +12442,15 @@
 00030990: 2069 6d61 6765 2070 726f 6365 7373 696e   image processin
 000309a0: 6720 7574 696c 6974 6965 7320 6173 2073  g utilities as s
 000309b0: 7562 7072 6f63 6573 7365 7320 6672 6f6d  ubprocesses from
 000309c0: 2077 6974 6869 6e20 610d 0a63 6f6e 6669   within a..confi
 000309d0: 6720 7363 7269 7074 2e0d 0a0d 0a0d 0a2e  g script........
 000309e0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 0d0a  . code-block::..
 000309f0: 0d0a 2020 2020 2321 2064 6765 6e65 7261  ..    #! dgenera
-00030a00: 7465 2033 2e35 2e30 0d0a 0d0a 2020 2020  te 3.5.0....    
+00030a00: 7465 2033 2e35 2e31 0d0a 0d0a 2020 2020  te 3.5.1....    
 00030a10: 2320 7275 6e20 6467 656e 6572 6174 6520  # run dgenerate 
 00030a20: 6173 2061 2073 7562 7072 6f63 6573 732c  as a subprocess,
 00030a30: 2072 6561 6420 6120 636f 6e66 6967 0d0a   read a config..
 00030a40: 2020 2020 2320 616e 6420 7365 6e64 2073      # and send s
 00030a50: 7464 6f75 7420 616e 6420 7374 6465 7272  tdout and stderr
 00030a60: 2074 6f20 6120 6669 6c65 0d0a 0d0a 2020   to a file....  
 00030a70: 2020 5c65 7865 6320 6467 656e 6572 6174    \exec dgenerat
@@ -12477,15 +12477,15 @@
 00030bc0: 0d0a 596f 7520 6361 6e20 6578 6974 2061  ..You can exit a
 00030bd0: 2063 6f6e 6669 6720 6561 726c 7920 6966   config early if
 00030be0: 206e 6565 6420 6265 2075 7369 6e67 2074   need be using t
 00030bf0: 6865 2060 605c 6578 6974 6060 2064 6972  he ``\exit`` dir
 00030c00: 6563 7469 7665 0d0a 0d0a 0d0a 2e2e 2063  ective........ c
 00030c10: 6f64 652d 626c 6f63 6b3a 3a20 6a69 6e6a  ode-block:: jinj
 00030c20: 610d 0a0d 0a20 2020 2023 2120 6467 656e  a....    #! dgen
-00030c30: 6572 6174 6520 332e 352e 300d 0a0d 0a20  erate 3.5.0.... 
+00030c30: 6572 6174 6520 332e 352e 310d 0a0d 0a20  erate 3.5.1.... 
 00030c40: 2020 2023 2065 7869 7420 7468 6520 7072     # exit the pr
 00030c50: 6f63 6573 7320 7769 7468 2072 6574 7572  ocess with retur
 00030c60: 6e20 636f 6465 2031 2c20 7768 6963 6820  n code 1, which 
 00030c70: 696e 6469 6361 7465 7320 616e 2065 7272  indicates an err
 00030c80: 6f72 0d0a 0d0a 2020 2020 5c70 7269 6e74  or....    \print
 00030c90: 2022 736f 6d65 2065 7272 6f72 206f 6363   "some error occ
 00030ca0: 7572 7265 6422 0d0a 2020 2020 5c65 7869  urred"..    \exi
@@ -12607,15 +12607,15 @@
 000313e0: 7465 645f 706c 7567 696e 5f6d 6f64 756c  ted_plugin_modul
 000313f0: 6573 2065 6c73 6520 2727 207d 7d0d 0a0d  es else '' }}...
 00031400: 0a43 6f6e 736f 6c65 2055 490d 0a3d 3d3d  .Console UI..===
 00031410: 3d3d 3d3d 3d3d 3d0d 0a0d 0a2e 2e20 696d  =======...... im
 00031420: 6167 653a 3a20 6874 7470 733a 2f2f 7261  age:: https://ra
 00031430: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
 00031440: 656e 742e 636f 6d2f 5465 7269 6b73 2f64  ent.com/Teriks/d
-00031450: 6765 6e65 7261 7465 2f76 332e 352e 302f  generate/v3.5.0/
+00031450: 6765 6e65 7261 7465 2f76 332e 352e 312f  generate/v3.5.1/
 00031460: 6578 616d 706c 6573 2f6d 6564 6961 2f75  examples/media/u
 00031470: 692e 6769 660d 0a20 2020 3a61 6c74 3a20  i.gif..   :alt: 
 00031480: 636f 6e73 6f6c 6520 7569 0d0a 0d0a 596f  console ui....Yo
 00031490: 7520 6361 6e20 6c61 756e 6368 2061 2063  u can launch a c
 000314a0: 726f 7373 2070 6c61 7466 6f72 6d20 546b  ross platform Tk
 000314b0: 696e 7465 7220 4755 4920 666f 7220 696e  inter GUI for in
 000314c0: 7465 7261 6374 696e 6720 7769 7468 2061  teracting with a
@@ -12831,41 +12831,41 @@
 000321e0: 7220 706c 7567 696e 7320 6361 6e20 6265  r plugins can be
 000321f0: 2066 6f75 6e64 0d0a 696e 2074 6865 2060   found..in the `
 00032200: 2277 7269 7469 6e67 5f70 6c75 6769 6e73  "writing_plugins
 00032210: 2f69 6d61 6765 5f70 726f 6365 7373 6f72  /image_processor
 00032220: 2220 3c68 7474 7073 3a2f 2f67 6974 6875  " <https://githu
 00032230: 622e 636f 6d2f 5465 7269 6b73 2f64 6765  b.com/Teriks/dge
 00032240: 6e65 7261 7465 2f74 7265 652f 7633 2e35  nerate/tree/v3.5
-00032250: 2e30 2f65 7861 6d70 6c65 732f 7772 6974  .0/examples/writ
+00032250: 2e31 2f65 7861 6d70 6c65 732f 7772 6974  .1/examples/writ
 00032260: 696e 675f 706c 7567 696e 732f 696d 6167  ing_plugins/imag
 00032270: 655f 7072 6f63 6573 736f 723e 605f 0d0a  e_processor>`_..
 00032280: 666f 6c64 6572 206f 6620 7468 6520 6578  folder of the ex
 00032290: 616d 706c 6573 2066 6f6c 6465 722e 0d0a  amples folder...
 000322a0: 0d0a 5468 6520 736f 7572 6365 2063 6f64  ..The source cod
 000322b0: 6520 666f 7220 7468 6520 6275 696c 7420  e for the built 
 000322c0: 696e 2060 6361 6e6e 7920 3c68 7474 7073  in `canny <https
 000322d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5465  ://github.com/Te
 000322e0: 7269 6b73 2f64 6765 6e65 7261 7465 2f62  riks/dgenerate/b
-000322f0: 6c6f 622f 7633 2e35 2e30 2f64 6765 6e65  lob/v3.5.0/dgene
+000322f0: 6c6f 622f 7633 2e35 2e31 2f64 6765 6e65  lob/v3.5.1/dgene
 00032300: 7261 7465 2f69 6d61 6765 7072 6f63 6573  rate/imageproces
 00032310: 736f 7273 2f63 616e 6e79 2e70 793e 605f  sors/canny.py>`_
 00032320: 2070 726f 6365 7373 6f72 2c0d 0a74 6865   processor,..the
 00032330: 2060 6f70 656e 706f 7365 203c 6874 7470   `openpose <http
 00032340: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
 00032350: 6572 696b 732f 6467 656e 6572 6174 652f  eriks/dgenerate/
-00032360: 626c 6f62 2f76 332e 352e 302f 6467 656e  blob/v3.5.0/dgen
+00032360: 626c 6f62 2f76 332e 352e 312f 6467 656e  blob/v3.5.1/dgen
 00032370: 6572 6174 652f 696d 6167 6570 726f 6365  erate/imageproce
 00032380: 7373 6f72 732f 6f70 656e 706f 7365 2e70  ssors/openpose.p
 00032390: 793e 605f 2070 726f 6365 7373 6f72 2c20  y>`_ processor, 
 000323a0: 616e 6420 7468 6520 7369 6d70 6c65 0d0a  and the simple..
 000323b0: 6070 696c 6c6f 7720 696d 6167 6520 6f70  `pillow image op
 000323c0: 6572 6174 696f 6e73 203c 6874 7470 733a  erations <https:
 000323d0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6572  //github.com/Ter
 000323e0: 696b 732f 6467 656e 6572 6174 652f 626c  iks/dgenerate/bl
-000323f0: 6f62 2f76 332e 352e 302f 6467 656e 6572  ob/v3.5.0/dgener
+000323f0: 6f62 2f76 332e 352e 312f 6467 656e 6572  ob/v3.5.1/dgener
 00032400: 6174 652f 696d 6167 6570 726f 6365 7373  ate/imageprocess
 00032410: 6f72 732f 696d 6167 656f 7073 2e70 793e  ors/imageops.py>
 00032420: 605f 2070 726f 6365 7373 6f72 7320 6361  `_ processors ca
 00032430: 6e20 616c 736f 0d0a 6265 206f 6620 7265  n also..be of re
 00032440: 6665 7265 6e63 6520 6173 2074 6865 7920  ference as they 
 00032450: 6172 6520 7772 6974 7465 6e20 6173 2069  are written as i
 00032460: 6e74 6572 6e61 6c20 696d 6167 6520 7072  nternal image pr
@@ -12875,29 +12875,29 @@
 000324a0: 6720 6469 7265 6374 6976 6573 2063 616e  g directives can
 000324b0: 2062 6520 666f 756e 6420 696e 2074 6865   be found in the
 000324c0: 0d0a 6022 7772 6974 696e 675f 706c 7567  ..`"writing_plug
 000324d0: 696e 732f 636f 6e66 6967 5f64 6972 6563  ins/config_direc
 000324e0: 7469 7665 2220 3c68 7474 7073 3a2f 2f67  tive" <https://g
 000324f0: 6974 6875 622e 636f 6d2f 5465 7269 6b73  ithub.com/Teriks
 00032500: 2f64 6765 6e65 7261 7465 2f74 7265 652f  /dgenerate/tree/
-00032510: 7633 2e35 2e30 2f65 7861 6d70 6c65 732f  v3.5.0/examples/
+00032510: 7633 2e35 2e31 2f65 7861 6d70 6c65 732f  v3.5.1/examples/
 00032520: 7772 6974 696e 675f 706c 7567 696e 732f  writing_plugins/
 00032530: 636f 6e66 6967 5f64 6972 6563 7469 7665  config_directive
 00032540: 3e60 5f20 666f 6c64 6572 0d0a 6f66 2074  >`_ folder..of t
 00032550: 6865 2065 7861 6d70 6c65 7320 666f 6c64  he examples fold
 00032560: 6572 2e20 436f 6e66 6967 2074 656d 706c  er. Config templ
 00032570: 6174 6520 6675 6e63 7469 6f6e 7320 6361  ate functions ca
 00032580: 6e20 616c 736f 2062 6520 696d 706c 656d  n also be implem
 00032590: 656e 7465 6420 6279 2070 6c75 6769 6e73  ented by plugins
 000325a0: 2c0d 0a73 6565 3a20 6022 7772 6974 696e  ,..see: `"writin
 000325b0: 675f 706c 7567 696e 732f 7465 6d70 6c61  g_plugins/templa
 000325c0: 7465 5f66 756e 6374 696f 6e22 203c 6874  te_function" <ht
 000325d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000325e0: 2f54 6572 696b 732f 6467 656e 6572 6174  /Teriks/dgenerat
-000325f0: 652f 7472 6565 2f76 332e 352e 302f 6578  e/tree/v3.5.0/ex
+000325f0: 652f 7472 6565 2f76 332e 352e 312f 6578  e/tree/v3.5.1/ex
 00032600: 616d 706c 6573 2f77 7269 7469 6e67 5f70  amples/writing_p
 00032610: 6c75 6769 6e73 2f74 656d 706c 6174 655f  lugins/template_
 00032620: 6675 6e63 7469 6f6e 3e60 5f0d 0a0d 0a43  function>`_....C
 00032630: 7572 7265 6e74 6c79 2074 6865 206f 6e6c  urrently the onl
 00032640: 7920 696e 7465 726e 616c 2064 6972 6563  y internal direc
 00032650: 7469 7665 2074 6861 7420 6973 2069 6d70  tive that is imp
 00032660: 6c65 6d65 6e74 6564 2061 7320 6120 706c  lemented as a pl
@@ -12905,15 +12905,15 @@
 00032680: 6d61 6765 5f70 726f 6365 7373 6060 2064  mage_process`` d
 00032690: 6972 6563 7469 7665 2c0d 0a77 686f 2773  irective,..who's
 000326a0: 2073 6f75 7263 6520 6669 6c65 2060 6361   source file `ca
 000326b0: 6e20 6265 206c 6f63 6174 6564 2068 6572  n be located her
 000326c0: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
 000326d0: 622e 636f 6d2f 5465 7269 6b73 2f64 6765  b.com/Teriks/dge
 000326e0: 6e65 7261 7465 2f62 6c6f 622f 7633 2e35  nerate/blob/v3.5
-000326f0: 2e30 2f64 6765 6e65 7261 7465 2f62 6174  .0/dgenerate/bat
+000326f0: 2e31 2f64 6765 6e65 7261 7465 2f62 6174  .1/dgenerate/bat
 00032700: 6368 7072 6f63 6573 732f 696d 6167 655f  chprocess/image_
 00032710: 7072 6f63 6573 735f 6469 7265 6374 6976  process_directiv
 00032720: 652e 7079 3e60 5f2c 0d0a 7468 6520 736f  e.py>`_,..the so
 00032730: 7572 6365 2066 696c 6520 666f 7220 7468  urce file for th
 00032740: 6973 2064 6972 6563 7469 7665 2069 7320  is directive is 
 00032750: 7465 7273 6520 6173 206d 6f73 7420 6f66  terse as most of
 00032760: 2060 605c 696d 6167 655f 7072 6f63 6573   ``\image_proces
@@ -12926,15 +12926,15 @@
 000327d0: 6963 6820 6973 2061 6c73 6f20 7573 6564  ich is also used
 000327e0: 2066 6f72 2060 602d 2d73 7562 2d63 6f6d   for ``--sub-com
 000327f0: 6d61 6e64 2069 6d61 6765 2d70 726f 6365  mand image-proce
 00032800: 7373 6060 2069 730d 0a60 6973 2069 6d70  ss`` is..`is imp
 00032810: 6c65 6d65 6e74 6564 2068 6572 6520 3c68  lemented here <h
 00032820: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00032830: 6d2f 5465 7269 6b73 2f64 6765 6e65 7261  m/Teriks/dgenera
-00032840: 7465 2f62 6c6f 622f 7633 2e35 2e30 2f64  te/blob/v3.5.0/d
+00032840: 7465 2f62 6c6f 622f 7633 2e35 2e31 2f64  te/blob/v3.5.1/d
 00032850: 6765 6e65 7261 7465 2f69 6d61 6765 5f70  generate/image_p
 00032860: 726f 6365 7373 3e60 5f2e 0d0a 0d0a 4669  rocess>`_.....Fi
 00032870: 6c65 2043 6163 6865 2043 6f6e 7472 6f6c  le Cache Control
 00032880: 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..==============
 00032890: 3d3d 3d3d 0d0a 0d0a 6467 656e 6572 6174  ====....dgenerat
 000328a0: 6520 7769 6c6c 2063 6163 6865 2060 602d  e will cache ``-
 000328b0: 2d69 6d61 6765 2d73 6565 6473 6060 2066  -image-seeds`` f
```

### Comparing `dgenerate-3.5.0/dgenerate.egg-info/SOURCES.txt` & `dgenerate-3.5.1/dgenerate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/dgenerate.egg-info/requires.txt` & `dgenerate-3.5.1/dgenerate.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/setup.py` & `dgenerate-3.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/tests/unit/concept_uri_parser_test.py` & `dgenerate-3.5.1/tests/unit/concept_uri_parser_test.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/tests/unit/image_seed_parse_test.py` & `dgenerate-3.5.1/tests/unit/image_seed_parse_test.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.5.0/tests/unit/plugin_loading_test.py` & `dgenerate-3.5.1/tests/unit/plugin_loading_test.py`

 * *Files identical despite different names*


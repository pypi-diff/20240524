# Comparing `tmp/whitebox-adversarial-toolbox-0.2.0.tar.gz` & `tmp/whitebox_adversarial_toolbox-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitebox-adversarial-toolbox-0.2.0.tar", last modified: Wed Jun 21 10:10:25 2023, max compression
+gzip compressed data, was "/home/wuhanstudio/Desktop/whitebox-adversarial-toolbox/dist/.tmp-z2dhhgut/whitebox_adversarial_toolbox-0.2.1.tar", last modified: Fri May 24 17:10:38 2024, max compression
```

## Comparing `whitebox-adversarial-toolbox-0.2.0.tar` & `whitebox_adversarial_toolbox-0.2.1.tar`

### file list

```diff
@@ -1,226 +1,195 @@
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1063 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/LICENSE
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       66 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/MANIFEST.in
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4257 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/PKG-INFO
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3219 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/README.md
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.369785 whitebox-adversarial-toolbox-0.2.0/docs/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       19 2023-06-09 20:43:02.000000 whitebox-adversarial-toolbox-0.2.0/docs/CNAME
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.457785 whitebox-adversarial-toolbox-0.2.0/docs/images/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  5657169 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/demo.gif
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   124402 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/what.eps
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  1070518 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/what.png
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    77237 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/what.psd
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   187801 2023-06-09 20:42:51.000000 whitebox-adversarial-toolbox-0.2.0/docs/images/what_logo.psd
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      135 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/index.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    84252 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/search.js
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.465784 whitebox-adversarial-toolbox-0.2.0/docs/what/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    76595 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/_main.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.465784 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.465784 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.465784 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/yolo/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   113391 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/yolo/PCB.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   118219 2023-06-21 10:07:54.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/yolo/TOG.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37957 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection/yolo.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36618 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks/detection.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39361 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/attacks.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37675 2023-06-21 10:07:54.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/cli.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    72344 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/faster_rcnn_demo.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79798 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/mobilenet_ssd_demo.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    75940 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/yolov3_demo.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    92781 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/yolov3_pcb_attack_demo.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    90861 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/yolov3_tog_attack_demo.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    75508 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples/yolov4_demo.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    44796 2023-06-21 10:07:54.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/examples.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/models/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    48520 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/coco.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    82238 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/fiftyone.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   120100 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/open_images.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   121756 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets/voc.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    35417 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/datasets.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.469784 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/frcnn/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241300 2023-06-21 10:07:57.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/frcnn/faster_rcnn.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37384 2023-06-21 10:07:56.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/frcnn.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/ssd/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   190796 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/ssd/mobilenet_v1_ssd.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   194634 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/ssd/mobilenet_v2_ssd_lite.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38242 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/ssd.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    48496 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils/array_utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    58750 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils/box_utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    47979 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils/time_utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36304 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/utils.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    55703 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/yolov3.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    56188 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/yolov3_tiny.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    59301 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/yolov4.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    60668 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo/yolov4_tiny.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39565 2023-06-21 10:07:58.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection/yolo.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38012 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models/detection.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    40578 2023-06-21 10:07:55.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/models.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    69669 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/file.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   110443 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/logger.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43089 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/proj.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    56657 2023-06-21 10:08:00.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils/resize.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38053 2023-06-21 10:07:59.000000 whitebox-adversarial-toolbox-0.2.0/docs/what/utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57945 2023-06-21 10:07:53.000000 whitebox-adversarial-toolbox-0.2.0/docs/what.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.337786 whitebox-adversarial-toolbox-0.2.0/examples/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.473785 whitebox-adversarial-toolbox-0.2.0/examples/.ipynb_checkpoints/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   584485 2022-08-13 20:41:55.000000 whitebox-adversarial-toolbox-0.2.0/examples/.ipynb_checkpoints/MinM-Attack-ICRA-checkpoint.ipynb
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.489784 whitebox-adversarial-toolbox-0.2.0/examples/__pycache__/
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2640 2022-06-30 13:26:59.000000 whitebox-adversarial-toolbox-0.2.0/examples/__pycache__/logger.cpython-37.pyc
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.741782 whitebox-adversarial-toolbox-0.2.0/examples/attack/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       44 2023-06-06 18:51:35.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/.gitignore
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      705 2022-06-20 17:20:47.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/coco_classes.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    63235 2022-08-11 09:36:40.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/demo.jpg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  1185437 2023-06-09 16:34:39.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/demo.mp4
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)  4153472 2023-06-09 15:43:26.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/noise.npy
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4831 2023-06-08 18:41:08.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_evaluation.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3098 2023-06-08 18:41:12.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_image.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3778 2023-06-09 15:44:21.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_universal_video.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4963 2023-06-08 18:43:35.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_universal_voc2012.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5441 2023-06-09 20:43:07.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_video.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4888 2023-06-08 18:44:02.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_tog_attack_evaluation.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3192 2023-06-08 18:45:28.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_tog_attack_image.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5429 2023-06-09 20:43:07.000000 whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_tog_attack_video.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.777782 whitebox-adversarial-toolbox-0.2.0/examples/inference/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2449 2023-06-08 16:19:14.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/faster_rcnn_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1910 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/mobilenet_v1_ssd_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1903 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/mobilenet_v2_ssd_lite_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1909 2023-06-08 16:13:45.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov3_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1985 2023-06-08 16:13:57.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov3_tiny_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1822 2023-06-08 16:14:06.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov4_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1852 2023-06-08 16:14:17.000000 whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov4_tiny_demo.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.845781 whitebox-adversarial-toolbox-0.2.0/examples/train/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       18 2023-06-06 18:52:43.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/.gitignore
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.865781 whitebox-adversarial-toolbox-0.2.0/examples/train/checkpoint/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       71 2023-06-09 16:42:39.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/checkpoint/.gitignore
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4346 2023-06-06 18:50:41.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/faster_rcnn_train.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4172 2023-06-06 18:49:31.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v1_ssd_train.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3372 2022-07-04 16:24:25.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v1_ssd_train_fast.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4199 2023-06-06 18:49:53.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v2_ssd_lite_train.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3390 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/examples/train/mobilenet_v2_ssd_lite_train_fast.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1476 2023-06-21 10:06:15.000000 whitebox-adversarial-toolbox-0.2.0/pyproject.toml
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       38 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/setup.cfg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2007 2023-06-08 20:03:33.000000 whitebox-adversarial-toolbox-0.2.0/setup.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.865781 whitebox-adversarial-toolbox-0.2.0/tests/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.905780 whitebox-adversarial-toolbox-0.2.0/tests/__pycache__/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      163 2023-06-01 14:20:34.000000 whitebox-adversarial-toolbox-0.2.0/tests/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      793 2023-06-01 14:20:36.000000 whitebox-adversarial-toolbox-0.2.0/tests/__pycache__/test_what.cpython-38-pytest-7.3.1.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      161 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/tests/test_what.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.937780 whitebox-adversarial-toolbox-0.2.0/what/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4966 2023-06-21 10:06:21.000000 whitebox-adversarial-toolbox-0.2.0/what/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       31 2023-06-01 14:11:31.000000 whitebox-adversarial-toolbox-0.2.0/what/__main__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4345 2023-06-09 13:01:43.000000 whitebox-adversarial-toolbox-0.2.0/what/_main.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.941780 whitebox-adversarial-toolbox-0.2.0/what/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      634 2023-06-09 14:08:02.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.941780 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      119 2023-06-09 14:09:29.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.941780 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3467 2023-06-09 19:39:34.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/PCB.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3515 2023-06-09 19:39:30.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/TOG.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      399 2023-06-09 14:10:17.000000 whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:24.965780 whitebox-adversarial-toolbox-0.2.0/what/cli/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      190 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/cli/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      308 2023-06-06 15:06:36.000000 whitebox-adversarial-toolbox-0.2.0/what/cli/attack.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1231 2023-06-09 19:57:45.000000 whitebox-adversarial-toolbox-0.2.0/what/cli/example.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2874 2023-06-08 19:49:22.000000 whitebox-adversarial-toolbox-0.2.0/what/cli/model.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/examples/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1562 2023-06-09 14:14:25.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2723 2023-06-08 16:13:19.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/faster_rcnn_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3416 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/mobilenet_ssd_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3027 2023-06-08 15:58:16.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4346 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_pcb_attack_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4226 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_tog_attack_demo.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2999 2023-06-08 19:48:12.000000 whitebox-adversarial-toolbox-0.2.0/what/examples/yolov4_demo.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/models/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1298 2023-06-09 14:03:33.000000 whitebox-adversarial-toolbox-0.2.0/what/models/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/models/detection/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      310 2023-06-09 14:15:42.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2466 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/coco.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2664 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/fiftyone.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4823 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/open_images.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5154 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/voc.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.001779 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      213 2023-06-09 19:28:40.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.033779 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:10:38.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3936 2023-06-09 18:42:48.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/dataset.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9989 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/util.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5592 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/voc_dataset.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10716 2023-06-09 18:48:38.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/faster_rcnn.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.105778 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1188 2023-06-09 18:49:26.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/averagevalue_meter.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3353 2023-06-09 18:49:40.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/confusion_meter.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      544 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/meter.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.129778 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:03:08.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    12038 2023-06-09 18:40:50.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/faster_rcnn_model.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5507 2023-06-09 18:41:40.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/faster_rcnn_vgg16.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7975 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/region_proposal_network.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.145778 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8810 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/bbox_tools.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    16788 2023-06-09 18:41:58.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/creator_tool.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.189777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:30:17.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1712 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/config.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    12665 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/eval_tool.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.197777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      374 2023-06-09 19:29:20.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7597 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/mobilenet_v1_ssd.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7730 2023-06-21 10:05:50.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/mobilenet_v2_ssd_lite.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.205778 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1673 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v1.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6607 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v2.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8233 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v3.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4876 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/squeezenet.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.261777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      624 2023-06-09 18:43:13.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_ssd_config.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3183 2023-06-09 18:43:24.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3607 2023-06-09 18:43:33.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3500 2023-06-09 18:46:50.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5319 2023-06-01 14:09:32.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1966 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/multibox_loss.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3150 2022-06-20 18:22:30.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/predictor.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1773 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/preprocessing.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      617 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/squeezenet_ssd_config.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3817 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7027 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/ssd.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.277777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/transforms/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    13325 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/transforms/transforms.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.277777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10937 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/box_utils.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      535 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/misc.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.281777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      153 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      589 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/array_utils.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1233 2022-06-20 17:46:01.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/box_utils.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      403 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/time_utils.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.281777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      525 2023-06-09 19:29:57.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/__init__.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.281777 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3470 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/utils/yolo_utils.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      896 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov3.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      911 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov3_tiny.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1040 2022-06-09 16:07:06.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov4.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1101 2023-06-06 15:51:49.000000 whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov4_tiny.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/what/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      267 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2397 2023-06-09 20:43:08.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/file.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3522 2022-06-30 13:51:17.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/logger.py
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      477 2022-06-21 20:00:37.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/proj.py
--rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1054 2022-06-21 19:32:15.000000 whitebox-adversarial-toolbox-0.2.0/what/utils/resize.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-21 10:10:25.293777 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4257 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6718 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        1 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       41 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      126 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/requires.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        5 2023-06-21 10:10:24.000000 whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/top_level.txt
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.985530 whitebox_adversarial_toolbox-0.2.1/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1063 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/LICENSE
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       82 2024-05-24 16:42:56.000000 whitebox_adversarial_toolbox-0.2.1/MANIFEST.in
+-rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5167 2024-05-24 17:10:38.981531 whitebox_adversarial_toolbox-0.2.1/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3737 2024-05-24 15:25:00.000000 whitebox_adversarial_toolbox-0.2.1/README.md
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1582 2024-05-24 16:48:51.000000 whitebox_adversarial_toolbox-0.2.1/pyproject.toml
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       38 2024-05-24 17:10:38.985530 whitebox_adversarial_toolbox-0.2.1/setup.cfg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2021 2023-11-26 16:26:28.000000 whitebox_adversarial_toolbox-0.2.1/setup.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4966 2024-05-24 15:27:52.000000 whitebox_adversarial_toolbox-0.2.1/what/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       31 2023-06-01 14:11:31.000000 whitebox_adversarial_toolbox-0.2.1/what/__main__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4345 2023-06-09 13:01:43.000000 whitebox_adversarial_toolbox-0.2.1/what/_main.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      634 2023-06-09 14:08:02.000000 whitebox_adversarial_toolbox-0.2.1/what/attacks/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/attacks/detection/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      119 2024-05-24 15:26:32.000000 whitebox_adversarial_toolbox-0.2.1/what/attacks/detection/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/attacks/detection/yolo/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3521 2023-11-21 17:29:18.000000 whitebox_adversarial_toolbox-0.2.1/what/attacks/detection/yolo/PCB.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3463 2024-01-29 16:50:29.000000 whitebox_adversarial_toolbox-0.2.1/what/attacks/detection/yolo/TOG.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      399 2023-06-09 14:10:17.000000 whitebox_adversarial_toolbox-0.2.1/what/attacks/detection/yolo/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/cli/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      190 2023-06-09 20:43:08.000000 whitebox_adversarial_toolbox-0.2.1/what/cli/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      308 2023-06-06 15:06:36.000000 whitebox_adversarial_toolbox-0.2.1/what/cli/attack.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1388 2023-11-26 16:35:24.000000 whitebox_adversarial_toolbox-0.2.1/what/cli/example.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3899 2023-11-26 17:24:50.000000 whitebox_adversarial_toolbox-0.2.1/what/cli/model.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/examples/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1562 2023-06-09 14:14:25.000000 whitebox_adversarial_toolbox-0.2.1/what/examples/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2770 2023-11-26 17:09:06.000000 whitebox_adversarial_toolbox-0.2.1/what/examples/faster_rcnn_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3451 2023-11-26 17:08:44.000000 whitebox_adversarial_toolbox-0.2.1/what/examples/mobilenet_ssd_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3116 2023-11-26 17:08:35.000000 whitebox_adversarial_toolbox-0.2.1/what/examples/yolov3_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4377 2023-11-26 17:08:28.000000 whitebox_adversarial_toolbox-0.2.1/what/examples/yolov3_pcb_attack_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4237 2024-01-29 16:52:08.000000 whitebox_adversarial_toolbox-0.2.1/what/examples/yolov3_tog_attack_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3088 2023-11-26 17:07:53.000000 whitebox_adversarial_toolbox-0.2.1/what/examples/yolov4_demo.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3464 2023-11-26 17:17:22.000000 whitebox_adversarial_toolbox-0.2.1/what/examples/yolox_demo.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/models/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1710 2023-11-26 17:59:12.000000 whitebox_adversarial_toolbox-0.2.1/what/models/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      381 2023-11-26 17:58:27.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2466 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/coco.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2664 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/fiftyone.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4823 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/open_images.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5154 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/voc.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      213 2023-06-09 19:28:40.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/datasets/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:10:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/datasets/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3936 2023-06-09 18:42:48.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/datasets/dataset.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9989 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/datasets/util.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5592 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/datasets/voc_dataset.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10716 2023-06-09 18:48:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/faster_rcnn.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.969530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/meter/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 20:43:08.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/meter/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1188 2023-06-09 18:49:26.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/meter/averagevalue_meter.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3353 2023-06-09 18:49:40.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/meter/confusion_meter.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      544 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/meter/meter.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:03:08.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    12038 2023-06-09 18:40:50.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/faster_rcnn_model.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5507 2023-06-09 18:41:40.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/faster_rcnn_vgg16.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7975 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/region_proposal_network.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8810 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/utils/bbox_tools.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    16788 2023-06-09 18:41:58.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/utils/creator_tool.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-09 19:30:17.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1712 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/utils/config.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    12665 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/utils/eval_tool.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      374 2023-06-09 19:29:20.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7597 2023-06-21 10:05:50.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/mobilenet_v1_ssd.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7730 2023-06-21 10:05:50.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/mobilenet_v2_ssd_lite.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:09:23.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1673 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/mobilenet_v1.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6607 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/mobilenet_v2.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8233 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/mobilenet_v3.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4876 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/squeezenet.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 16:53:15.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      624 2023-06-09 18:43:13.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_ssd_config.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3183 2023-06-09 18:43:24.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3607 2023-06-09 18:43:33.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3500 2023-06-09 18:46:50.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5319 2023-06-01 14:09:32.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1966 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/multibox_loss.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3150 2022-06-20 18:22:30.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/predictor.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1773 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/preprocessing.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      617 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/squeezenet_ssd_config.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3817 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7027 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/ssd.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/transforms/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:09:12.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/transforms/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    13325 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/transforms/transforms.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10937 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/utils/box_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      535 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/utils/misc.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      153 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      589 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/utils/array_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1342 2023-11-26 17:09:35.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/utils/box_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      403 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/utils/time_utils.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      525 2023-06-09 19:29:57.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       55 2024-05-24 16:48:02.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3470 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/utils/yolo_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      896 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/yolov3.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      911 2022-06-09 16:07:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/yolov3_tiny.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1066 2023-11-21 17:31:36.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/yolov4.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1101 2023-06-06 15:51:49.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/yolov4_tiny.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.973530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      509 2023-11-26 17:16:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.977530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/core/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      152 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/core/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4387 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/core/launch.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    13707 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/core/trainer.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.977530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      354 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7382 2023-11-26 16:25:19.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/data_augment.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1649 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/data_prefetcher.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3671 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/dataloading.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.977530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/datasets/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      325 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/datasets/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6363 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/datasets/coco.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1296 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/datasets/coco_classes.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10878 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/datasets/datasets_wrapper.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9595 2023-11-26 16:27:01.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/datasets/mosaicdetection.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    11968 2023-11-26 16:27:11.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/datasets/voc.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      442 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/datasets/voc_classes.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2854 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/data/samplers.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.977530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/evaluators/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      178 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/evaluators/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    11511 2023-11-26 16:27:25.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/evaluators/coco_evaluator.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5631 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/evaluators/voc_eval.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6586 2023-11-26 16:27:39.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/evaluators/voc_evaluator.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.977530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/exp/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      175 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/exp/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2622 2023-11-26 16:28:31.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/exp/base_exp.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1268 2023-11-26 16:37:30.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/exp/build.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.977530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/exp/default/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1005 2023-11-26 16:42:27.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/exp/default/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    13633 2023-11-26 16:42:57.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/exp/yolox_base.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.977530 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/layers/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      385 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/layers/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5795 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/layers/fast_coco_eval_api.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4462 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/layers/jit_ops.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.981531 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      308 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4266 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/build.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6019 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/darknet.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1677 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/losses.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6092 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/network_blocks.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2476 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/yolo_fpn.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    23963 2023-11-26 16:43:05.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/yolo_head.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3530 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/yolo_pafpn.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1542 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/models/yolox.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1756 2023-11-26 15:30:06.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/predictor.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.981531 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/tools/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      966 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/tools/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.981531 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      452 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2835 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/allreduce_norm.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4712 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/boxes.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1312 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/checkpoint.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      310 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/compat.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5101 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/demo_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8062 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/dist.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2073 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/ema.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    14636 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/logger.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6551 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/lr_scheduler.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3456 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/metric.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5614 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/model_utils.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2675 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/setup_env.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3599 2023-11-06 16:16:38.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/utils/visualize.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1756 2023-11-26 17:16:16.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/yolox_l.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1756 2023-11-26 17:16:22.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/yolox_m.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1756 2023-11-26 17:16:27.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/yolox_s.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1756 2023-11-26 17:14:32.000000 whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolox/yolox_x.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.981531 whitebox_adversarial_toolbox-0.2.1/what/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      267 2023-06-09 20:43:08.000000 whitebox_adversarial_toolbox-0.2.1/what/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2397 2023-06-09 20:43:08.000000 whitebox_adversarial_toolbox-0.2.1/what/utils/file.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3522 2022-06-30 13:51:17.000000 whitebox_adversarial_toolbox-0.2.1/what/utils/logger.py
+-rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      477 2022-06-21 20:00:37.000000 whitebox_adversarial_toolbox-0.2.1/what/utils/proj.py
+-rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1054 2022-06-21 19:32:15.000000 whitebox_adversarial_toolbox-0.2.1/what/utils/resize.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2024-05-24 17:10:38.981531 whitebox_adversarial_toolbox-0.2.1/whitebox_adversarial_toolbox.egg-info/
+-rw-r--r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5167 2024-05-24 17:10:38.000000 whitebox_adversarial_toolbox-0.2.1/whitebox_adversarial_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6657 2024-05-24 17:10:38.000000 whitebox_adversarial_toolbox-0.2.1/whitebox_adversarial_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        1 2024-05-24 17:10:38.000000 whitebox_adversarial_toolbox-0.2.1/whitebox_adversarial_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       41 2024-05-24 17:10:38.000000 whitebox_adversarial_toolbox-0.2.1/whitebox_adversarial_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      167 2024-05-24 17:10:38.000000 whitebox_adversarial_toolbox-0.2.1/whitebox_adversarial_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        5 2024-05-24 17:10:38.000000 whitebox_adversarial_toolbox-0.2.1/whitebox_adversarial_toolbox.egg-info/top_level.txt
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/LICENSE` & `whitebox_adversarial_toolbox-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/PKG-INFO` & `whitebox_adversarial_toolbox-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whitebox-adversarial-toolbox
-Version: 0.2.0
+Version: 0.2.1
 Summary: WHite-box Adversarial Toolbox (WHAT) - Python Library for Deep Learning Security
 Home-page: https://github.com/wuhanstudio/whitebox-adversarial-toolbox
 Author: wuhanstudio
 Author-email: wuhanstudio <wuhanstudios@gmail.com>
 Maintainer: wuhanstudio
 Maintainer-email: wuhanstudio <wuhanstudios@gmail.com>
 License: MIT License
@@ -16,14 +16,29 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.18.0
+Requires-Dist: tqdm
+Requires-Dist: six
+Requires-Dist: setuptools
+Requires-Dist: torch==1.11.0
+Requires-Dist: torchvision
+Requires-Dist: opencv-python
+Requires-Dist: scikit-image
+Requires-Dist: tensorflow==2.4.0
+Requires-Dist: keras==2.4.3
+Requires-Dist: h5py==2.10.0
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: click
+Requires-Dist: progressbar
 
 <img src="https://what.wuhanstudio.uk/images/what.png" width=300px style="float: left;" >
 
 # WHite-box Adversarial Toolbox (WHAT)
 
 <!-- [![CircleCI](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox.svg?style=svg)](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox) -->
 [![Build Status](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox.svg?branch=master)](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox)
@@ -79,23 +94,27 @@
 [x] 3 : YOLOv3 Tiny (    Darknet    )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
 [x] 4 : YOLOv3 Tiny (   MobileNet   )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
 [x] 5 : YOLOv4      (    Darknet    )   Object Detection        YOLOv4 pretrained on MS COCO dataset.
 [x] 6 : YOLOv4 Tiny (    Darknet    )   Object Detection        YOLOv4 Tiny pretrained on MS COCO dataset.
 [x] 7 : SSD         ( MobileNet  v1 )   Object Detection        SSD pretrained on VOC-2012 dataset.
 [x] 8 : SSD         ( MobileNet  v2 )   Object Detection        SSD pretrained on VOC-2012 dataset.
 [x] 9 : FasterRCNN  (     VGG16     )   Object Detection        Faster-RCNN pretrained on VOC-2012 dataset.
+[x] 10 : YOLOX X-Large                  Object Detection        YOLOX-X pretrained on MS COCO dataset.
+[x] 11 : YOLOX Large                    Object Detection        YOLOX-L pretrained on MS COCO dataset.
+[x] 12 : YOLOX Medium                   Object Detection        YOLOX-M pretrained on MS COCO dataset.
+[x] 13 : YOLOX Small                    Object Detection        YOLOX-S pretrained on MS COCO dataset.
 ```
 
 ## A Man-in-the-Middle Hardware Attack
 
 The Universal Adversarial Perturbation (UAP) can be deployed using a Man-in-the-Middle Hardware Attack.
 
 [[ Talk ]](https://minm.wuhanstudio.uk) [[ Video ]](https://youtu.be/OvIpe-R3ZS8) [[ Paper ]](https://arxiv.org/abs/2208.07174) [[ Code ]](https://github.com/wuhanstudio/adversarial-camera)
 
-![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.png)
+[![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.png)](https://github.com/wuhanstudio/adversarial-camera)
 
-![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.jpg)
+[![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.jpg)](https://github.com/wuhanstudio/adversarial-camera)
 
 The Man-in-the-Middle Attack consists of two steps:
 
 - Step 1: [Generating the perturbation](detection/README.md).
 - Step 2: [Deploying the perturbation](hardware/README.md).
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/README.md` & `whitebox_adversarial_toolbox-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -56,23 +56,27 @@
 [x] 3 : YOLOv3 Tiny (    Darknet    )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
 [x] 4 : YOLOv3 Tiny (   MobileNet   )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
 [x] 5 : YOLOv4      (    Darknet    )   Object Detection        YOLOv4 pretrained on MS COCO dataset.
 [x] 6 : YOLOv4 Tiny (    Darknet    )   Object Detection        YOLOv4 Tiny pretrained on MS COCO dataset.
 [x] 7 : SSD         ( MobileNet  v1 )   Object Detection        SSD pretrained on VOC-2012 dataset.
 [x] 8 : SSD         ( MobileNet  v2 )   Object Detection        SSD pretrained on VOC-2012 dataset.
 [x] 9 : FasterRCNN  (     VGG16     )   Object Detection        Faster-RCNN pretrained on VOC-2012 dataset.
+[x] 10 : YOLOX X-Large                  Object Detection        YOLOX-X pretrained on MS COCO dataset.
+[x] 11 : YOLOX Large                    Object Detection        YOLOX-L pretrained on MS COCO dataset.
+[x] 12 : YOLOX Medium                   Object Detection        YOLOX-M pretrained on MS COCO dataset.
+[x] 13 : YOLOX Small                    Object Detection        YOLOX-S pretrained on MS COCO dataset.
 ```
 
 ## A Man-in-the-Middle Hardware Attack
 
 The Universal Adversarial Perturbation (UAP) can be deployed using a Man-in-the-Middle Hardware Attack.
 
 [[ Talk ]](https://minm.wuhanstudio.uk) [[ Video ]](https://youtu.be/OvIpe-R3ZS8) [[ Paper ]](https://arxiv.org/abs/2208.07174) [[ Code ]](https://github.com/wuhanstudio/adversarial-camera)
 
-![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.png)
+[![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.png)](https://github.com/wuhanstudio/adversarial-camera)
 
-![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.jpg)
+[![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.jpg)](https://github.com/wuhanstudio/adversarial-camera)
 
 The Man-in-the-Middle Attack consists of two steps:
 
 - Step 1: [Generating the perturbation](detection/README.md).
 - Step 2: [Deploying the perturbation](hardware/README.md).
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/examples/attack/yolov3_pcb_attack_universal_video.py` & `whitebox_adversarial_toolbox-0.2.1/what/examples/yolov3_tog_attack_demo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,118 @@
 import cv2
-import random
 import numpy as np
 
 from what.models.detection.datasets.coco import COCO_CLASS_NAMES
 from what.models.detection.utils.box_utils import draw_bounding_boxes
-from what.models.detection.yolo.utils.yolo_utils import yolo_process_output, yolov3_anchors
+from what.models.detection.yolo.yolov3 import YOLOV3
+from what.models.detection.yolo.utils.yolo_utils import yolo_process_output, yolov3_anchors, yolov3_tiny_anchors
 
-from what.attacks.detection.yolo.PCB import PCBAttack
+from what.attacks.detection.yolo.TOG import TOGAttack
 from what.utils.resize import bilinear_resize
-import what.utils.logger as log
 
 from what.cli.model import *
 from what.utils.file import get_file
 
-logger = log.get_logger(__name__)
-
 # Target Model
 what_yolov3_model_list = what_model_list[0:4]
 
-if __name__ == '__main__':
-    # Read video frames
-    input_video = []
-
-    cap = cv2.VideoCapture('demo.mp4')
-    success, image = cap.read()
-    while success:
-        input_video.append(image)
-        success,image = cap.read()
-    cap.release()
+def yolov3_tog_attack_demo():
 
-    classes = COCO_CLASS_NAMES 
+    classes = COCO_CLASS_NAMES
 
     colors = np.random.uniform(0, 255, size=(len(classes), 3))
 
-    logger.info(f"Read {len(input_video)} images")
-
-    # random.shuffle(input_video)
-
-    x_train = np.array(input_video[:int(len(input_video) * 0.9)])
-    x_test = np.array(input_video[int(len(input_video) * 0.9):])
-
     # Check what_model_list for all supported models
     index = 3
 
     # Download the model first if not exists
     if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX])):
         get_file(what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX],
                     WHAT_MODEL_PATH,
                     what_yolov3_model_list[index][WHAT_MODEL_URL_INDEX],
                     what_yolov3_model_list[index][WHAT_MODEL_HASH_INDEX])
 
-    # Adversarial Attack
-    model_path = os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX])
-    attack = PCBAttack(model_path, "multi_untargeted", classes)
+    attack = TOGAttack(os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX]), classes)
     attack.fixed = False
 
-    fourcc = cv2.VideoWriter_fourcc(*'XVID')
-
-    out = cv2.VideoWriter('output.avi', fourcc, 20.0, (1280, 720))
-
-    logger.info(f"Train: {len(x_train)}")
-    logger.info(f"Test: {len(x_test)}")
-
-    for n in range(5):
-        for i in range(len(x_train)):
-            logger.info(f"Iteration: {n}, Frame: {i}")
-
-            origin_cv_image = cv2.cvtColor(x_train[i, :, :, :], cv2.COLOR_BGR2RGB)
-
-            # For YOLO, the input pixel values are normalized to [0, 1]
-            input_cv_image = cv2.resize(origin_cv_image, (416, 416))
-
-            input_cv_image = np.array(input_cv_image).astype(np.float32) / 255.0
-
-            # Yolo inference
-            input_cv_image, outs = attack.attack(input_cv_image)
-            boxes, labels, probs = yolo_process_output(outs, yolov3_anchors, len(classes))
-
-            # Draw bounding boxes
-            origin_cv_image = cv2.cvtColor(origin_cv_image, cv2.COLOR_RGB2BGR)
-            origin_cv_image = origin_cv_image.astype(np.float32) / 255.0
-            height, width, _ = origin_cv_image.shape
-            noise = attack.noise
-            noise_r = bilinear_resize(noise[:, :, 0], height, width)
-            noise_g = bilinear_resize(noise[:, :, 1], height, width)
-            noise_b = bilinear_resize(noise[:, :, 2], height, width)
-            noise = np.dstack((noise_r, noise_g, noise_b))
-
-            origin_cv_image = origin_cv_image + noise
-            origin_cv_image = np.clip(origin_cv_image, 0, 1)
-
-            origin_cv_image = (origin_cv_image * 255.0).astype(np.uint8)
-            out_img = draw_bounding_boxes(origin_cv_image, boxes, labels, classes, probs);
-
-            out.write(out_img)
-
-            cv2.namedWindow("result", cv2.WINDOW_NORMAL)
-            cv2.imshow("result", out_img)
-
-            if (cv2.waitKey(1) & 0xFF == ord('q')):
-                break
+    last_outs = None
+    last_boxes = None
+    last_probs = None
+
+    # Initialize the camera
+    video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+
+    while not video.isdigit():
+        video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+
+    # Capture from camera
+    cap = cv2.VideoCapture(int(video))
+    #cap.set(3, 1920)
+    #cap.set(4, 1080)
+
+    n = 0
+
+    while(True): 
+        # Capture the video frame
+        success, origin_cv_image = cap.read()  # read the camera frame
+        if not success:
+            break
+
+        # For YOLO, the input pixel values are normalized to [0, 1]
+        input_cv_image = cv2.resize(origin_cv_image, (416, 416))
+        input_cv_image = np.array(input_cv_image).astype(np.float32) / 255.0
+
+        # Image preprocessing
+        input_cv_image = cv2.cvtColor(input_cv_image, cv2.COLOR_BGR2RGB)
+
+        # Yolo inference
+        input_cv_image, outs = attack.attack(input_cv_image)
+
+        if last_outs is not None:
+            res_list = []
+            for out, last_out in zip(outs, last_outs):
+                out = out.reshape((-1, 5 + len(classes)))
+                last_out = last_out.reshape((-1, 5 + len(classes)))
+
+                res = np.mean(out[:, 4] - last_out[:, 4])
+                res_list.append(res)
+        else:
+            last_outs = outs
+
+        boxes, labels, probs = yolo_process_output(outs, yolov3_tiny_anchors, len(classes))
+
+        if last_boxes is not None:
+            # Eliminate the boxes with low confidence and overlaped boxes
+            if last_boxes.size > 0 and boxes.size > 0:
+                indexes = cv2.dnn.NMSBoxes(np.vstack((boxes, last_boxes)).tolist(), np.hstack((np.array(probs), np.array(last_probs))), 0.5, 0.4)
+                if len(indexes) > 0:
+                    indexes = indexes.flatten()
+
+        last_boxes = np.copy(boxes)
+        last_probs = np.copy(probs)
+
+        # Draw bounding boxes
+        out_img = cv2.cvtColor(origin_cv_image, cv2.COLOR_BGR2RGB)
+        out_img = out_img.astype(np.float32) / 255.0
+        height, width, _ = out_img.shape
+        noise = attack.noise
+
+        # Resize the noise to the same shape as the input image
+        # noise_r = bilinear_resize(noise[:, :, 0], height, width)
+        # noise_g = bilinear_resize(noise[:, :, 1], height, width)
+        # noise_b = bilinear_resize(noise[:, :, 2], height, width)
+        # noise = np.dstack((noise_r, noise_g, noise_b))
+
+        # out_img = out_img + noise
+        out_img = np.clip(out_img, 0, 1)
+
+        out_img = (out_img * 255.0).astype(np.uint8)
+
+        out_img = cv2.cvtColor(out_img, cv2.COLOR_RGB2BGR)
+        if len(boxes) > 0:
+            out_img = draw_bounding_boxes(out_img, boxes, labels, classes, probs);
 
-    out.release()
+        cv2.namedWindow("result", cv2.WINDOW_NORMAL)
+        cv2.imshow("result", out_img)
 
-    logger.info("Perturbation saved to noise.npy")
-    np.save('noise.npy', attack.noise)
+        if (cv2.waitKey(1) & 0xFF == ord('q')):
+            break
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/examples/inference/faster_rcnn_demo.py` & `whitebox_adversarial_toolbox-0.2.1/what/examples/faster_rcnn_demo.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,75 +7,79 @@
 
 from what.cli.model import *
 from what.utils.file import get_file
 
 from what.models.detection.utils.box_utils import draw_bounding_boxes
 from what.models.detection.datasets.voc import VOC_CLASS_NAMES
 
-# Download the model first if not exists
-# Check what_model_list for all available models
-index = 8
-if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, what_model_list[index][WHAT_MODEL_FILE_INDEX])):
-    get_file(what_model_list[index][WHAT_MODEL_FILE_INDEX],
-                WHAT_MODEL_PATH,
-                what_model_list[index][WHAT_MODEL_URL_INDEX],
-                what_model_list[index][WHAT_MODEL_HASH_INDEX])
+def frcnn_inference_demo():
 
-video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
-
-while not video.isdigit():
     video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
 
-# Capture from camera
-cap = cv2.VideoCapture(int(video))
-#cap.set(3, 1920)
-#cap.set(4, 1080)
-
-device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-
-model = FasterRCNN(device=device)
-model.load(os.path.join(WHAT_MODEL_PATH, what_model_list[8][WHAT_MODEL_FILE_INDEX]), map_location=device)
-
-while True:
-    _, orig_image = cap.read()
-    if orig_image is None:
-        continue
-
-    # Image preprocessing
-    input = cv2.cvtColor(orig_image, cv2.COLOR_BGR2RGB)
-    height, width, _ = input.shape
-
-    # NHWC -> NCHW
-    input = np.array(input).transpose((2, 0, 1))
-    input = torch.from_numpy(input)[None]
-
-    # img = read_image('notebooks/demo.jpg', format='NCHW')
-    # input = torch.from_numpy(img)[None]
-    # RGB --> BGR
-    # img = img.transpose((1, 2, 0)).astype(np.uint8)
-
-    inputs, boxes, labels, scores = model.predict(input)
-
-    # (x1, y1, x2, y2) --> (c1, c2, w, h) (0.0, 1.0)
-    boxes = np.array(boxes)[0]
-    box_w  = boxes[:, 2] - boxes[:, 0]
-    box_h = boxes[:, 3] - boxes[:, 1]
-    boxes[:, 0] += box_w / 2
-    boxes[:, 0] /= width
-    boxes[:, 1] += box_h / 2
-    boxes[:, 1] /= height
-    boxes[:, 2] = box_w / width
-    boxes[:, 3] = box_h / height
-
-    output = draw_bounding_boxes(orig_image,
-            boxes,
-            labels[0],
-            VOC_CLASS_NAMES[1:],
-            scores[0])
+    while not video.isdigit():
+        video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+
+    # Capture from camera
+    cap = cv2.VideoCapture(int(video))
+    #cap.set(3, 1920)
+    #cap.set(4, 1080)
+
+    # Download the model first if not exists
+    # Check what_model_list for all available models
+    index = 8
+    if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, what_model_list[index][WHAT_MODEL_FILE_INDEX])):
+        get_file(what_model_list[index][WHAT_MODEL_FILE_INDEX],
+                 WHAT_MODEL_PATH,
+                 what_model_list[index][WHAT_MODEL_URL_INDEX],
+                 what_model_list[index][WHAT_MODEL_HASH_INDEX])
+
+    device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+
+    model = FasterRCNN(device=device)
+
+    model.load(os.path.join(WHAT_MODEL_PATH, what_model_list[index][WHAT_MODEL_FILE_INDEX]), map_location=device)
+
+    while True:
+        _, orig_image = cap.read()
+        if orig_image is None:
+            continue
+
+        # Image preprocessing
+        input_img = cv2.cvtColor(orig_image, cv2.COLOR_BGR2RGB)
+        height, width, _ = input_img.shape
+
+        # NHWC -> NCHW
+        input_img = np.array(input_img).transpose((2, 0, 1))
+        input_img = torch.from_numpy(input_img)[None]
+
+        # img = read_image('notebooks/demo.jpg', format='NCHW')
+        # input_img = torch.from_numpy(img)[None]
+        # RGB --> BGR
+        # img = img.transpose((1, 2, 0)).astype(np.uint8)
+
+        inputs, boxes, labels, scores = model.predict(input_img)
+
+        # (x1, y1, x2, y2) --> (c1, c2, w, h) (0.0, 1.0)
+        boxes = np.array(boxes)[0]
+        box_w  = boxes[:, 2] - boxes[:, 0]
+        box_h = boxes[:, 3] - boxes[:, 1]
+        boxes[:, 0] += box_w / 2
+        boxes[:, 0] /= width
+        boxes[:, 1] += box_h / 2
+        boxes[:, 1] /= height
+        boxes[:, 2] = box_w / width
+        boxes[:, 3] = box_h / height
+
+        if len(boxes) > 0:
+            output = draw_bounding_boxes(orig_image,
+                    boxes,
+                    labels[0],
+                    VOC_CLASS_NAMES[1:],
+                    scores[0])
 
-    cv2.imshow('Faster RCNN', output)
+        cv2.imshow('Faster RCNN Demo', output)
 
-    if cv2.waitKey(1) & 0xFF == ord('q'):
-        break
+        if cv2.waitKey(1) & 0xFF == ord('q'):
+            break
 
-cap.release()
-cv2.destroyAllWindows()
+    cap.release()
+    cv2.destroyAllWindows()
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/examples/inference/mobilenet_v2_ssd_lite_demo.py` & `whitebox_adversarial_toolbox-0.2.1/what/examples/yolov3_demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,89 @@
 import cv2
-import torch
+import os.path
+
+from what.models.detection.datasets.coco import COCO_CLASS_NAMES
+from what.models.detection.utils.box_utils import draw_bounding_boxes
+
+from what.models.detection.yolo.yolov3 import YOLOV3
+from what.models.detection.yolo.yolov3_tiny import YOLOV3_TINY
 
 from what.cli.model import *
+
 from what.utils.file import get_file
 
-from what.models.detection.ssd.mobilenet_v2_ssd_lite import MobileNetV2SSDLite
-from what.models.detection.utils.box_utils import draw_bounding_boxes
-from what.models.detection.datasets.voc import VOC_CLASS_NAMES
+what_yolov3_model_list = what_model_list[0:4]
+
+def yolov3_inference_demo():
 
-device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+    max_len = max([len(x[WHAT_MODEL_NAME_INDEX]) for x in what_yolov3_model_list])
+    for i, model in enumerate(what_yolov3_model_list, start=1):
+        if os.path.isfile(os.path.join(WHAT_MODEL_PATH, model[WHAT_MODEL_FILE_INDEX])):
+            downloaded = 'x'
+        else:
+            downloaded = ' '
+        print('[{}] {} : {:<{w}s}\t{}\t{}'.format(downloaded, i, model[WHAT_MODEL_NAME_INDEX], model[WHAT_MODEL_TYPE_INDEX], model[WHAT_MODEL_DESC_INDEX], w=max_len))
+
+    index = input(f"Please input the model index: ")
+    while not index.isdigit() or int(index) > len(what_yolov3_model_list):
+        index = input(f"Model [{index}] does not exist. Please try again: ")
+
+    index = int(index) - 1
+
+    # Download the model first if not exists
+    WHAT_YOLOV3_MODEL_FILE = what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX]
+    WHAT_YOLOV3_MODEL_URL  = what_yolov3_model_list[index][WHAT_MODEL_URL_INDEX]
+    WHAT_YOLOV3_MODEL_HASH = what_yolov3_model_list[index][WHAT_MODEL_HASH_INDEX]
 
-video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+    if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, WHAT_YOLOV3_MODEL_FILE)):
+        get_file(WHAT_YOLOV3_MODEL_FILE,
+                WHAT_MODEL_PATH,
+                WHAT_YOLOV3_MODEL_URL,
+                WHAT_YOLOV3_MODEL_HASH)
+
+    if index == 0 or index == 1:
+        model = YOLOV3(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, WHAT_YOLOV3_MODEL_FILE))
+
+    if index == 2 or index == 3:
+        model = YOLOV3_TINY(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, WHAT_YOLOV3_MODEL_FILE))
 
-while not video.isdigit():
     video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
 
-# Capture from camera
-cap = cv2.VideoCapture(int(video))
-#cap.set(3, 1920)
-#cap.set(4, 1080)
-
-# Download the model first if not exists
-# Check what_model_list for all available models
-index = 7
-if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, what_model_list[index][WHAT_MODEL_FILE_INDEX])):
-    get_file(what_model_list[index][WHAT_MODEL_FILE_INDEX],
-                WHAT_MODEL_PATH,
-                what_model_list[index][WHAT_MODEL_URL_INDEX],
-                what_model_list[index][WHAT_MODEL_HASH_INDEX])
+    while not video.isdigit():
+        video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+
+    try:
+        # Capture from camera or video
+        if video.isdigit():
+            cap = cv2.VideoCapture(int(video))
+        else:
+            cap = cv2.VideoCapture(video)
+
+        #cap.set(3, 1920)
+        #cap.set(4, 1080)
 
-# Initialize the model
-model = MobileNetV2SSDLite(os.path.join(WHAT_MODEL_PATH, what_model_list[index][WHAT_MODEL_FILE_INDEX]),
-                           VOC_CLASS_NAMES,
-                           is_test=True,
-                           device=device)
+        while True:
+            _, orig_image = cap.read()
+            if orig_image is None:
+                continue
 
-while True:
-    _, orig_image = cap.read()
-    if orig_image is None:
-        continue
+            # Image preprocessing
+            image = cv2.cvtColor(orig_image, cv2.COLOR_BGR2RGB)
 
-    # Image preprocessing
-    image = cv2.cvtColor(orig_image, cv2.COLOR_BGR2RGB)
+            # Run inference
+            images, boxes, labels, probs = model.predict(image)
+            image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
 
-    # Run inference
-    images, boxes, labels, probs = model.predict(image, 10, 0.4)
-    image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
+            # Draw bounding boxes onto the image
+            if len(boxes) > 0:
+                output = draw_bounding_boxes(image, boxes, labels, model.class_names, probs);
 
-    # Draw bounding boxes onto the image
-    output = draw_bounding_boxes(image, boxes, labels, model.class_names, probs);
+            cv2.imshow('YOLOv3 Demo', image)
 
-    cv2.imshow('MobileNetv2 SSD Lite', image)
+            if cv2.waitKey(1) & 0xFF == ord('q'):
+                break
 
-    if cv2.waitKey(1) & 0xFF == ord('q'):
-        break
+        cap.release()
+        cv2.destroyAllWindows()
 
-cap.release()
-cv2.destroyAllWindows()
+    except Exception as e:
+        print(e)
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov3_demo.py` & `whitebox_adversarial_toolbox-0.2.1/what/examples/mobilenet_ssd_demo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,93 @@
 import cv2
-
-from what.models.detection.datasets.coco import COCO_CLASS_NAMES
-from what.models.detection.utils.box_utils import draw_bounding_boxes
-from what.models.detection.yolo.yolov3 import YOLOV3
+import torch
 
 from what.cli.model import *
 from what.utils.file import get_file
 
-what_yolov3_model_list = what_model_list[0:4]
+from what.models.detection.ssd.mobilenet_v1_ssd import MobileNetV1SSD
+from what.models.detection.ssd.mobilenet_v2_ssd_lite import MobileNetV2SSDLite
+from what.models.detection.datasets.voc import VOC_CLASS_NAMES
+
+from what.models.detection.utils.box_utils import draw_bounding_boxes
+
+device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+
+what_ssd_model_list = what_model_list[6:8]
+
+def mobilenet_ssd_inference_demo():
 
-video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+    max_len = max([len(x[WHAT_MODEL_NAME_INDEX]) for x in what_ssd_model_list])
+    for i, model in enumerate(what_ssd_model_list, start=1):
+        if os.path.isfile(os.path.join(WHAT_MODEL_PATH, model[WHAT_MODEL_FILE_INDEX])):
+            downloaded = 'x'
+        else:
+            downloaded = ' '
+        print('[{}] {} : {:<{w}s}\t{}\t{}'.format(downloaded, i, model[WHAT_MODEL_NAME_INDEX], model[WHAT_MODEL_TYPE_INDEX], model[WHAT_MODEL_DESC_INDEX], w=max_len))
+
+    index = input(f"Please input the model index: ")
+    while not index.isdigit() or int(index) > len(what_ssd_model_list):
+        index = input(f"Model [{index}] does not exist. Please try again: ")
+
+    index = int(index) - 1
+
+    # Download the model first if not exists
+    # Check what_model_list for all available models
+    if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, what_ssd_model_list[index][WHAT_MODEL_FILE_INDEX])):
+        get_file(what_ssd_model_list[index][WHAT_MODEL_FILE_INDEX],
+                    WHAT_MODEL_PATH,
+                    what_ssd_model_list[index][WHAT_MODEL_URL_INDEX],
+                    what_ssd_model_list[index][WHAT_MODEL_HASH_INDEX])
+
+    if index == 0:
+        # Initialize the model
+        model = MobileNetV1SSD(os.path.join(WHAT_MODEL_PATH, what_ssd_model_list[index][WHAT_MODEL_FILE_INDEX]),
+                               VOC_CLASS_NAMES,
+                               is_test=True,
+                               device=device)
+
+    if index == 1:
+        # Initialize the model
+        model = MobileNetV2SSDLite(os.path.join(WHAT_MODEL_PATH, what_ssd_model_list[index][WHAT_MODEL_FILE_INDEX]),
+                                   VOC_CLASS_NAMES,
+                                   is_test=True,
+                                   device=device)
 
-while not video.isdigit():
     video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
 
-# Capture from camera
-cap = cv2.VideoCapture(int(video))
-#cap.set(3, 1920)
-#cap.set(4, 1080)
-
-# Check what_model_list for all supported models
-index = 1
-
-# Download the model first if not exists
-if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX])):
-    get_file(what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX],
-                WHAT_MODEL_PATH,
-                what_yolov3_model_list[index][WHAT_MODEL_URL_INDEX],
-                what_yolov3_model_list[index][WHAT_MODEL_HASH_INDEX])
-
-# MobileNet
-model = YOLOV3(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX]))
-
-# You can also use your own model
-# model = YOLOV3(COCO_CLASS_NAMES, "models/yolov3.h5")
-# model = YOLOV3(COCO_CLASS_NAMES, "models/yolov3_mobilenet_lite_416_coco.h5")
-
-while True:
-    _, orig_image = cap.read()
-    if orig_image is None:
-        continue
-
-    # Image preprocessing
-    image = cv2.cvtColor(orig_image, cv2.COLOR_BGR2RGB)
-
-    # Run inference
-    images, boxes, labels, probs = model.predict(image, 10, 0.4)
-    image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
-
-    # Draw bounding boxes onto the image
-    output = draw_bounding_boxes(image, boxes, labels, model.class_names, probs);
+    while not video.isdigit():
+        video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+
+    # Capture from camera
+    cap = cv2.VideoCapture(int(video))
+    #cap.set(3, 1920)
+    #cap.set(4, 1080)
+
+    try:
+        while True:
+            _, orig_image = cap.read()
+            if orig_image is None:
+                continue
+
+            # Image preprocessing
+            image = cv2.cvtColor(orig_image, cv2.COLOR_BGR2RGB)
+
+            # Run inference
+            images, boxes, labels, probs = model.predict(image, 10, 0.4)
+            image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
+
+            # Draw bounding boxes onto the image
+            height, width, _ = image.shape
+
+            if len(boxes) > 0:
+                output = draw_bounding_boxes(image, boxes, labels, model.class_names, probs);
+
+            cv2.imshow('MobileNet SSD Demo', output)
 
-    cv2.imshow('YOLOv3 MobileNet', image)
+            if cv2.waitKey(1) & 0xFF == ord('q'):
+                break
 
-    if cv2.waitKey(1) & 0xFF == ord('q'):
-        break
+        cap.release()
+        cv2.destroyAllWindows()
 
-cap.release()
-cv2.destroyAllWindows()
+    except Exception as e:
+        print(enumerate)
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/examples/inference/yolov3_tiny_demo.py` & `whitebox_adversarial_toolbox-0.2.1/what/examples/yolov4_demo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,89 @@
 import cv2
+import os.path
 
 from what.models.detection.datasets.coco import COCO_CLASS_NAMES
 from what.models.detection.utils.box_utils import draw_bounding_boxes
-from what.models.detection.yolo.yolov3_tiny import YOLOV3_TINY
+
+from what.models.detection.yolo.yolov4 import YOLOV4
+from what.models.detection.yolo.yolov4_tiny import YOLOV4_TINY
 
 from what.cli.model import *
+
 from what.utils.file import get_file
 
-what_yolov3_model_list = what_model_list[0:4]
+what_yolov4_model_list = what_model_list[4:6]
 
-video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+def yolov4_inference_demo():
 
-while not video.isdigit():
-    video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+    max_len = max([len(x[WHAT_MODEL_NAME_INDEX]) for x in what_yolov4_model_list])
+    for i, model in enumerate(what_yolov4_model_list, start=1):
+        if os.path.isfile(os.path.join(WHAT_MODEL_PATH, model[WHAT_MODEL_FILE_INDEX])):
+            downloaded = 'x'
+        else:
+            downloaded = ' '
+        print('[{}] {} : {:<{w}s}\t{}\t{}'.format(downloaded, i, model[WHAT_MODEL_NAME_INDEX], model[WHAT_MODEL_TYPE_INDEX], model[WHAT_MODEL_DESC_INDEX], w=max_len))
+
+    index = input(f"Please input the model index: ")
+    while not index.isdigit() or int(index) > len(what_yolov4_model_list):
+        index = input(f"Model [{index}] does not exist. Please try again: ")
+
+    index = int(index) - 1
+
+    # Download the model first if not exists
+    WHAT_YOLOV4_MODEL_FILE = what_yolov4_model_list[index][WHAT_MODEL_FILE_INDEX]
+    WHAT_YOLOV4_MODEL_URL  = what_yolov4_model_list[index][WHAT_MODEL_URL_INDEX]
+    WHAT_YOLOV4_MODEL_HASH = what_yolov4_model_list[index][WHAT_MODEL_HASH_INDEX]
 
-# Capture from camera
-cap = cv2.VideoCapture(int(video))
-#cap.set(3, 1920)
-#cap.set(4, 1080)
-
-# Check what_model_list for all supported models
-index = 3
-
-# Download the model first if not exists
-if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX])):
-    get_file(what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX],
+    if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, WHAT_YOLOV4_MODEL_FILE)):
+        get_file(WHAT_YOLOV4_MODEL_FILE,
                 WHAT_MODEL_PATH,
-                what_yolov3_model_list[index][WHAT_MODEL_URL_INDEX],
-                what_yolov3_model_list[index][WHAT_MODEL_HASH_INDEX])
+                WHAT_YOLOV4_MODEL_URL,
+                WHAT_YOLOV4_MODEL_HASH)
+
+    if index == 0:
+        model = YOLOV4(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, WHAT_YOLOV4_MODEL_FILE))
+
+    if index == 1:
+        model = YOLOV4_TINY(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, WHAT_YOLOV4_MODEL_FILE))
+
+    video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+
+    while not video.isdigit():
+        video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
+
+    try:
+        # Capture from camera or video
+        if video.isdigit():
+            cap = cv2.VideoCapture(int(video))
+        else:
+            cap = cv2.VideoCapture(video)
 
-# Check what_model_list for all supported models
-model = YOLOV3_TINY(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX]))
+        #cap.set(3, 1920)
+        #cap.set(4, 1080)
 
-# You can also use your own model
-# model = YOLOV3_TINY(COCO_CLASS_NAMES, "models/yolov3-tiny.h5")
-# model = YOLOV3_TINY(COCO_CLASS_NAMES, "models/tiny_yolo3_mobilenet_lite_416_coco.h5")
+        while True:
+            _, orig_image = cap.read()
+            if orig_image is None:
+                continue
 
-while True:
-    _, orig_image = cap.read()
-    if orig_image is None:
-        continue
+            # Image preprocessing
+            image = cv2.cvtColor(orig_image, cv2.COLOR_BGR2RGB)
 
-    # Image preprocessing
-    image = cv2.cvtColor(orig_image, cv2.COLOR_BGR2RGB)
+            # Run inference
+            images, boxes, labels, probs = model.predict(image)
+            image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
 
-    # Run inference
-    images, boxes, labels, probs = model.predict(image, 10, 0.4)
-    image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
+            # Draw bounding boxes onto the image
+            if len(boxes) > 0:
+                output = draw_bounding_boxes(image, boxes, labels, model.class_names, probs);
 
-    # Draw bounding boxes onto the image
-    output = draw_bounding_boxes(image, boxes, labels, model.class_names, probs);
+            cv2.imshow('YOLOv4 Demo', image)
 
-    cv2.imshow('YOLOv3 Tiny MobileNet', image)
+            if cv2.waitKey(1) & 0xFF == ord('q'):
+                break
 
-    if cv2.waitKey(1) & 0xFF == ord('q'):
-        break
+        cap.release()
+        cv2.destroyAllWindows()
 
-cap.release()
-cv2.destroyAllWindows()
+    except Exception as e:
+        print(e)
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/pyproject.toml` & `whitebox_adversarial_toolbox-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
 requires = [
     "numpy>=1.18.0",
     "tqdm",
     "six",
-    "setuptools",
-    "torch",
+    "torch==1.11.0",
     "torchvision",
     "opencv-python",
     "scikit-image",
-    "tensorflow",
+    "tensorflow==2.4.0",
+    "keras==2.4.3",
+    "h5py==2.10.0",
     "matplotlib",
     "click",
     "progressbar",
+    "loguru",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitebox-adversarial-toolbox"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 maintainers = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 description = "WHite-box Adversarial Toolbox (WHAT) - Python Library for Deep Learning Security"
@@ -38,19 +40,21 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "numpy>=1.18.0",
     "tqdm",
     "six",
     "setuptools",
-    "torch",
+    "torch==1.11.0",
     "torchvision",
     "opencv-python",
     "scikit-image",
-    "tensorflow",
+    "tensorflow==2.4.0",
+    "keras==2.4.3",
+    "h5py==2.10.0",
     "matplotlib",
     "pandas",
     "click",
     "progressbar",
 ]
 
 [project.scripts]
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/setup.py` & `whitebox_adversarial_toolbox-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "scikit-image",
     "tensorflow",
     "tensorrt",
     "matplotlib",
     "pandas",
     "click",
     "progressbar",
+    "loguru",
 ]
 
 setuptools.setup(
     name='whitebox-adversarial-toolbox',
     version=get_version(os.path.join("what", "__init__.py")),
     author="wuhanstudio",
     author_email="wuhanstudios@gmail.com",
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/__init__.py` & `whitebox_adversarial_toolbox-0.2.1/what/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,8 +121,8 @@
 
 # Project Imports
 from what import models
 from what import attacks
 from what import utils
 
 # Semantic Version
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/_main.py` & `whitebox_adversarial_toolbox-0.2.1/what/_main.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/attacks/__init__.py` & `whitebox_adversarial_toolbox-0.2.1/what/attacks/__init__.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/PCB.py` & `whitebox_adversarial_toolbox-0.2.1/what/attacks/detection/yolo/PCB.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 import tensorflow as tf
 tf.compat.v1.disable_eager_execution()
 import keras.backend as K
 
 from what.utils.proj import proj_lp
 
 class PCBAttack:
-    def __init__(self, model, attack_type, classes, init="zero", learning_rate = 4 / 255.0, batch = 1, decay = 0.98):
+    def __init__(self, model, attack_type, classes, init="zero", learning_rate = 4 / 255.0, batch = 1, decay = 0.98, custom_objects = None):
         self.classes = len(classes)
         self.epsilon = 1
         self.graph = tf.compat.v1.get_default_graph()
         self.use_filter = False
 
         if init == "uniform":
             self.noise = np.random.uniform( -2 / 255.0, 2 / 255.0, size=(416, 416, 3))
         else:
             self.noise = np.zeros((416, 416, 3))
 
         self.adv_patch_boxes = []
         self.fixed = True
 
-        self.model = load_model(model)
+        self.model = load_model(model, custom_objects=custom_objects)
         self.model.summary()
         self.attack_type = attack_type
 
         self.lr = learning_rate
         self.delta = 0
         self.decay = decay
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/attacks/detection/yolo/TOG.py` & `whitebox_adversarial_toolbox-0.2.1/what/attacks/detection/yolo/TOG.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import tensorflow as tf
 tf.compat.v1.disable_eager_execution()
 import keras.backend as K
 
 from what.utils.proj import proj_lp
 
 class TOGAttack:
-    def __init__(self, model, attack_type, classes, init="zero", decay=0.99):
+    def __init__(self, model, classes, init="zero", decay=1.00):
         self.classes = len(classes)
         self.epsilon = 1
         self.graph = tf.compat.v1.get_default_graph()
         self.use_filter = False
 
         if init == "uniform":
             self.noise = np.random.uniform( -2 / 255.0, 2 / 255.0, size=(416, 416, 3))
@@ -22,15 +22,14 @@
             self.noise = np.zeros((416, 416, 3))
 
         self.adv_patch_boxes = []
         self.fixed = True
 
         self.model = load_model(model)
         self.model.summary()
-        self.attack_type = attack_type
 
         self.delta = 0
         loss = 0
         self.lr = 4 / 255.0
         self.decay = decay
 
         self.c_h = []
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/cli/example.py` & `whitebox_adversarial_toolbox-0.2.1/what/cli/example.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Model Inference
 from what.examples.yolov3_demo import yolov3_inference_demo
 from what.examples.yolov4_demo import yolov4_inference_demo
+from what.examples.yolox_demo import yolox_inference_demo
 from what.examples.faster_rcnn_demo import frcnn_inference_demo
 from what.examples.mobilenet_ssd_demo import mobilenet_ssd_inference_demo
 
 # Adversarial Attack
 from what.examples.yolov3_pcb_attack_demo import yolov3_pcb_attack_demo
 from what.examples.yolov3_tog_attack_demo import yolov3_tog_attack_demo
 
@@ -12,12 +13,13 @@
 WHAT_EXAMPLE_TYPE_INDEX = 1
 WHAT_EXAMPLE_DESC_INDEX = 2
 WHAT_EXAMPLE_FUNC_INDEX = 3
 
 what_example_list = [
     ('    Yolov3 Demo    ', ' Model Inference ', 'Yolov3 Object Detection.', yolov3_inference_demo),
     ('    Yolov4 Demo    ', ' Model Inference ', 'Yolov4 Object Detection.', yolov4_inference_demo),
+    ('     YoloX Demo    ', ' Model Inference ', 'YoloX Object Detection.', yolox_inference_demo),
     ('  FasterRCNN Demo  ', ' Model Inference ', 'FRCNN Object Detection.', frcnn_inference_demo),
     ('MobileNet SSD Demo', ' Model Inference ', 'MobileNet SSD Object Detection.', mobilenet_ssd_inference_demo),
     (' TOG Attack Demo ', 'Adversarial Attack', 'Real-time TOG Attack against Yolov3 Tiny.', yolov3_pcb_attack_demo),
     (' PCB Attack Demo ', 'Adversarial Attack', 'Real-time PCB Attack against Yolov3 Tiny.', yolov3_tog_attack_demo),
 ]
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/cli/model.py` & `whitebox_adversarial_toolbox-0.2.1/what/cli/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,9 +15,13 @@
     ('YOLOv3      (   Mobilenet   )', 'Object Detection', 'YOLOv3 pretrained on MS COCO dataset.', 'yolov3_mobilenet_lite_416_coco.h5', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/yolov3_mobilenet_lite_416_coco.h5', '93eb7be204fca8dd8bafa5146b9795978c9ca6a0ba1d2e2c002f4ed0a1322436'),
     ('YOLOv3 Tiny (    Darknet    )', 'Object Detection', 'YOLOv3 Tiny pretrained on MS COCO dataset.', 'yolov3-tiny.h5', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/yolov3-tiny.h5', '344387880e8ff5e45a313c85f2eeeb2fa4f6d3511ed1e5611aaed438db1f3876'),
     ('YOLOv3 Tiny (   MobileNet   )', 'Object Detection', 'YOLOv3 Tiny pretrained on MS COCO dataset.', 'tiny_yolo3_mobilenet_lite_416_coco.h5', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/tiny_yolo3_mobilenet_lite_416_coco.h5', 'e124316a47915936baa39a157aca58cac86813b2c9bf49646e26c24e80252000'),
     ('YOLOv4      (    Darknet    )', 'Object Detection', 'YOLOv4 pretrained on MS COCO dataset.', 'yolov4.h5', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/yolov4.h5', '54802f99cdbddcb0f31180a55d30be1a80d0b73edaa13e9152829318387512e4'),
     ('YOLOv4 Tiny (    Darknet    )', 'Object Detection', 'YOLOv4 Tiny pretrained on MS COCO dataset.', 'yolov4-tiny.h5', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/yolov4-tiny.h5', '867f54dced382170538a9ca2374e14e778f80d4abd6011652b911b6aca77384e'),
     ('SSD         ( MobileNet  v1 )', 'Object Detection', 'SSD pretrained on VOC-2012 dataset.', 'mobilenet-v1-ssd-mp-0_675.pth', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/mobilenet-v1-ssd-mp-0_675.pth', '58694cafa60456eeab4e81ae50ff49a01c46ab387bfea5200f047143ecd973a9'),
     ('SSD         ( MobileNet  v2 )', 'Object Detection', 'SSD pretrained on VOC-2012 dataset.', 'mobilenet-v2-ssd-lite-mp-0_686.pth', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/mobilenet-v2-ssd-lite-mp-0_686.pth', 'b0d1ac2cdbf3c241ba837f51eeebc565ea37b95b7258e2604506a2f991e398a4'),
-    ('FasterRCNN  (     VGG16     )', 'Object Detection', 'Faster-RCNN pretrained on VOC-2012 dataset.', 'fasterrcnn_12211511_0.701052458187_torchvision_pretrain.pth', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/fasterrcnn_12211511_0.701052458187_torchvision_pretrain.pth', '3fd279284b536da3eac754404779e32e2e9fdd82d8511bbc7f6c50e14f0c69d2')
+    ('FasterRCNN  (     VGG16     )', 'Object Detection', 'Faster-RCNN pretrained on VOC-2012 dataset.', 'fasterrcnn_12211511_0.701052458187_torchvision_pretrain.pth', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/fasterrcnn_12211511_0.701052458187_torchvision_pretrain.pth', '3fd279284b536da3eac754404779e32e2e9fdd82d8511bbc7f6c50e14f0c69d2'),
+    ('YOLOX X-Large                ', 'Object Detection', 'YOLOX-X pretrained on MS COCO dataset.', 'yolox-x.pth', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/yolox_x.pth', '5652330b6ae860043f091b8f550a60c10e1129f416edfdb65c259be6caf355cf'),
+    ('YOLOX Large                  ', 'Object Detection', 'YOLOX-L pretrained on MS COCO dataset.', 'yolox-l.pth', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/yolox_l.pth', '1e6b7fa6240375370b2a8a8eab9066b3cdd43fd1d0bfa8d2027fd3a51def2917'),
+    ('YOLOX Medium                 ', 'Object Detection', 'YOLOX-M pretrained on MS COCO dataset.', 'yolox-m.pth', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/yolox_m.pth', '60076992b32da82951c90cfa7bd6ab70eba9eda243e08b940a396f60ac2d19b6'),
+    ('YOLOX Small                  ', 'Object Detection', 'YOLOX-S pretrained on MS COCO dataset.', 'yolox-s.pth', 'https://wuhanstudio.nyc3.cdn.digitaloceanspaces.com/what/yolox_s.pth', 'f55ded7181e1b0c13285c56e7790b8f0e8f8db590fe4edb37f0b7f345c913a30'),
 ]
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/examples/__init__.py` & `whitebox_adversarial_toolbox-0.2.1/what/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_demo.py` & `whitebox_adversarial_toolbox-0.2.1/what/examples/yolox_demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 import cv2
 import os.path
 
 from what.models.detection.datasets.coco import COCO_CLASS_NAMES
 from what.models.detection.utils.box_utils import draw_bounding_boxes
 
-from what.models.detection.yolo.yolov3 import YOLOV3
-from what.models.detection.yolo.yolov3_tiny import YOLOV3_TINY
+from what.models.detection.yolox.yolox_x import YOLOX_X
+from what.models.detection.yolox.yolox_l import YOLOX_L
+from what.models.detection.yolox.yolox_m import YOLOX_M
+from what.models.detection.yolox.yolox_s import YOLOX_S
 
 from what.cli.model import *
 
 from what.utils.file import get_file
 
-what_yolov3_model_list = what_model_list[0:4]
+what_yolox_model_list = what_model_list[9:13]
 
-def yolov3_inference_demo():
+def yolox_inference_demo():
 
-    max_len = max([len(x[WHAT_MODEL_NAME_INDEX]) for x in what_yolov3_model_list])
-    for i, model in enumerate(what_yolov3_model_list, start=1):
+    max_len = max([len(x[WHAT_MODEL_NAME_INDEX]) for x in what_yolox_model_list])
+    for i, model in enumerate(what_yolox_model_list, start=1):
         if os.path.isfile(os.path.join(WHAT_MODEL_PATH, model[WHAT_MODEL_FILE_INDEX])):
             downloaded = 'x'
         else:
             downloaded = ' '
         print('[{}] {} : {:<{w}s}\t{}\t{}'.format(downloaded, i, model[WHAT_MODEL_NAME_INDEX], model[WHAT_MODEL_TYPE_INDEX], model[WHAT_MODEL_DESC_INDEX], w=max_len))
 
     index = input(f"Please input the model index: ")
-    while not index.isdigit() or int(index) > len(what_yolov3_model_list):
+    while not index.isdigit() or int(index) > len(what_yolox_model_list):
         index = input(f"Model [{index}] does not exist. Please try again: ")
 
     index = int(index) - 1
 
     # Download the model first if not exists
-    if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX])):
-        get_file(what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX],
-                 WHAT_MODEL_PATH,
-                 what_yolov3_model_list[index][WHAT_MODEL_URL_INDEX],
-                 what_yolov3_model_list[index][WHAT_MODEL_HASH_INDEX])
+    WHAT_YOLOX_MODEL_FILE = what_yolox_model_list[index][WHAT_MODEL_FILE_INDEX]
+    WHAT_YOLOX_MODEL_URL  = what_yolox_model_list[index][WHAT_MODEL_URL_INDEX]
+    WHAT_YOLOX_MODEL_HASH = what_yolox_model_list[index][WHAT_MODEL_HASH_INDEX]
+
+    if not os.path.isfile(os.path.join(WHAT_MODEL_PATH, WHAT_YOLOX_MODEL_FILE)):
+        get_file(WHAT_YOLOX_MODEL_FILE,
+                WHAT_MODEL_PATH,
+                WHAT_YOLOX_MODEL_URL,
+                WHAT_YOLOX_MODEL_HASH)
+
+    if index == 0:
+        model = YOLOX_X(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, WHAT_YOLOX_MODEL_FILE))
 
-    if index == 0 or index == 1:
-        model = YOLOV3(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX]))
+    if index == 1:
+        model = YOLOX_L(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, WHAT_YOLOX_MODEL_FILE))
 
-    if index == 2 or index == 3:
-        model = YOLOV3_TINY(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, what_yolov3_model_list[index][WHAT_MODEL_FILE_INDEX]))
+    if index == 2:
+        model = YOLOX_M(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, WHAT_YOLOX_MODEL_FILE))
+
+    if index == 3:
+        model = YOLOX_S(COCO_CLASS_NAMES, os.path.join(WHAT_MODEL_PATH, WHAT_YOLOX_MODEL_FILE))
 
     video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
 
     while not video.isdigit():
         video = input(f"Please input the OpenCV capture device (e.g. 0, 1, 2): ")
 
     try:
@@ -62,23 +74,28 @@
             if orig_image is None:
                 continue
 
             # Image preprocessing
             image = cv2.cvtColor(orig_image, cv2.COLOR_BGR2RGB)
 
             # Run inference
-            images, boxes, labels, probs = model.predict(image, 10, 0.4)
+            images, boxes, labels, probs = model.predict(image)
             image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
 
             # Draw bounding boxes onto the image
-            output = draw_bounding_boxes(image, boxes, labels, model.class_names, probs);
+            if len(boxes) > 0:
+                output = draw_bounding_boxes(image, boxes, labels, model.class_names, probs);
 
-            cv2.imshow('YOLOv3 Demo', image)
+            cv2.imshow('YOLOX Demo', image)
 
             if cv2.waitKey(1) & 0xFF == ord('q'):
                 break
 
         cap.release()
         cv2.destroyAllWindows()
 
     except Exception as e:
         print(e)
+
+
+if __name__ == "__main__":
+    yolox_inference_demo()
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/examples/yolov3_pcb_attack_demo.py` & `whitebox_adversarial_toolbox-0.2.1/what/examples/yolov3_pcb_attack_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
         out_img = (out_img * 255.0).astype(np.uint8)
 
         # for i in range(boxes.shape[0]):
         #     logger.info(f"{classes[labels[i]]}: {probs[i]:.2f}")
 
         out_img = cv2.cvtColor(out_img, cv2.COLOR_RGB2BGR)
-        out_img = draw_bounding_boxes(out_img, boxes, labels, classes, probs);
+        if len(boxes) > 0:
+            out_img = draw_bounding_boxes(out_img, boxes, labels, classes, probs);
 
         cv2.namedWindow("result", cv2.WINDOW_NORMAL)
         cv2.imshow("result", out_img)
 
         if (cv2.waitKey(1) & 0xFF == ord('q')):
             break
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/__init__.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 [ ] 3 : YOLOv3 Tiny (    Darknet    )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
 [ ] 4 : YOLOv3 Tiny (   MobileNet   )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
 [ ] 5 : YOLOv4      (    Darknet    )   Object Detection        YOLOv4 pretrained on MS COCO dataset.
 [ ] 6 : YOLOv4 Tiny (    Darknet    )   Object Detection        YOLOv4 Tiny pretrained on MS COCO dataset.
 [ ] 7 : SSD         ( MobileNet  v1 )   Object Detection        SSD pretrained on VOC-2012 dataset.
 [ ] 8 : SSD         ( MobileNet  v2 )   Object Detection        SSD pretrained on VOC-2012 dataset.
 [ ] 9 : FasterRCNN  (     VGG16     )   Object Detection        Faster-RCNN pretrained on VOC-2012 dataset.
+[x] 10 : YOLOX X-Large                  Object Detection        YOLOX-X pretrained on MS COCO dataset.
+[x] 11 : YOLOX Large                    Object Detection        YOLOX-L pretrained on MS COCO dataset.
+[x] 12 : YOLOX Medium                   Object Detection        YOLOX-M pretrained on MS COCO dataset.
+[x] 13 : YOLOX Small                    Object Detection        YOLOX-S pretrained on MS COCO dataset.
 ```
 
 ## what.models.detection
 
 '''
 
 from what.models import detection
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/coco.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/fiftyone.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/fiftyone.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/open_images.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/open_images.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/datasets/voc.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/dataset.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/util.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/datasets/util.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/datasets/voc_dataset.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/datasets/voc_dataset.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/faster_rcnn.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/averagevalue_meter.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/meter/averagevalue_meter.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/confusion_meter.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/meter/confusion_meter.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/meter/meter.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/meter/meter.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/faster_rcnn_model.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/faster_rcnn_model.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/faster_rcnn_vgg16.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/faster_rcnn_vgg16.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/region_proposal_network.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/region_proposal_network.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/bbox_tools.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/utils/bbox_tools.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/model/utils/creator_tool.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/model/utils/creator_tool.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/config.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/utils/config.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/frcnn/utils/eval_tool.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/frcnn/utils/eval_tool.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/mobilenet_v1_ssd.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/mobilenet_v1_ssd.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/mobilenet_v2_ssd_lite.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/mobilenet_v2_ssd_lite.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v1.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/mobilenet_v1.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v2.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/mobilenet_v3.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/nn/squeezenet.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/nn/squeezenet.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_ssd_config.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_ssd_config.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/multibox_loss.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/multibox_loss.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/predictor.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/predictor.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/preprocessing.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/squeezenet_ssd_config.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/squeezenet_ssd_config.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/ssd/ssd.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/ssd/ssd.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/transforms/transforms.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/box_utils.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/ssd/utils/misc.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/ssd/utils/misc.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/array_utils.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/utils/array_utils.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/utils/box_utils.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/utils/box_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 from .array_utils import to_numpy
 
 def draw_bounding_boxes(image, boxes, labels, class_names, probs):
     if len(boxes) > 0:
         assert(boxes.shape[1] == 4)
         boxes = to_numpy(boxes)
 
-    # (x, y, w, h) --> (x1, y1, x2, y2)
-    height, width, _ = image.shape
-    for box in boxes:
-        box[0] *= width
-        box[1] *= height
-        box[2] *= width 
-        box[3] *= height
-
-        # From center to top left
-        box[0] -= box[2] / 2
-        box[1] -= box[3] / 2
-
-        # From width and height to x2 and y2
-        box[2] += box[0]
-        box[3] += box[1]
-
-    # Draw bounding boxes and labels
-    for i in range(boxes.shape[0]):
-        box = boxes[i]
-        label = f"{class_names[labels[i]]}: {probs[i]:.2f}"
-        # print(label)
-
-        # Draw bounding boxes
-        cv2.rectangle(image, (int(box[0].item()), int(box[1].item())), (int(box[2].item()), int(box[3].item())), (255, 255, 0), 4)
-
-        # Draw labels
-        cv2.putText(image, label,
-                    (int(box[0]+20), int(box[1]+40)),
-                    cv2.FONT_HERSHEY_SIMPLEX,
-                    1,  # font scale
-                    (255, 0, 255),
-                    2)  # line type
+        # (x, y, w, h) --> (x1, y1, x2, y2)
+        height, width, _ = image.shape
+        for box in boxes:
+            box[0] *= width
+            box[1] *= height
+            box[2] *= width 
+            box[3] *= height
+
+            # From center to top left
+            box[0] -= box[2] / 2
+            box[1] -= box[3] / 2
+
+            # From width and height to x2 and y2
+            box[2] += box[0]
+            box[3] += box[1]
+
+        # Draw bounding boxes and labels
+        for i in range(boxes.shape[0]):
+            box = boxes[i]
+            label = f"{class_names[labels[i]]}: {probs[i]:.2f}"
+            # print(label)
+
+            # Draw bounding boxes
+            cv2.rectangle(image, (int(box[0].item()), int(box[1].item())), (int(box[2].item()), int(box[3].item())), (255, 255, 0), 4)
+
+            # Draw labels
+            cv2.putText(image, label,
+                        (int(box[0]+20), int(box[1]+40)),
+                        cv2.FONT_HERSHEY_SIMPLEX,
+                        1,  # font scale
+                        (255, 0, 255),
+                        2)  # line type
+
     return image
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/__init__.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/__init__.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/utils/yolo_utils.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/utils/yolo_utils.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov3.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/yolov3.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov3_tiny.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/yolov3_tiny.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov4.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/yolov4_tiny.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import cv2
 import numpy as np
 
+import tensorflow as tf
 from keras.models import load_model
 import tensorflow.keras.backend as K
 
 from what.models.detection.utils.time_utils import Timer
 
-from .utils.yolo_utils import yolo_process_output, yolov4_anchors
+from .utils.yolo_utils import yolo_process_output, yolov4_tiny_anchors
 
 def mish(x):
     return x * K.tanh(K.softplus(x))
 
-class YOLOV4:
+class YOLOV4_TINY:
     def __init__(self, class_names, model_path):
         self.model = load_model(model_path, custom_objects = {
+            'tf': tf,
             'mish': mish
         })
         self.class_names = class_names
         self.timer = Timer()
 
     def predict(self, image, top_k=-1, prob_threshold=None):
         input_cv_image = cv2.resize(image, (416, 416))
         input_cv_image = np.array(input_cv_image).astype(np.float32) / 255.0
 
         # Yolo inference
         self.timer.start()
         outs = self.model.predict(np.array([input_cv_image]))
         print("FPS: ", int(1.0 / self.timer.end()))
 
-        boxes, class_ids, confidences = yolo_process_output(outs, yolov4_anchors, len(self.class_names))
+        boxes, class_ids, confidences = yolo_process_output(outs, yolov4_tiny_anchors, len(self.class_names))
 
         return input_cv_image, boxes, class_ids, confidences
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/models/detection/yolo/yolov4_tiny.py` & `whitebox_adversarial_toolbox-0.2.1/what/models/detection/yolo/yolov4.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 
 import tensorflow as tf
 from keras.models import load_model
 import tensorflow.keras.backend as K
 
 from what.models.detection.utils.time_utils import Timer
 
-from .utils.yolo_utils import yolo_process_output, yolov4_tiny_anchors
+from .utils.yolo_utils import yolo_process_output, yolov4_anchors
 
-def mish(x):
-    return x * K.tanh(K.softplus(x))
-
-class YOLOV4_TINY:
+class YOLOV4:
     def __init__(self, class_names, model_path):
         self.model = load_model(model_path, custom_objects = {
-            'tf': tf,
-            'mish': mish
+            'mish': lambda x: x * K.tanh(K.softplus(x)),
+            'tf': tf
         })
         self.class_names = class_names
         self.timer = Timer()
 
     def predict(self, image, top_k=-1, prob_threshold=None):
         input_cv_image = cv2.resize(image, (416, 416))
         input_cv_image = np.array(input_cv_image).astype(np.float32) / 255.0
 
         # Yolo inference
         self.timer.start()
         outs = self.model.predict(np.array([input_cv_image]))
         print("FPS: ", int(1.0 / self.timer.end()))
 
-        boxes, class_ids, confidences = yolo_process_output(outs, yolov4_tiny_anchors, len(self.class_names))
+        boxes, class_ids, confidences = yolo_process_output(outs, yolov4_anchors, len(self.class_names))
 
         return input_cv_image, boxes, class_ids, confidences
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/utils/file.py` & `whitebox_adversarial_toolbox-0.2.1/what/utils/file.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/utils/logger.py` & `whitebox_adversarial_toolbox-0.2.1/what/utils/logger.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/what/utils/resize.py` & `whitebox_adversarial_toolbox-0.2.1/what/utils/resize.py`

 * *Files identical despite different names*

### Comparing `whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/PKG-INFO` & `whitebox_adversarial_toolbox-0.2.1/whitebox_adversarial_toolbox.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whitebox-adversarial-toolbox
-Version: 0.2.0
+Version: 0.2.1
 Summary: WHite-box Adversarial Toolbox (WHAT) - Python Library for Deep Learning Security
 Home-page: https://github.com/wuhanstudio/whitebox-adversarial-toolbox
 Author: wuhanstudio
 Author-email: wuhanstudio <wuhanstudios@gmail.com>
 Maintainer: wuhanstudio
 Maintainer-email: wuhanstudio <wuhanstudios@gmail.com>
 License: MIT License
@@ -16,14 +16,29 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.18.0
+Requires-Dist: tqdm
+Requires-Dist: six
+Requires-Dist: setuptools
+Requires-Dist: torch==1.11.0
+Requires-Dist: torchvision
+Requires-Dist: opencv-python
+Requires-Dist: scikit-image
+Requires-Dist: tensorflow==2.4.0
+Requires-Dist: keras==2.4.3
+Requires-Dist: h5py==2.10.0
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: click
+Requires-Dist: progressbar
 
 <img src="https://what.wuhanstudio.uk/images/what.png" width=300px style="float: left;" >
 
 # WHite-box Adversarial Toolbox (WHAT)
 
 <!-- [![CircleCI](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox.svg?style=svg)](https://circleci.com/gh/wuhanstudio/whitebox-adversarial-toolbox) -->
 [![Build Status](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox.svg?branch=master)](https://app.travis-ci.com/wuhanstudio/whitebox-adversarial-toolbox)
@@ -79,23 +94,27 @@
 [x] 3 : YOLOv3 Tiny (    Darknet    )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
 [x] 4 : YOLOv3 Tiny (   MobileNet   )   Object Detection        YOLOv3 Tiny pretrained on MS COCO dataset.
 [x] 5 : YOLOv4      (    Darknet    )   Object Detection        YOLOv4 pretrained on MS COCO dataset.
 [x] 6 : YOLOv4 Tiny (    Darknet    )   Object Detection        YOLOv4 Tiny pretrained on MS COCO dataset.
 [x] 7 : SSD         ( MobileNet  v1 )   Object Detection        SSD pretrained on VOC-2012 dataset.
 [x] 8 : SSD         ( MobileNet  v2 )   Object Detection        SSD pretrained on VOC-2012 dataset.
 [x] 9 : FasterRCNN  (     VGG16     )   Object Detection        Faster-RCNN pretrained on VOC-2012 dataset.
+[x] 10 : YOLOX X-Large                  Object Detection        YOLOX-X pretrained on MS COCO dataset.
+[x] 11 : YOLOX Large                    Object Detection        YOLOX-L pretrained on MS COCO dataset.
+[x] 12 : YOLOX Medium                   Object Detection        YOLOX-M pretrained on MS COCO dataset.
+[x] 13 : YOLOX Small                    Object Detection        YOLOX-S pretrained on MS COCO dataset.
 ```
 
 ## A Man-in-the-Middle Hardware Attack
 
 The Universal Adversarial Perturbation (UAP) can be deployed using a Man-in-the-Middle Hardware Attack.
 
 [[ Talk ]](https://minm.wuhanstudio.uk) [[ Video ]](https://youtu.be/OvIpe-R3ZS8) [[ Paper ]](https://arxiv.org/abs/2208.07174) [[ Code ]](https://github.com/wuhanstudio/adversarial-camera)
 
-![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.png)
+[![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.png)](https://github.com/wuhanstudio/adversarial-camera)
 
-![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.jpg)
+[![](https://github.com/wuhanstudio/adversarial-camera/raw/master/doc/demo.jpg)](https://github.com/wuhanstudio/adversarial-camera)
 
 The Man-in-the-Middle Attack consists of two steps:
 
 - Step 1: [Generating the perturbation](detection/README.md).
 - Step 2: [Deploying the perturbation](hardware/README.md).
```

### Comparing `whitebox-adversarial-toolbox-0.2.0/whitebox_adversarial_toolbox.egg-info/SOURCES.txt` & `whitebox_adversarial_toolbox-0.2.1/whitebox_adversarial_toolbox.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-docs/CNAME
-docs/index.html
-docs/search.js
-docs/what.html
-docs/images/demo.gif
-docs/images/what.eps
-docs/images/what.png
-docs/images/what.psd
-docs/images/what_logo.psd
-docs/what/_main.html
-docs/what/attacks.html
-docs/what/cli.html
-docs/what/examples.html
-docs/what/models.html
-docs/what/utils.html
-docs/what/attacks/detection.html
-docs/what/attacks/detection/yolo.html
-docs/what/attacks/detection/yolo/PCB.html
-docs/what/attacks/detection/yolo/TOG.html
-docs/what/examples/faster_rcnn_demo.html
-docs/what/examples/mobilenet_ssd_demo.html
-docs/what/examples/yolov3_demo.html
-docs/what/examples/yolov3_pcb_attack_demo.html
-docs/what/examples/yolov3_tog_attack_demo.html
-docs/what/examples/yolov4_demo.html
-docs/what/models/detection.html
-docs/what/models/detection/datasets.html
-docs/what/models/detection/frcnn.html
-docs/what/models/detection/ssd.html
-docs/what/models/detection/utils.html
-docs/what/models/detection/yolo.html
-docs/what/models/detection/datasets/coco.html
-docs/what/models/detection/datasets/fiftyone.html
-docs/what/models/detection/datasets/open_images.html
-docs/what/models/detection/datasets/voc.html
-docs/what/models/detection/frcnn/faster_rcnn.html
-docs/what/models/detection/ssd/mobilenet_v1_ssd.html
-docs/what/models/detection/ssd/mobilenet_v2_ssd_lite.html
-docs/what/models/detection/utils/array_utils.html
-docs/what/models/detection/utils/box_utils.html
-docs/what/models/detection/utils/time_utils.html
-docs/what/models/detection/yolo/yolov3.html
-docs/what/models/detection/yolo/yolov3_tiny.html
-docs/what/models/detection/yolo/yolov4.html
-docs/what/models/detection/yolo/yolov4_tiny.html
-docs/what/utils/file.html
-docs/what/utils/logger.html
-docs/what/utils/proj.html
-docs/what/utils/resize.html
-examples/.ipynb_checkpoints/MinM-Attack-ICRA-checkpoint.ipynb
-examples/__pycache__/logger.cpython-37.pyc
-examples/attack/.gitignore
-examples/attack/coco_classes.txt
-examples/attack/demo.jpg
-examples/attack/demo.mp4
-examples/attack/noise.npy
-examples/attack/yolov3_pcb_attack_evaluation.py
-examples/attack/yolov3_pcb_attack_image.py
-examples/attack/yolov3_pcb_attack_universal_video.py
-examples/attack/yolov3_pcb_attack_universal_voc2012.py
-examples/attack/yolov3_pcb_attack_video.py
-examples/attack/yolov3_tog_attack_evaluation.py
-examples/attack/yolov3_tog_attack_image.py
-examples/attack/yolov3_tog_attack_video.py
-examples/inference/faster_rcnn_demo.py
-examples/inference/mobilenet_v1_ssd_demo.py
-examples/inference/mobilenet_v2_ssd_lite_demo.py
-examples/inference/yolov3_demo.py
-examples/inference/yolov3_tiny_demo.py
-examples/inference/yolov4_demo.py
-examples/inference/yolov4_tiny_demo.py
-examples/train/.gitignore
-examples/train/faster_rcnn_train.py
-examples/train/mobilenet_v1_ssd_train.py
-examples/train/mobilenet_v1_ssd_train_fast.py
-examples/train/mobilenet_v2_ssd_lite_train.py
-examples/train/mobilenet_v2_ssd_lite_train_fast.py
-examples/train/checkpoint/.gitignore
-tests/test_what.py
-tests/__pycache__/__init__.cpython-38.pyc
-tests/__pycache__/test_what.cpython-38-pytest-7.3.1.pyc
 what/__init__.py
 what/__main__.py
 what/_main.py
 what/attacks/__init__.py
 what/attacks/detection/__init__.py
 what/attacks/detection/yolo/PCB.py
 what/attacks/detection/yolo/TOG.py
@@ -99,14 +18,15 @@
 what/examples/__init__.py
 what/examples/faster_rcnn_demo.py
 what/examples/mobilenet_ssd_demo.py
 what/examples/yolov3_demo.py
 what/examples/yolov3_pcb_attack_demo.py
 what/examples/yolov3_tog_attack_demo.py
 what/examples/yolov4_demo.py
+what/examples/yolox_demo.py
 what/models/__init__.py
 what/models/detection/__init__.py
 what/models/detection/datasets/__init__.py
 what/models/detection/datasets/coco.py
 what/models/detection/datasets/fiftyone.py
 what/models/detection/datasets/open_images.py
 what/models/detection/datasets/voc.py
@@ -129,42 +49,104 @@
 what/models/detection/frcnn/model/utils/creator_tool.py
 what/models/detection/frcnn/utils/__init__.py
 what/models/detection/frcnn/utils/config.py
 what/models/detection/frcnn/utils/eval_tool.py
 what/models/detection/ssd/__init__.py
 what/models/detection/ssd/mobilenet_v1_ssd.py
 what/models/detection/ssd/mobilenet_v2_ssd_lite.py
+what/models/detection/ssd/nn/__init__.py
 what/models/detection/ssd/nn/mobilenet_v1.py
 what/models/detection/ssd/nn/mobilenet_v2.py
 what/models/detection/ssd/nn/mobilenet_v3.py
 what/models/detection/ssd/nn/squeezenet.py
+what/models/detection/ssd/ssd/__init__.py
 what/models/detection/ssd/ssd/mobilenet_ssd_config.py
 what/models/detection/ssd/ssd/mobilenet_v1_ssd_create.py
 what/models/detection/ssd/ssd/mobilenet_v1_ssd_lite_create.py
 what/models/detection/ssd/ssd/mobilenet_v2_ssd_lite_create.py
 what/models/detection/ssd/ssd/mobilenet_v3_ssd_lite_create.py
 what/models/detection/ssd/ssd/multibox_loss.py
 what/models/detection/ssd/ssd/predictor.py
 what/models/detection/ssd/ssd/preprocessing.py
 what/models/detection/ssd/ssd/squeezenet_ssd_config.py
 what/models/detection/ssd/ssd/squeezenet_ssd_lite_create.py
 what/models/detection/ssd/ssd/ssd.py
+what/models/detection/ssd/transforms/__init__.py
 what/models/detection/ssd/transforms/transforms.py
+what/models/detection/ssd/utils/__init__.py
 what/models/detection/ssd/utils/box_utils.py
 what/models/detection/ssd/utils/misc.py
 what/models/detection/utils/__init__.py
 what/models/detection/utils/array_utils.py
 what/models/detection/utils/box_utils.py
 what/models/detection/utils/time_utils.py
 what/models/detection/yolo/__init__.py
 what/models/detection/yolo/yolov3.py
 what/models/detection/yolo/yolov3_tiny.py
 what/models/detection/yolo/yolov4.py
 what/models/detection/yolo/yolov4_tiny.py
+what/models/detection/yolo/utils/__init__.py
 what/models/detection/yolo/utils/yolo_utils.py
+what/models/detection/yolox/__init__.py
+what/models/detection/yolox/predictor.py
+what/models/detection/yolox/yolox_l.py
+what/models/detection/yolox/yolox_m.py
+what/models/detection/yolox/yolox_s.py
+what/models/detection/yolox/yolox_x.py
+what/models/detection/yolox/core/__init__.py
+what/models/detection/yolox/core/launch.py
+what/models/detection/yolox/core/trainer.py
+what/models/detection/yolox/data/__init__.py
+what/models/detection/yolox/data/data_augment.py
+what/models/detection/yolox/data/data_prefetcher.py
+what/models/detection/yolox/data/dataloading.py
+what/models/detection/yolox/data/samplers.py
+what/models/detection/yolox/data/datasets/__init__.py
+what/models/detection/yolox/data/datasets/coco.py
+what/models/detection/yolox/data/datasets/coco_classes.py
+what/models/detection/yolox/data/datasets/datasets_wrapper.py
+what/models/detection/yolox/data/datasets/mosaicdetection.py
+what/models/detection/yolox/data/datasets/voc.py
+what/models/detection/yolox/data/datasets/voc_classes.py
+what/models/detection/yolox/evaluators/__init__.py
+what/models/detection/yolox/evaluators/coco_evaluator.py
+what/models/detection/yolox/evaluators/voc_eval.py
+what/models/detection/yolox/evaluators/voc_evaluator.py
+what/models/detection/yolox/exp/__init__.py
+what/models/detection/yolox/exp/base_exp.py
+what/models/detection/yolox/exp/build.py
+what/models/detection/yolox/exp/yolox_base.py
+what/models/detection/yolox/exp/default/__init__.py
+what/models/detection/yolox/layers/__init__.py
+what/models/detection/yolox/layers/fast_coco_eval_api.py
+what/models/detection/yolox/layers/jit_ops.py
+what/models/detection/yolox/models/__init__.py
+what/models/detection/yolox/models/build.py
+what/models/detection/yolox/models/darknet.py
+what/models/detection/yolox/models/losses.py
+what/models/detection/yolox/models/network_blocks.py
+what/models/detection/yolox/models/yolo_fpn.py
+what/models/detection/yolox/models/yolo_head.py
+what/models/detection/yolox/models/yolo_pafpn.py
+what/models/detection/yolox/models/yolox.py
+what/models/detection/yolox/tools/__init__.py
+what/models/detection/yolox/utils/__init__.py
+what/models/detection/yolox/utils/allreduce_norm.py
+what/models/detection/yolox/utils/boxes.py
+what/models/detection/yolox/utils/checkpoint.py
+what/models/detection/yolox/utils/compat.py
+what/models/detection/yolox/utils/demo_utils.py
+what/models/detection/yolox/utils/dist.py
+what/models/detection/yolox/utils/ema.py
+what/models/detection/yolox/utils/logger.py
+what/models/detection/yolox/utils/lr_scheduler.py
+what/models/detection/yolox/utils/metric.py
+what/models/detection/yolox/utils/model_utils.py
+what/models/detection/yolox/utils/setup_env.py
+what/models/detection/yolox/utils/visualize.py
 what/utils/__init__.py
 what/utils/file.py
 what/utils/logger.py
 what/utils/proj.py
 what/utils/resize.py
 whitebox_adversarial_toolbox.egg-info/PKG-INFO
 whitebox_adversarial_toolbox.egg-info/SOURCES.txt
```


# Comparing `tmp/acetone_nnet-0.3.tar.gz` & `tmp/acetone_nnet-0.3.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.3.tar", last modified: Wed May 22 06:47:28 2024, max compression
+gzip compressed data, was "acetone_nnet-0.3.1.dev1.tar", last modified: Fri May 24 07:09:14 2024, max compression
```

## Comparing `acetone_nnet-0.3.tar` & `acetone_nnet-0.3.1.dev1.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.298191 acetone_nnet-0.3/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.3/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.3/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.3/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6677 2024-05-22 06:47:28.298191 acetone_nnet-0.3/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.3/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2063 2024-05-22 06:46:57.000000 acetone_nnet-0.3/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-22 06:47:28.298191 acetone_nnet-0.3/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.861186 acetone_nnet-0.3/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.917186 acetone_nnet-0.3/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2012 2024-05-22 06:40:35.000000 acetone_nnet-0.3/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.918186 acetone_nnet-0.3/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.3/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2769 2024-05-15 12:06:29.000000 acetone_nnet-0.3/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.3/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.918186 acetone_nnet-0.3/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4946 2024-05-15 06:49:14.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.920186 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3281 2024-05-16 12:23:11.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4494 2024-05-16 12:12:33.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.921186 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1708 2024-05-15 08:12:43.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6094 2024-05-21 06:29:34.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1713 2024-05-15 08:12:54.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1724 2024-05-15 08:13:23.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1723 2024-05-15 08:13:39.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5069 2024-05-16 14:03:28.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.923186 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5695 2024-05-17 07:53:15.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3541 2024-05-16 11:41:23.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4691 2024-05-15 07:06:26.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2863 2024-05-21 06:24:17.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-05-16 11:34:22.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     9817 2024-05-17 11:33:03.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3045 2024-05-21 06:29:09.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3868 2024-05-21 12:26:03.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.924186 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3507 2024-05-17 06:51:32.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.944187 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6337 2024-05-21 10:14:37.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.945187 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    12359 2024-05-17 06:57:46.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6895 2024-05-16 12:47:31.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5476 2024-05-16 12:48:31.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2359 2024-05-16 08:00:32.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    28977 2024-05-21 15:08:31.000000 acetone_nnet-0.3/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.945187 acetone_nnet-0.3/src/acetone_nnet/debug_tools/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1393 2024-05-22 06:40:28.000000 acetone_nnet-0.3/src/acetone_nnet/debug_tools/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2725 2024-05-21 15:03:01.000000 acetone_nnet-0.3/src/acetone_nnet/debug_tools/debug_keras.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3646 2024-05-21 15:03:05.000000 acetone_nnet-0.3/src/acetone_nnet/debug_tools/debug_onnx.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3542 2024-05-22 06:38:47.000000 acetone_nnet-0.3/src/acetone_nnet/debug_tools/debug_tools.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.946187 acetone_nnet-0.3/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.946187 acetone_nnet-0.3/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18659 2024-05-15 06:28:43.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.946187 acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14558 2024-05-14 15:18:40.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.947187 acetone_nnet-0.3/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5379 2024-05-14 15:15:39.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.947187 acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    32768 2024-05-21 06:37:35.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-14 14:54:21.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.3/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:27.947187 acetone_nnet-0.3/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.3/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.042188 acetone_nnet-0.3/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.3/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.151189 acetone_nnet-0.3/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.198190 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.230190 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      847 2024-05-17 07:06:52.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-17 07:07:01.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      742 2024-05-17 07:07:09.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      724 2024-05-17 07:07:16.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.232190 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.262190 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1350 2024-05-21 10:14:20.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.275190 acetone_nnet-0.3/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.285190 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1030 2024-05-21 10:01:05.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1060 2024-05-21 10:01:00.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.3/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-22 06:47:28.298191 acetone_nnet-0.3/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6677 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7098 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-22 06:47:27.000000 acetone_nnet-0.3/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:14.126356 acetone_nnet-0.3.1.dev1/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.3.1.dev1/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.3.1.dev1/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.3.1.dev1/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-24 07:09:14.126356 acetone_nnet-0.3.1.dev1/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.3.1.dev1/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-23 14:34:50.000000 acetone_nnet-0.3.1.dev1/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-24 07:09:14.126356 acetone_nnet-0.3.1.dev1/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.717352 acetone_nnet-0.3.1.dev1/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.794353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1974 2024-05-23 08:02:27.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.795353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2769 2024-05-15 12:06:29.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.796353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5217 2024-05-23 08:59:21.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.799353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3826 2024-05-23 14:34:41.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6435 2024-05-24 06:37:23.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.800353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2002 2024-05-22 12:46:55.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7194 2024-05-24 07:08:26.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1839 2024-05-22 12:47:14.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1850 2024-05-22 12:47:42.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1851 2024-05-22 12:48:11.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7354 2024-05-23 13:12:01.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.801353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8424 2024-05-24 06:41:54.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4311 2024-05-23 11:45:23.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4833 2024-05-23 09:59:18.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3415 2024-05-23 14:39:38.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6165 2024-05-23 14:35:13.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    11710 2024-05-23 11:53:48.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3570 2024-05-23 09:56:34.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5156 2024-05-23 09:45:10.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.802353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4530 2024-05-24 06:51:11.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.803353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7926 2024-05-24 06:28:37.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.804353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14511 2024-05-23 15:03:15.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6989 2024-05-23 14:48:34.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5660 2024-05-23 14:50:00.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2715 2024-05-23 09:00:44.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    29388 2024-05-23 08:56:40.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.804353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/debug_tools/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1320 2024-05-23 08:01:52.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/debug_tools/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2644 2024-05-23 08:37:10.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/debug_tools/debug_keras.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3602 2024-05-23 08:36:19.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/debug_tools/debug_onnx.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3553 2024-05-22 14:16:11.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/debug_tools/debug_tools.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.804353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.804353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18708 2024-05-22 15:28:07.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.805353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14564 2024-05-22 15:27:00.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.805353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5379 2024-05-14 15:15:39.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.805353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    32928 2024-05-22 15:26:34.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-14 14:54:21.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.806353 acetone_nnet-0.3.1.dev1/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.906354 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:13.996355 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:14.047356 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:14.066356 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      847 2024-05-17 07:06:52.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-17 07:07:01.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      742 2024-05-17 07:07:09.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      724 2024-05-17 07:07:16.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:14.068356 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:14.097356 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1350 2024-05-21 10:14:20.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:14.111356 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:14.121356 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1030 2024-05-21 10:01:05.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1060 2024-05-21 10:01:00.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-24 07:09:14.125356 acetone_nnet-0.3.1.dev1/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-24 07:09:13.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7098 2024-05-24 07:09:13.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-24 07:09:13.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-24 07:09:13.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-24 07:09:13.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-24 07:09:13.000000 acetone_nnet-0.3.1.dev1/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.3/AUTHORS.md` & `acetone_nnet-0.3.1.dev1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/COPYING` & `acetone_nnet-0.3.1.dev1/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/LICENSE` & `acetone_nnet-0.3.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/PKG-INFO` & `acetone_nnet-0.3.1.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.3
+Version: 0.3.1.dev1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.3/README.md` & `acetone_nnet-0.3.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/pyproject.toml` & `acetone_nnet-0.3.1.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.3"
+version = "0.3.1.dev1"
 requires-python = ">=3.10, <3.12"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest,
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip, LeakyReLu
 )
 
 from . import debug_tools
 from .debug_tools import (
-    debug_onnx, run_model_onnx, 
-    debug_keras, run_model_keras, 
+    debug_onnx, debug_keras, 
     compare_result, extract_outputs_c, extract_outputs_python
 )
 
 from .cli_acetone import cli_acetone
 from .cli_compare import cli_compare
 
 __all__ = (
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,15 +71,17 @@
     
     def __init__(self, alpha:float):
         super().__init__()
         self.name = 'leakyrelu'
         self.comment = ' and apply rectifier'
         self.alpha = alpha
 
-        assert self.alpha > 0
+        ### Checking value consistency ###
+        if self.alpha < 0:
+            raise ValueError("Error: alpha value in LeakyRelu (alpha < 0)")
     
     def compute(self, z:np.ndarray):
         temp_tensor = z.flatten()
         for i in range(len(temp_tensor)):
             if(temp_tensor[i]<0):
                 temp_tensor[i] =  self.alpha*temp_tensor[i]
         return temp_tensor.reshape(z.shape)
@@ -154,14 +156,18 @@
 class Clip(ActivationFunctions):
     def __init__(self, max:float|int, min:float|int):
         super().__init__()
         self.name = 'Clip'
         self.comment = ' and apply rectifier'
         self.max = max
         self.min = min
+
+        ### Checking value consistency ###
+        if  self.min > self.max:
+            raise ValueError("Error: min and max values in Clip (min > max)")
     
     def compute(self, z:np.ndarray):
         return np.clip(z,self.min,self.max)
     
     def write_activation_str(self,local_var):
         s = local_var +' > '+str(self.max)+' ? '+ str(self.max) +' : (' + local_var + ' < ' + str(self.min) + ' ? ' + str(self.min) + ' : ' + local_var + ')'
         return s
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,21 +34,26 @@
         self.biases = biases
         self.nb_biases = self.count_elements_array(self.biases)
         self.activation_function = activation_function
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert type(self.biases) == np.ndarray
-        assert isinstance(self.activation_function, ActivationFunctions)
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in AddBias (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in AddBias (size must be int)")
+        if type(self.biases) != np.ndarray:
+            raise TypeError("Error: biases in AddBias (biases must be an numpy array)")
+        if not isinstance(self.activation_function, ActivationFunctions):
+            raise TypeError("Error: activation function type in AddBias (activation function must be a sub-classe of acetone_nnet Activation Function)")
 
         ### Checking value consistency ###
-        assert  len(self.biases.shape) == 1 and self.biases.shape[0] == self.size
+        if len(self.biases.shape) != 1 or self.biases.shape[0] != self.size:
+            raise ValueError("Error:non consistency between the biases shape and the output shape in AddBias ("+str(self.biases.shape[0])+"!="+str(self.size)+")")
     
     #Go through all the indices and do the operation
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str#if the value is in a road or saved eslewhere
 
         mustach_hash = {}
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,80 +19,76 @@
 """
 
 from ..Layer import Layer
 from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
-class BatchNormalization(Layer):
+class Dense(Layer):
 
-    def __init__(self, idx:int, size:int, input_shape:list, epsilon:float|int, scale:np.ndarray, biases:np.ndarray, mean:np.ndarray, var:np.ndarray, activation_function:ActivationFunctions):
+    def __init__(self, idx:int, size:int, weights:np.ndarray, biases:np.ndarray, activation_function:ActivationFunctions):
+        
         super().__init__()
         self.idx = idx
         self.size = size
-        self.name = 'BatchNormalization'
-        self.output_channels = input_shape[1]
-        self.output_height = input_shape[2]
-        self.output_width = input_shape[3]
-        self.epsilon = epsilon
-        self.scale = scale
-        self.mean = mean
-        self.var = var
+        self.name = 'Dense'
+        self.weights = weights
         self.biases = biases
-        self.nb_biases = self.count_elements_array(self.biases)
-
         self.activation_function = activation_function
+        self.local_var = 'dotproduct'
+        
+        self.nb_weights = self.count_elements_array(self.weights)
+        self.nb_biases = self.count_elements_array(self.biases)
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert type(self.output_channels) == int
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
-        assert type(self.epsilon) == float or type(self.epsilon) == int
-        assert type(self.scale) == np.ndarray
-        assert type(self.mean) == np.ndarray 
-        assert type(self.var) == np.ndarray
-        assert type(self.biases) == np.ndarray
-        assert isinstance(self.activation_function, ActivationFunctions)
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in Dense (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in Dense (size must be int)")
+        if type(self.weights) != np.ndarray:
+            raise TypeError("Error: weights in Dense (weights must be an numpy array)")
+        if type(self.biases) != np.ndarray:
+            raise TypeError("Error: biases in Dense (biases must be an numpy array)")
+        if not isinstance(self.activation_function, ActivationFunctions):
+            raise TypeError("Error: activation function type in Dense (activation function must be a sub-classe of acetone_nnet Activation Function)")
 
         ### Checking value consistency ###
-        assert self.size == self.output_channels*self.output_height*self.output_width
-        assert len(self.scale.shape) == 1 and self.scale.shape[0] == self.output_channels
-        assert len(self.mean.shape) == 1 and self.mean.shape[0] == self.output_channels
-        assert len(self.var.shape) == 1 and self.var.shape[0] == self.output_channels
-        assert len(self.biases.shape) == 1 and self.biases.shape[0] == self.output_channels
-
+        if self.size != self.weights.shape[-1]:
+            raise ValueError("Error: non consistency between weight shape and output shape in Dense ("+str(self.size)+"!="+str(self.weights.shape[-1])+")")
+        if self.size != self.biases.shape[0]:
+            raise ValueError("Error: non consistency between biases shape and output shape in Dense ("+str(self.size)+"!="+str(self.weights.shape[-1])+")")
 
+        
     def generate_inference_code_layer(self):
         #Variable indicating under which name the input tensor is
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['comment'] = self.activation_function.comment
         mustach_hash['output_str'] = output_str
-        mustach_hash['path'] = self.path
-        
-        if(self.activation_function.name != 'linear'):
-            mustach_hash['activation_function'] = self.activation_function.write_activation_str('output_'+str(self.path)+'[k + '+str(self.output_height*self.output_width)+'*f]')
+        mustach_hash['road'] = self.path
+        mustach_hash['size'] = self.size
+
+        mustach_hash['activation_function'] = self.activation_function.write_activation_str(self.local_var)
 
-        mustach_hash['input_channels'] = self.output_channels
-        mustach_hash['channel_size'] = self.output_height*self.output_width
-        mustach_hash['epsilon'] = self.epsilon
+        mustach_hash['prev_size'] = self.previous_layer[0].size
 
-        with open(self.template_path+'layers/template_BatchNormalization.c.tpl','r') as template_file:
+        if(self.fused_layer):
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str(self.local_var,self.idx,'i')
+
+            if(self.activation_function.name == 'linear'):
+                mustach_hash['linear'] = True
+        
+        with open(self.template_path+'layers/template_Dense.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def forward_path_layer(self, input:np.ndarray):
-        input = np.reshape(input, (self.output_channels, self.output_height, self.output_width))
-        output = []
-        for i in range(self.output_channels):
-            output.append((input[i] - self.mean[i])/np.sqrt(self.var[i] + self.epsilon)*self.scale[i] + self.biases[i])
-        return np.array(output)
+        input = input.reshape(self.previous_layer[0].size)
+        return self.activation_function.compute(np.dot(input, self.weights) + self.biases)
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,27 +17,27 @@
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
 import numpy as np
 
-#Addition of several tensor
-class Add(Broadcast):
+#Subtraction of several tensors
+class Subtract(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Add'
-        self.specific_operator = ' + '
+        self.name = 'Subtract'
+        self.specific_operator = ' - '
     
     def forward_path_layer(self, inputs:np.ndarray):
         if(self.constant is None):
-            constant = 0
+            constant = np.zeros(1)
         else: 
             constant = self.constant
         if(len(self.previous_layer) > 1):
-            output = inputs[0]
-            for input in inputs[1:]:
-                output += input
+            output = np.zeros(self.input_shapes[0][1:])
+            for i in range(len(self.input_shapes)):
+                output -= np.reshape(inputs[i],self.input_shapes[i][1:])
         else:
-            output = inputs
-        return self.activation_function.compute(output+constant)
+            output = np.reshape(inputs,self.input_shapes[0][1:])
+        return self.activation_function.compute(output-constant)
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,31 +45,38 @@
         self.constant = constant
         if(constant is not None):
             self.constant_size = self.count_elements_array(self.constant)
         
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert type(self.output_channels) == int
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
-        assert isinstance(self.activation_function, ActivationFunctions)
-        assert type(self.constant) == np.ndarray or self.constant == None
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in Broadcast (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in Broadcast (size must be int)")
+        if type(self.output_channels) != int:
+            raise TypeError("Error: output channels type in Broadcast (must be int)")
+        if type(self.output_height) != int:
+            raise TypeError("Error: output height type in Broadcast (must be int)")
+        if type(self.output_width) != int:
+            raise TypeError("Error: output width type in Broadcast (must be int)")
+        if not isinstance(self.activation_function, ActivationFunctions):
+            raise TypeError("Error: activation function type in Broadcast (activation function must be a sub-classe of acetone_nnet Activation Function)")
+        if type(self.constant) != np.ndarray and self.constant != None:
+            raise TypeError("Error: constant type in Broadcast")
 
         ### Checking value consistency ###
-        assert self.size == self.output_channels*self.output_height*self.output_width
-        assert all(shape[1] == 1 or shape[1]==self.output_channels for shape in self.input_shapes)
-        assert all(shape[2] == 1 or shape[2]==self.output_height for shape in self.input_shapes)
-        assert all(shape[3] == 1 or shape[3]==self.output_width for shape in self.input_shapes)
-        assert self.output_channels == np.max(self.input_shapes[:,1])
-        assert self.output_height == np.max(self.input_shapes[:,2])
-        assert self.output_width == np.max(self.input_shapes[:,3])
-
+        if self.size != self.output_channels*self.output_height*self.output_width:
+            raise ValueError("Error: size value in Broadcast ("+str(self.size)+"!="+str(self.output_channels*self.output_height*self.output_width)+")")
+        if (self.output_channels,self.output_height,self.output_width) != (np.max(self.input_shapes[:,1]),np.max(self.input_shapes[:,2]),np.max(self.input_shapes[:,3])):
+            raise ValueError("Error: non consistency between inputs shape and output shape in Broadcast ("+str((np.max(self.input_shapes[:,1]),np.max(self.input_shapes[:,2]),np.max(self.input_shapes[:,3])))+"!="+str((self.output_channels,self.output_height,self.output_width))+")")
+        for shape in self.input_shapes:
+            if (shape[1] != 1 and shape[1]!=self.output_channels) or (shape[2] != 1 and shape[2]!=self.output_height) or (shape[3] != 1 and shape[3]!=self.output_width):
+                raise ValueError("Error: input shape in Broadcast not broadcastable to shape " + str((self.output_channels,self.output_height,self.output_width)))
+        
     #Go through all the indices and do the operation
     def generate_inference_code_layer(self):
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.name = 'Divide'
         self.specific_operator = '/'
     
     def forward_path_layer(self, inputs:np.ndarray):
         if(self.constant is None):
-            constant = 1
+            constant = np.ones(1)
         else: 
             constant = self.constant
         if(len(self.previous_layer) > 1):
-            output = inputs[0]
-            for input in inputs[1:]:
-                output /= input
+            output = np.ones(self.input_shapes[0][1:])
+            for i in range(len(self.input_shapes)):
+                output /= np.reshape(inputs[i],self.input_shapes[i][1:])
         else:
-            output = inputs
+            output = np.reshape(inputs,self.input_shapes[0][1:])
         return self.activation_function.compute(output/constant)
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.name = 'Multiply'
         self.specific_operator = '*'
     
     def forward_path_layer(self, inputs:np.ndarray):
         if(self.constant is None):
-            constant = 1
+            constant = np.ones(1)
         else: 
             constant = self.constant
         if(len(self.previous_layer) > 1):
-            output = inputs[0]
-            for input in inputs[1:]:
-                output *= input
+            output = np.ones(self.input_shapes[0][1:])
+            for i in range(len(self.input_shapes)):
+                output *= np.reshape(inputs[i],self.input_shapes[i][1:])
         else:
-            output = inputs
-        return self.activation_function.compute(constant*output)
+            output = np.reshape(inputs,self.input_shapes[0][1:])
+        return self.activation_function.compute(output*constant)
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,30 +14,31 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from .Broadcast import Broadcast
+from .Pooling2D import Pooling2D
+
 import numpy as np
 
-#Subtraction of several tensors
-class Subtract(Broadcast):
-    
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.name = 'Subtract'
-        self.specific_operator = ' - '
+class MaxPooling2D(Pooling2D):
+    def __init__(self, **kwds):
+        super().__init__(**kwds)
+        
+        self.name = 'MaxPooling2D'
+        self.pooling_function = np.amax
+        self.local_var = 'max'
+        self.output_var = self.local_var
+
+    def update_local_vars(self):
+        
+        s = self.local_var +' = -INFINITY;\n'
+
+        return s
+
+    def specific_function(self, index:str, input_of_layer:str):
+        s = 'if ('+input_of_layer+'['+index+'] > '+self.local_var+')\n'
+        s += '                                '+self.local_var+' = '+input_of_layer+'['+index+'];\n'
     
-    def forward_path_layer(self, inputs:np.ndarray):
-        if(self.constant is None):
-            constant = 0
-        else: 
-            constant = self.constant
-        if(len(self.previous_layer) > 1):
-            output = inputs[0]
-            for input in inputs[1:]:
-                output -= input
-        else:
-            output = inputs
-        return self.activation_function.compute(output-constant)
+        return s
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,96 +19,107 @@
 """
 
 from ..Layer import Layer
 from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
-#Concatenate two tensor alongside a given axis
-#attribut: axis alongside of which the concatenation will be done
-#input: a list of tensor to concatenate
-#output: the concatenated tensor 
-class Concatenate(Layer):
-    def __init__(self, idx:int, size:int, axis:int, input_shapes:list, output_shape:list, activation_function:ActivationFunctions):
+#extract a list of subtensor from a given tensor
+#attribut: axis alongside of which the submatrix will be extracted (if the desired submatrix must have the height, width or channels of the parent tensor)
+#input: a tensor
+#output: a list of tensor
+class Gather(Layer):
+    
+    def __init__(self, idx:int, size:int, axis:int,  indices:np.ndarray, input_shape:list, output_shape:list, activation_function:ActivationFunctions):
+        
         super().__init__()
         self.idx = idx
         self.size = size
-        self.input_shapes = input_shapes
-        self.name = 'Concatenate'
+        self.name = 'Gather'
+        self.indices = indices
         self.axis = axis
+        self.output_channels = input_shape[1]
+        self.input_height = input_shape[2]
+        self.input_width = input_shape[3]
         self.output_height = output_shape[2]
         self.output_width = output_shape[3]
-        self.output_channels = output_shape[1]
         self.activation_function = activation_function
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert all((type(shape) == int for shape in input_shape) for input_shape in self.input_shapes)
-        assert self.axis in [1,2,3]
-        assert type(self.output_channels) == int
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
-        assert isinstance(self.activation_function, ActivationFunctions)
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in Gather (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in Gather (size must be int)")
+        if type(self.axis) != int:
+            raise TypeError("Erro: axis type in Gather (axis must be int)")
+        if type(self.indices) != np.ndarray:
+            raise TypeError("Error: indices in Gather (indices must be an numpy array)")
+        if type(self.output_channels) != int:
+            raise TypeError("Error: output channels type in Gather (must be int)")
+        if type(self.output_height) != int:
+            raise TypeError("Error: output height type in Gather (must be int)")
+        if type(self.output_width) != int:
+            raise TypeError("Error: output width type in Gather (must be int)")
+        if type(self.input_height) != int:
+            raise TypeError("Error: input height type in Gather (must be int)")
+        if type(self.input_width) != int:
+            raise TypeError("Error: input width type in Gather (must be int)")
+        if not isinstance(self.activation_function, ActivationFunctions):
+            raise TypeError("Error: activation function type in Gather (activation function must be a sub-classe of acetone_nnet Activation Function)")
 
         ### Checking value consistency ###
-        assert self.size == self.output_channels*self.output_height*self.output_width
-        assert self.axis == 1 or all(self.output_channels == input_shape[1] for input_shape in self.input_shapes)
-        assert self.axis == 2 or all(self.output_height== input_shape[2] for input_shape in self.input_shapes)
-        assert self.axis == 3 or all(self.output_width == input_shape[3] for input_shape in self.input_shapes)
-    
+        if self.size != self.output_channels*self.output_height*self.output_width:
+            raise ValueError("Error: size value in Gather ("+str(self.size)+"!="+str(self.output_channels*self.output_height*self.output_width)+")")
+        if axis not in [1,2,3]:
+            raise ValueError("Error: axis out of bound in Gather ("+str(axis)+"for tensor in 4 dimension with first dimension unused)")
+        for indice in self.indices.flatten():
+            if indice < 0 or indice >= input_shape[self.axis]:
+                raise ValueError("Error: indice out of bound in Gather ("+str(indice)+"out of bound for input of size"+str(input_shape[self.axis])+")")
+        
     def generate_inference_code_layer(self):
-        borne_sup = 0
-        borne_inf = 0
+        output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['comment'] = self.activation_function.comment
+        mustach_hash['output_str'] = output_str
         mustach_hash['road'] = self.path
         mustach_hash['size'] = self.size
 
-        mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[k]')
+        mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[position]')
 
-        mustach_hash['output_channels'] = self.output_channels
-        mustach_hash['output_height'] = self.output_height
-        mustach_hash['output_width'] = self.output_width
+        mustach_hash['indices_len'] = len(self.indices.flatten())
+        mustach_hash['input_width'] = self.input_width
+        mustach_hash['input_height'] = self.input_height
 
         if(self.axis == 1):
             mustach_hash['channels'] = True
+            mustach_hash['output_height'] = self.output_height
+            mustach_hash['output_width'] = self.output_width
         elif(self.axis == 2):
             mustach_hash['heights'] = True
+            mustach_hash['output_channels'] = self.output_channels
+            mustach_hash['output_width'] = self.output_width
         elif(self.axis == 3):
             mustach_hash['widths'] = True
+            mustach_hash['output_channels'] = self.output_channels
+            mustach_hash['output_height'] = self.output_height
 
-        mustach_hash['concat'] = []
-        for k in range(len(self.previous_layer)):
-            borne_sup += self.input_shapes[k][self.axis]
-
-            layer_to_concat = {}
-            layer_to_concat['input_width'] = self.input_shapes[k][3]
-            layer_to_concat['input_height'] = self.input_shapes[k][2]
-            layer_to_concat['output_str'] = self.previous_layer[k].output_str
-            layer_to_concat['borne_sup'] = borne_sup
-            layer_to_concat['borne_inf'] = borne_inf
-            mustach_hash['concat'].append(layer_to_concat)
+        if(self.activation_function.name == 'linear'):
+            mustach_hash['linear'] = True
 
-            borne_inf += self.input_shapes[k][self.axis]
+        if(self.fused_layer):
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tensor_temp[position]',self.idx,'position')
 
-
-        with open(self.template_path+'layers/template_Concatenate.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Gather.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
-    
-    def forward_path_layer(self, inputs):
-        output = inputs[0]
-        output = output.reshape(self.input_shapes[0][1],self.input_shapes[0][2],self.input_shapes[0][3])
-        for i in range(1,len(inputs)):
-            input = inputs[i]
-            input = input.reshape(self.input_shapes[i][1],self.input_shapes[i][2],self.input_shapes[i][3])
-            output = np.concatenate((output, input),axis=self.axis - 1) 
-        return self.activation_function.compute(output)
+        
+    def forward_path_layer(self, input:np.ndarray):
+        input = input.reshape(self.output_channels,self.input_height,self.input_width)
+        return np.take(input, indices=self.indices, axis=self.axis-1)
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,99 +14,105 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from ...Layer import Layer
-from ...activation_functions import ActivationFunctions
+from .Resize import Resize
 import numpy as np
 import math
-from abc import abstractmethod
+import pystache
 
-class Conv2D(Layer):
+#The mode Linear of the Resize layers
+#The value in the output tensor are found thanks to a (bi)linear interpolation
+class ResizeLinear(Resize):
     
-    def __init__(self, idx:int, conv_algorithm:str, size:int, padding:str|np.ndarray, strides:int, kernel_h:int, kernel_w:int, dilation_rate:int, nb_filters:int, input_shape:list, output_shape:list, weights:np.ndarray, biases:np.ndarray, activation_function:ActivationFunctions):
-        super().__init__()
-        self.conv_algorithm = conv_algorithm
-        self.idx = idx
-        self.size = size
-        self.name = 'Conv2D'
-        self.padding = padding
-        self.strides = strides
-        self.kernel_h = kernel_h
-        self.kernel_w = kernel_w
-        self.dilation_rate = dilation_rate
-        self.nb_filters = nb_filters
-    
-        self.input_channels = input_shape[1]
-        self.input_height = input_shape[2]
-        self.input_width = input_shape[3]
-        self.output_height = output_shape[2]
-        self.output_width = output_shape[3]
-
-        self.input_shape = [self.input_channels, self.input_height, self.input_width]
-        self.output_channels = self.nb_filters
-
-        self.weights = weights
-        self.biases = biases
-        self.activation_function = activation_function
-        self.local_var = 'sum'
-
-        self.nb_weights = self.count_elements_array(self.weights)
-        self.nb_biases = self.count_elements_array(self.biases)
-        self.pad_right, self.pad_left, self.pad_bottom, self.pad_top = self.compute_padding(self.padding,self.input_height, self.input_width, self.kernel_h, self.kernel_w, self.strides, self.dilation_rate)
-    
-        ####### Checking the instantiation#######
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.mode = 'linear'
+        self.template_dict = {'1D':self.template_path+'layers/Resize/template_ResizeLinear1D.c.tpl',
+                              '2D':self.template_path+'layers/Resize/template_ResizeLinear2D.c.tpl'}
+        
+    def generate_inference_code_layer(self):
 
-        ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert type(conv_algorithm) == str
-        assert type(self.padding) == str or all(type(pad) == int for pad in self.padding)
-        assert type(self.strides) == int
-        assert type(self.kernel_h) == int
-        assert type(self.kernel_w) == int
-        assert type(self.dilation_rate) == int
-        assert type(self.nb_filters) == int
-        assert type(self.input_channels) == int
-        assert type(self.input_height) == int
-        assert type(self.input_width) == int
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
-        assert type(self.weights) == np.ndarray
-        assert type(self.biases) == np.ndarray
-
-        ### Checking value consistency ###
-        assert self.size == self.output_channels*self.output_height*self.output_width
-        assert self.weights.shape == (self.input_channels, self.kernel_h, self.kernel_w, self.nb_filters)
-        assert len(self.biases.shape) == 1 and self.biases.shape[0] == self.nb_filters
-        assert self.output_height == math.floor((self.input_height + self.pad_bottom + self.pad_top - self.kernel_h - (self.kernel_h - 1)*(self.dilation_rate - 1))/self.strides) + 1
-        assert self.output_width == math.floor((self.input_width + self.pad_left + self.pad_right - self.kernel_w - (self.kernel_w - 1)*(self.dilation_rate - 1))/self.strides) + 1
-        assert self.conv_algorithm in ['6loops',
-                                       'indirect_gemm_nn','indirect_gemm_tn','indirect_gemm_nt','indirect_gemm_tt',
-                                       'std_gemm_nn','std_gemm_tn','std_gemm_nt','std_gemm_']
+        output_str = self.previous_layer[0].output_str
 
-    @abstractmethod
-    def generate_inference_code_layer(self):
-        pass
+        mustach_hash = {}
 
-    def forward_path_layer(self, input:np.ndarray):
-        # Conv for chw
-        input = input.reshape(self.input_channels, self.input_height, self.input_width)
+        mustach_hash['name'] = self.name
+        mustach_hash['idx'] = "{:02d}".format(self.idx)
+        mustach_hash['comment'] = self.activation_function.comment
+        mustach_hash['output_str'] = output_str
+        mustach_hash['road'] = self.path
+        mustach_hash['size'] = self.size
+
+        if(self.activation_function.name != 'linear'):
+            mustach_hash['linear'] = True
+            mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[j + ' + str(self.output_width) + '*(i + ' + str(self.output_height) + '*f)]')
+
+        mustach_hash['output_channels'] = self.output_channels
+        mustach_hash['output_height'] = self.output_height
+        mustach_hash['output_width'] = self.output_width
         
-        output = np.zeros((self.nb_filters, self.output_height, self.output_width))
-        print(self.weights.shape)
+        if ((self.input_height == 1) and (self.input_width > 1)):
+            mustach_hash['len_dimension'] = self.input_width-1
+            mustach_hash['dimension'] = self.input_width
+            mustach_hash['coordinate_transformation_mode'] = self.coordinate_transformation_mode_mapping[self.coordinate_transformation_mode]('j',3,'x')
+            dimension = '1D'
+            #return self.write_cst_interpolation_1D_width()
+        elif((self.input_height > 1) and (self.input_width == 1)):
+            mustach_hash['len_dimension'] = self.input_height-1
+            mustach_hash['dimension'] = self.input_height
+            mustach_hash['coordinate_transformation_mode'] = self.coordinate_transformation_mode_mapping[self.coordinate_transformation_mode]('i',2,'x')
+            dimension = '1D'
+            #return self.write_cst_interpolation_1D_height()
+        elif((self.input_height > 1) and (self.input_width > 1)):
+            mustach_hash['len_height'] = self.input_height-1
+            mustach_hash['len_width'] = self.input_width-1
+            mustach_hash['input_width'] = self.input_width
+            mustach_hash['input_height'] = self.input_height
+            mustach_hash['coordinate_transformation_mode_x'] = self.coordinate_transformation_mode_mapping[self.coordinate_transformation_mode]('i',2,'x')
+            mustach_hash['coordinate_transformation_mode_y'] = self.coordinate_transformation_mode_mapping[self.coordinate_transformation_mode]('j',3,'y')
+            dimension = '2D'
+            #return self.write_cst_interpolation_2D()
+
+        if(self.fused_layer):
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tensor_temp[j + ' + str(self.output_width) + '*(i + ' + str(self.output_height) + '*f)]',self.idx,'j + ' + str(self.output_width) + '*(i + ' + str(self.output_height) + '*f)')
+
+        with open(self.template_dict[dimension],'r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return pystache.render(template,mustach_hash)
 
-        if self.pad_right and self.pad_left and self.pad_top and self.pad_bottom:
-            input_padded = np.zeros((self.input_channels, self.input_height + self.pad_top + self.pad_bottom, self.input_width + self.pad_left + self.pad_right))
-            input_padded[:, self.pad_top:-self.pad_bottom, self.pad_left:-self.pad_right] = input
-        else:
-            input_padded = input
-            
-        for f in range(self.nb_filters):
+    def forward_path_layer(self, input:np.ndarray):
+        input = input.reshape(self.input_channels, self.input_height, self.input_width)
+        output = np.zeros((self.output_channels,self.output_height,self.output_width))
+        for f in range(self.output_channels):
             for i in range(self.output_height):
                 for j in range(self.output_width):
-                        output[f,i,j]=np.sum(input_padded[:, i*self.strides:i*self.strides+self.kernel_h, j*self.strides:j*self.strides+self.kernel_w] 
-                                            * self.weights[:,:,:,f]) + self.biases[f]
-        return self.activation_function.compute(output)
+                    x = self.coordinate_transformation_mode_implem_mapping[self.coordinate_transformation_mode](i,2)
+                    x = np.clip(x,0,self.input_height-1)
+                    y = self.coordinate_transformation_mode_implem_mapping[self.coordinate_transformation_mode](j,3)
+                    y = np.clip(y,0,self.input_width-1)
+
+                    x0,x1 = math.floor(x), math.floor(x) + 1
+                    y0,y1 = math.floor(y), math.floor(y) + 1
+
+                    f11 = input[f,x0,y0]
+                    if x1 >= self.input_height:
+                        f21 = 0
+                    else:
+                        f21 = input[f,x1,y0]
+                    if x1 >= self.input_height or y1 >= self.input_width:
+                        f22 = 0
+                    else:
+                        f22 = input[f,x1,y1]
+                    if y1 >= self.input_width:
+                        f12 = 0
+                    else:
+                        f12 = input[f,x0,y1]
+                    
+                    output[f,i,j] = (f11*(x1 - x)*(y1 - y) + f21*(x - x0)*(y1 - y) + f12*(x1 - x)*(y - y0) + f22*(x - x0)*(y - y0))/((x1 - x0)*(y1 - y0))
+        
+        return output
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,74 +14,84 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from ..Layer import Layer
-from ..activation_functions import ActivationFunctions
-import numpy as np
 import pystache
+import numpy as np
+from abc import ABC
+from ... import templates
 
-class Dense(Layer):
+class Normalizer(ABC):
 
-    def __init__(self, idx:int, size:int, weights:np.ndarray, biases:np.ndarray, activation_function:ActivationFunctions):
-        
+    def __init__(self, input_size:int, output_size:int, mins:list, maxes:list, means:list, ranges:list):
+        self.input_size = input_size
+        self.output_size = output_size
+        self.mins = mins
+        self.maxes = maxes
+        self.means = means
+        self.ranges = ranges
+        self.template_path = templates.__file__[:-11]
         super().__init__()
-        self.idx = idx
-        self.size = size
-        self.name = 'Dense'
-        self.weights = weights
-        self.biases = biases
-        self.activation_function = activation_function
-        self.local_var = 'dotproduct'
-        
-        self.nb_weights = self.count_elements_array(self.weights)
-        self.nb_biases = self.count_elements_array(self.biases)
-
-        ####### Checking the instantiation#######
-
-        ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert type(self.weights) == np.ndarray
-        assert type(self.biases) == np.ndarray
-        assert isinstance(self.activation_function, ActivationFunctions)
-
-        ### Checking value consistency ###
-        assert self.size == self.weights.shape[-1]
-        assert self.size == self.biases.shape[0]
-
-        
-    def generate_inference_code_layer(self):
-        #Variable indicating under which name the input tensor is
-        output_str = self.previous_layer[0].output_str
-
-        mustach_hash = {}
-
-        mustach_hash['name'] = self.name
-        mustach_hash['idx'] = "{:02d}".format(self.idx)
-        mustach_hash['comment'] = self.activation_function.comment
-        mustach_hash['output_str'] = output_str
-        mustach_hash['road'] = self.path
-        mustach_hash['size'] = self.size
-
-        mustach_hash['activation_function'] = self.activation_function.write_activation_str(self.local_var)
-
-        mustach_hash['prev_size'] = self.previous_layer[0].size
-
-        if(self.fused_layer):
-            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str(self.local_var,self.idx,'i')
-
-            if(self.activation_function.name == 'linear'):
-                mustach_hash['linear'] = True
-        
-        with open(self.template_path+'layers/template_Dense.c.tpl','r') as template_file:
+
+    def array_to_str(self, array:list):
+        s = "{"
+        for element in array:
+            s += str(element) + ", "
+        s = s[:-2] + "}"
+        return s
+
+    def write_pre_processing(self):
+        with open(self.template_path+'normalization/template_pre_processing.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return pystache.render(template,{'input_size':self.input_size})
+
+
+    def write_post_processing(self):
+        with open(self.template_path+'normalization/template_post_processing.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return pystache.render(template,{'output_size':self.output_size})
+
+    def write_normalization_cst_in_header_file(self):
+        mustach_hash= {}
+
+        mustach_hash['input_size'] = self.input_size
+
+        with open(self.template_path+'normalization/template_normalization_cst_in_header_file.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
+    
+    def write_normalization_cst_in_globalvars_file(self):
+        mustach_hash= {}
+
+        mustach_hash['input_size'] = self.input_size
+        mustach_hash['input_min'] = self.array_to_str(self.mins)
+        mustach_hash['input_max'] = self.array_to_str(self.maxes)
+        mustach_hash['input_mean'] = self.array_to_str(self.means[:-1])
+        mustach_hash['input_range'] = self.array_to_str(self.ranges[:-1])
+        mustach_hash['output_mean'] = self.means[-1]
+        mustach_hash['output_range'] = self.ranges[-1]
+
+        with open(self.template_path+'normalization/template_normalization_cst_in_global_var_file.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return  pystache.render(template, mustach_hash)
 
-    def forward_path_layer(self, input:np.ndarray):
-        input = input.reshape(self.previous_layer[0].size)
-        return self.activation_function.compute(np.dot(input, self.weights) + self.biases)
+    def pre_processing(self, nn_input:np.ndarray):
+        inputs = nn_input.flatten()
+        for i in range(self.input_size):
+            inputs[i] = (max(self.mins[i],min(self.maxes[i],inputs[i])) - self.means[i]) / self.ranges[i]
+        return np.reshape(inputs, nn_input.shape)
+
+    def post_processing(self, nn_output:np.ndarray):
+        for i in range(len(nn_output)):
+            nn_output[i] = nn_output[i]*self.ranges[-1] + self.means[-1]
+        return nn_output
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,18 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
+##############################################
+############ STAND BY. UN-UPDATED ############
+##############################################
+
 from ..Layer import Layer
 from..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 
 #Do the dotproduct of two tensors
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,57 +15,56 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ..Layer import Layer
-import pystache
 import numpy as np
+import pystache
 
-class Flatten(Layer):
+class Softmax(Layer):
 
-    def __init__(self, idx:int, size:int, input_shape:int, data_format:str):
-       
+    def __init__(self, idx:int, size:int, axis:int|None):
+        
         super().__init__()
         self.idx = idx
         self.size = size
-        self.input_shape = input_shape
-        self.data_format = data_format
-        self.name = 'Flatten'
+        self.name = 'Softmax'
+        self.axis = axis
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert all(type(shape) == int for shape in self.input_shape[1:])
-        assert self.data_format == 'channels_last' or self.data_format == 'channels_first'
-
-        ### Checking value consistency ###
-        assert self.size == self.input_shape[1]*self.input_shape[2]*self.input_shape[3]
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in Softmax (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in Softmax (size must be int)")
+        if  type(self.axis)!= int and self.axis!=None:
+            raise TypeError("Error: axis type in Softmax (axis must be int or None)")
 
     def generate_inference_code_layer(self):
+        output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
-        if(self.data_format == 'channels_last'):
-            mustach_hash['channels_last'] = True
-            mustach_hash['input_channels'] = self.input_shape[1]
-            mustach_hash['input_height'] = self.input_shape[2]
-            mustach_hash['input_width'] = self.input_shape[3]
-            mustach_hash['name'] = self.name
-            mustach_hash['idx'] = "{:02d}".format(self.idx)
-            mustach_hash['path'] = self.path
-            mustach_hash['size'] = self.size
+        mustach_hash['name'] = self.name
+        mustach_hash['idx'] = "{:02d}".format(self.idx)
+        mustach_hash['size'] = self.size
+        mustach_hash['road'] = self.path
+        mustach_hash['output_str'] = output_str
 
-        with open(self.template_path+'layers/template_Flatten.c.tpl','r') as template_file:
+        if (self.fused_layer):
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output_'+str(self.path)+'[j]', self.idx, 'j')
+
+        with open(self.template_path+'layers/template_Softmax.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
-
+    
     def forward_path_layer(self, input:np.ndarray):
-        if(self.data_format == 'channels_last'):
-            return np.transpose(np.reshape(input,self.input_shape[1:]),(1,2,0))
-        else:
-            return input
+        
+        exp = np.exp(input, dtype=np.float)
+        output = exp/np.sum(exp,keepdims=1, axis=self.axis)
+
+        return output
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,93 +19,88 @@
 """
 
 from ..Layer import Layer
 from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
-#extract a list of subtensor from a given tensor
-#attribut: axis alongside of which the submatrix will be extracted (if the desired submatrix must have the height, width or channels of the parent tensor)
-#input: a tensor
-#output: a list of tensor
-class Gather(Layer):
-    
-    def __init__(self, idx:int, size:int, axis:int,  indices:np.ndarray, input_shape:list, output_shape:list, activation_function:ActivationFunctions):
+class MatMul(Layer):
+
+    def __init__(self, idx:int, size:int, input_shape:list, weights:np.ndarray, side:bool, activation_function:ActivationFunctions):
         
         super().__init__()
         self.idx = idx
         self.size = size
-        self.name = 'Gather'
-        self.indices = indices
-        self.axis = axis
-        self.output_channels = input_shape[1]
-        self.input_height = input_shape[2]
-        self.input_width = input_shape[3]
-        self.output_height = output_shape[2]
-        self.output_width = output_shape[3]
+        self.name = 'MatMul'
+        self.weights = weights
         self.activation_function = activation_function
+        self.local_var = 'dotproduct'
+        self.side = side
+        self.input_shape = input_shape
+        self.nb_weights = self.count_elements_array(self.weights)
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert type(self.axis) == int
-        assert type(self.indices) == np.ndarray
-        assert type(self.output_channels) == int
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
-        assert type(self.input_height) == int
-        assert type(self.input_width) == int
-        assert isinstance(self.activation_function,ActivationFunctions)
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in MatMul (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in MatMul (size must be int)")
+        if any(type(shape) != int for shape in self.input_shape):
+            raise TypeError("Error: input_shape in MatMul (all dim must be int)")
+        if type(self.weights) != np.ndarray:
+            raise TypeError("Error: weights in MatMul (weights must be an numpy array)")
+        if type(side) != bool:
+            raise TypeError("Error: side type in MatMul (side must be a boolean)")
+        if not isinstance(self.activation_function, ActivationFunctions):
+            raise TypeError("Error: activation function type in MatMul (activation function must be a sub-classe of acetone_nnet Activation Function)")
 
         ### Checking value consistency ###
-        assert self.size == self.output_channels*self.output_height*self.output_width
-        assert axis in [1,2,3]
-        assert all(indice >= 0 and indice < input_shape[axis] for indice in self.indices.flatten())
+        if self.side:
+            if self.weights.shape[-1] != self.input_shape[-2]:
+                raise ValueError("Error: non consistency between weight shape and input shape in MatMul ("+str(self.weights.shape[-1])+"!="+str(self.input_shape[-2])+")")
+            if self.size != self.weights.shape[-2] * self.input_shape[-1]:
+                raise ValueError("Error: size value in MatMul ("+str(self.size)+" !="+str(self.weights.shape[-2] * self.input_shape[-1])+")")
+        else:
+            if self.weights.shape[-2] != self.input_shape[-1]:
+                raise ValueError("Error: non consistency between weight shape and input shape in MatMul ("+str(self.weights.shape[-2])+"!="+str(self.input_shape[-1])+")")
+            if self.size != self.weights.shape[-1] * self.input_shape[-2]:
+                raise ValueError("Error: size value in MatMul ("+str(self.size)+" !="+str(self.weights.shape[-1] * self.input_shape[-2])+")")
         
+
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['comment'] = self.activation_function.comment
         mustach_hash['output_str'] = output_str
         mustach_hash['road'] = self.path
         mustach_hash['size'] = self.size
 
-        mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[position]')
+        mustach_hash['activation_function'] = self.activation_function.write_activation_str(self.local_var)
 
-        mustach_hash['indices_len'] = len(self.indices.flatten())
-        mustach_hash['input_width'] = self.input_width
-        mustach_hash['input_height'] = self.input_height
-
-        if(self.axis == 1):
-            mustach_hash['channels'] = True
-            mustach_hash['output_height'] = self.output_height
-            mustach_hash['output_width'] = self.output_width
-        elif(self.axis == 2):
-            mustach_hash['heights'] = True
-            mustach_hash['output_channels'] = self.output_channels
-            mustach_hash['output_width'] = self.output_width
-        elif(self.axis == 3):
-            mustach_hash['widths'] = True
-            mustach_hash['output_channels'] = self.output_channels
-            mustach_hash['output_height'] = self.output_height
-
-        if(self.activation_function.name == 'linear'):
-            mustach_hash['linear'] = True
+        mustach_hash['prev_size'] = self.previous_layer[0].size
+        mustach_hash['side'] = self.side
 
         if(self.fused_layer):
-            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tensor_temp[position]',self.idx,'position')
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str(self.local_var,self.idx,'i')
 
-        with open(self.template_path+'layers/template_Gather.c.tpl','r') as template_file:
+            if(self.activation_function.name == 'linear'):
+                mustach_hash['linear'] = True
+        
+        with open(self.template_path+'layers/template_MatMul.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
         
-    def forward_path_layer(self, input:np.ndarray):
-        input = input.reshape(self.output_channels,self.input_height,self.input_width)
-        return np.take(input, indices=self.indices, axis=self.axis-1)
+    def forward_path_layer(self, input):
+        input = input.reshape(self.input_shape)
+        if self.side:
+            weights = np.moveaxis(self.weights,3,0)
+            weights = np.reshape(weights,(1,1,weights.shape[-1],weights.shape[0]))
+            return self.activation_function.compute(np.matmul(weights,input))
+        else:
+            return self.activation_function.compute(np.matmul(input,self.weights))
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files 21% similar despite different names*

```diff
@@ -63,33 +63,52 @@
         self.activation_function = activation_function
         self.nb_weights = self.count_elements_array(self.weights)
         self.nb_biases = self.count_elements_array(self.biases)
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert type(self.alpha[0]) == float or type(self.alpha[0]) == int
-        assert type(self.beta[0]) == float or type(self.beta[0]) == int
-        assert all(type(self.transpo[i]) == int or type(self.transpo[i]) == bool for i in range(2))
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
-        assert type(self.input_height) == int
-        assert type(self.input_width) == int
-        assert type(self.weights) == np.ndarray
-        assert type(self.biases) == np.ndarray
-        assert isinstance(self.activation_function,ActivationFunctions)
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in Gemm (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in Gemm (size must be int)")
+        if  type(self.alpha[0]) != float and type(self.alpha[0]) == int:
+            raise TypeError("Error: alpha type in Gemm (alpha must be int or float)")
+        if  type(self.beta[0]) != float and type(self.beta[0]) == int:
+            raise TypeError("Error: beta type in Gemm (beta must be int or float)")
+        if any(type(self.transpo[i]) != int and type(self.transpo[i]) != bool for i in range(2)):
+            raise TypeError("Error: transpose type in Gemm (must be boolean or int)")
+        if type(self.output_height) != int:
+            raise TypeError("Error: output height type in Gemm (must be int)")
+        if type(self.output_width) != int:
+            raise TypeError("Error: output width type in Gemm (must be int)")
+        if type(self.input_height) != int:
+            raise TypeError("Error: input height type in Gemm (must be int)")
+        if type(self.input_width) != int:
+            raise TypeError("Error: input width type in Gemm (must be int)")
+        if type(self.weights) != np.ndarray:
+            raise TypeError("Error: weights in Gemm (weights must be an numpy array)")
+        if type(self.biases) != np.ndarray:
+            raise TypeError("Error: biases in Gemm (biases must be an numpy array)")
+        if not isinstance(self.activation_function, ActivationFunctions):
+            raise TypeError("Error: activation function type in Gemm (activation function must be a sub-classe of acetone_nnet Activation Function)")
 
         ### Checking value consistency ###
-        assert self.size == self.output_height*self.output_width
-        assert self.weights.shape[self.transpo[1]] == self.input_height if self.transpo[0] else self.input_width
-        assert self.output_height == self.input_width if self.transpo[0] else self.input_height
-        assert self.output_width == self.weights.shape[1-self.transpo[1]]
-        assert all(self.biases.shape[i] == 1 or self.biases.shape[i] == output_shape[3-i] for i in range(len(self.biases.shape)))
+        if self.size != self.output_height*self.output_width:
+            raise ValueError("Error: size value in Gemm ("+str(self.size)+"!="+str(self.output_height*self.output_width)+")")
+        if self.weights.shape[self.transpo[1]] != self.input_height if self.transpo[0] else self.input_width:
+            shape = self.input_height if self.transpo[0] else self.input_width
+            raise ValueError("Error: non consistency between weight shape and input shape in Gemm ("+str(self.weights.shape[self.transpo[1]])+"!="+str(shape)+")")
+        if self.output_height != self.input_width if self.transpo[0] else self.input_height:
+            shape = self.input_width if self.transpo[0] else self.input_height
+            raise ValueError("Error: non consistency between input shape and output shape in Gemm ("+str(self.output_height)+"!="+str(shape)+")")
+        if self.output_width != self.weights.shape[1-self.transpo[1]]:
+            raise ValueError("Error: non consistency between output shape and weight shape in Gemm ("+str(self.output_width)+"!="+str(self.weights.shape[1-self.transpo[1]])+")")
+        if any(self.biases.shape[i] != 1 and self.biases.shape[i] != output_shape[3-i] for i in range(len(self.biases.shape))):
+            raise ValueError("Error: biases in Gemm not broadcastable to dim "+str((self.output_height,self.output_width)))
 
         
     #The various ways to compute the operation: 
     
     #None of the tensor ar transposed
     def write_gemm_nn(self, m, n, k, A, B):
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,70 +14,65 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import numpy as np
 from ..Layer import Layer
 import pystache
+import numpy as np
 
-class InputLayer(Layer):
+class Flatten(Layer):
 
-    def __init__(self, idx:int, size:int, input_shape:list, data_format:str):
+    def __init__(self, idx:int, size:int, input_shape:int, data_format:str):
        
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shape = input_shape
-        if len(self.input_shape) == 4:
-            self.output_channels = self.input_shape[1]
-            self.output_height = self.input_shape[2]
-            self.output_width = self.input_shape[3]
         self.data_format = data_format
-        self.name = 'Input_layer'
+        self.name = 'Flatten'
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert all(type(dim) == int for dim in self.input_shape[1:])
-        assert self.data_format == 'channels_last' or self.data_format == 'channels_first'
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in Flatten (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in Flatten (size must be int)")
+        if any(type(shape) != int for shape in self.input_shape):
+            raise TypeError("Error: input_shape in Flatten (all dim must be int)")
+        if type(self.data_format) != str:
+            raise TypeError("Error: data format type in Flatten")
 
         ### Checking value consistency ###
-        prod = 1
-        for shape in self.input_shape:
-            if shape != None and shape != 0:
-                prod *= shape
-
-        assert self.size == prod
+        if self.size != self.input_shape[1]*self.input_shape[2]*self.input_shape[3]:
+            raise ValueError("Error: size value in Flatten ("+str(self.size)+"!="+str(self.input_shape[1]*self.input_shape[2]*self.input_shape[3])+")")
+        if self.data_format not in ['channels_last','channels_first']:
+            raise ValueError("Error: data format value in Flatten ("+self.data_format+")")
 
     def generate_inference_code_layer(self):
 
         mustach_hash = {}
 
-        mustach_hash['name'] = self.name
-        mustach_hash['idx'] = "{:02d}".format(self.idx)
-        mustach_hash['road'] = self.path
-
-        if(self.data_format == 'channels_last' and len(self.input_shape) == 4):
+        if(self.data_format == 'channels_last'):
             mustach_hash['channels_last'] = True
-            mustach_hash['input_channels'] = self.output_channels
-            mustach_hash['input_height'] = self.output_height
-            mustach_hash['input_width'] = self.output_width
-        else:
+            mustach_hash['input_channels'] = self.input_shape[1]
+            mustach_hash['input_height'] = self.input_shape[2]
+            mustach_hash['input_width'] = self.input_shape[3]
+            mustach_hash['name'] = self.name
+            mustach_hash['idx'] = "{:02d}".format(self.idx)
+            mustach_hash['path'] = self.path
             mustach_hash['size'] = self.size
 
-
-
-
-        with open(self.template_path+'layers/template_Input_Layer.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Flatten.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def forward_path_layer(self, input:np.ndarray):
-        
-        return input 
+        if(self.data_format == 'channels_last'):
+            return np.transpose(np.reshape(input,self.input_shape[1:]),(1,2,0))
+        else:
+            return input
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,82 +13,73 @@
  * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
+from .Pad import Pad
 
-from ..Layer import Layer
-from ..activation_functions import ActivationFunctions
-import numpy as np
 import pystache
 
-class MatMul(Layer):
+#The Edge mode of the Pad layers
+#Pads with the edge values of array.
+class Edge_pad(Pad):
+    
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.mode = 'edge'
 
-    def __init__(self, idx:int, size:int, input_shape:list, weights:np.ndarray, side:bool, activation_function:ActivationFunctions):
-        
-        super().__init__()
-        self.idx = idx
-        self.size = size
-        self.name = 'MatMul'
-        self.weights = weights
-        self.activation_function = activation_function
-        self.local_var = 'dotproduct'
-        self.side = side
-        self.input_shape = input_shape
-        self.nb_weights = self.count_elements_array(self.weights)
-
-        ####### Checking the instantiation#######
-
-        ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert all(type(shape) == int for shape in self.input_shape)
-        assert type(self.weights) == np.ndarray
-        assert type(side) == bool
-        assert isinstance(self.activation_function, ActivationFunctions)
-
-        ### Checking value consistency ###
-        if self.side:
-            assert self.weights.shape[-1] == self.input_shape[-2]
-            assert self.size == self.weights.shape[-2] * self.input_shape[-1]
-        else:
-            assert self.weights.shape[-2] == self.input_shape[-1]
-            assert self.size == self.weights.shape[-1] * self.input_shape[-2]
+    def write_padding(self):
+        mustach_hash = {}
+
+        mustach_hash['pads_front'] = self.pads[1]
+        mustach_hash['pads_top'] = self.pads[2]
+        mustach_hash['pads_left'] = self.pads[3]
+        mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
+        mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
+        mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
+
+        with open(self.template_path+'layers/Pad/template_Edge_Pad.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return pystache.render(template, mustach_hash)
+    
 
     def generate_inference_code_layer(self):
+        
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['comment'] = self.activation_function.comment
+        mustach_hash['size'] = self.size
         mustach_hash['output_str'] = output_str
         mustach_hash['road'] = self.path
-        mustach_hash['size'] = self.size
 
-        mustach_hash['activation_function'] = self.activation_function.write_activation_str(self.local_var)
+        mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
 
-        mustach_hash['prev_size'] = self.previous_layer[0].size
-        mustach_hash['side'] = self.side
+        mustach_hash['output_channels'] = self.output_channels
+        mustach_hash['output_height'] = self.output_height
+        mustach_hash['output_width'] = self.output_width
+        mustach_hash['pads_front'] = self.pads[1]
+        mustach_hash['pads_top'] = self.pads[2]
+        mustach_hash['pads_left'] = self.pads[3]
+        mustach_hash['input_width'] = self.input_shape[3]
+        mustach_hash['input_height'] = self.input_shape[2]
 
-        if(self.fused_layer):
-            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str(self.local_var,self.idx,'i')
+        mustach_hash['change_indice'] = self.write_padding()
 
-            if(self.activation_function.name == 'linear'):
-                mustach_hash['linear'] = True
+        if(self.activation_function.name == 'linear'):
+            mustach_hash['linear'] = True
         
-        with open(self.template_path+'layers/template_MatMul.c.tpl','r') as template_file:
+        if(self.fused_layer):
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tenser_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
+
+        with open(self.template_path+'layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
-        return pystache.render(template, mustach_hash)
-        
-    def forward_path_layer(self, input):
-        
-        input = input.reshape(self.input_shape)
-        if self.side:
-            return self.activation_function.compute(np.matmul(self.weights,input))
-        else:
-            return self.activation_function.compute(np.matmul(input,self.weights))
+        return pystache.render(template, mustach_hash)
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,37 +13,42 @@
  * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
+
 from .Pad import Pad
 
 import pystache
 
-#The Edge mode of the Pad layers
-#Pads with the edge values of array.
-class Edge_pad(Pad):
+#The Wrap mode of the Pad layers
+#Pads with the wrap of the vector along the axis. 
+#The first values are used to pad the end and the end values are used to pad the beginning.
+class Wrap_pad(Pad):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.mode = 'edge'
-
+        self.mode = 'wrap'
+    
     def write_padding(self):
         mustach_hash = {}
 
         mustach_hash['pads_front'] = self.pads[1]
         mustach_hash['pads_top'] = self.pads[2]
         mustach_hash['pads_left'] = self.pads[3]
         mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
         mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
         mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
-
-        with open(self.template_path+'layers/Pad/template_Edge_Pad.c.tpl','r') as template_file:
+        mustach_hash['input_channels'] = self.input_shape[1]
+        mustach_hash['input_width'] = self.input_shape[3]
+        mustach_hash['input_height'] = self.input_shape[2]
+        
+        with open(self.template_path+'layers/Pad/template_Wrap_Pad.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
 
     def generate_inference_code_layer(self):
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files 24% similar despite different names*

```diff
@@ -45,28 +45,40 @@
         self.output_width = input_shape[3] + pads[3] + pads[7]
         self.mode = ''
         self.activation_function = activation_function
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert all(type(pad) == int for pad in self.pads)
-        assert type(self.constant_value) == float or type(self.constant_value) == int
-        assert type(self.output_channels) == int
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
-        assert all(type(shape) == int for shape in self.input_shape[1:])
-        assert isinstance(self.activation_function, ActivationFunctions)
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in Pad (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in Pad (size must be int)")
+        if any(type(pad) != int for pad in self.pads):
+            raise TypeError("Error: pads type in Pad (must be int)")
+        if type(self.constant_value) != float and type(self.constant_value) != int:
+            raise TypeError("Error: constant value type in Pad (must be float or int)")
+        if type(self.output_channels) != int:
+            raise TypeError("Error: output channels type in Pad (must be int)")
+        if type(self.output_height) != int:
+            raise TypeError("Error: output height type in Pad (must be int)")
+        if type(self.output_width) != int:
+            raise TypeError("Error: output width type in Pad (must be int)")
+        if any(type(shape) != int for shape in self.input_shape[1:]):
+            raise TypeError("Error: input shape type in Pad (must be int)")
+        if not isinstance(self.activation_function, ActivationFunctions):
+            raise TypeError("Error: activation function type in Pad (activation function must be a sub-classe of acetone_nnet Activation Function)")
 
 
         ### Checking value consistency ###
-        assert self.size == self.output_channels*self.output_height*self.output_width
-        assert all(0 <= axe and axe < 4 for axe in self.axes)
+        if self.size != self.output_channels*self.output_height*self.output_width:
+            raise ValueError("Error: size value in Pad ("+str(self.size)+"!="+str(self.output_channels*self.output_height*self.output_width)+")")
+        for axe in self.axes:
+            if axe < 0 or axe >= 4:
+                raise ValueError("Error: axe out of bound in Pad ("+str(axe)+"for tensor in 4 dimension with first dimension unused)")
     
     def forward_path_layer(self, input:np.ndarray):
         input = input.reshape(self.input_shape[1], self.input_shape[2], self.input_shape[3])
         nb_dim = len(self.pads)//2
         pad_width = [(self.pads[i],self.pads[i+nb_dim]) for i in range(1,nb_dim)] #Constructing the pads accordingly to the numpy nomenclature
         return self.activation_function.compute(np.pad(input,pad_width=pad_width,mode=self.mode,constant_values=self.constant_value,))
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,32 +53,46 @@
 
         self.pad_right, self.pad_left, self.pad_bottom, self.pad_top = self.compute_padding(self.padding,self.input_height, self.input_width, self.pool_size,self.pool_size, self.strides)
 
 
     ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert type(self.padding) == str or all(type(pad) == int for pad in self.padding)
-        assert type(self.strides) == int
-        assert type(self.pool_size) == int
-        assert type(self.input_channels) == int
-        assert type(self.input_height) == int
-        assert type(self.input_width) == int
-        assert type(self.output_channels) == int
-        assert type(self.output_height) == int
-        assert type(self.output_width) == int
-        assert isinstance(self.activation_function, ActivationFunctions)
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in Pooling (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in Pooling (size must be int)")
+        if type(self.padding) != str and any(type(pad) != int for pad in self.padding):
+            raise TypeError("Error: padding type in Pooling (must be str or ints)")
+        if  type(self.strides)!= int:
+            raise TypeError("Error: strides type in Pooling (must be int)")
+        if  type(self.pool_size)!= int:
+            raise TypeError("Error: pool_size type in Pooling (must be int)")
+        if type(self.input_channels) != int:
+            raise TypeError("Error: input channels type in Pooling (must be int)")
+        if type(self.input_height) != int:
+            raise TypeError("Error: input height type in Pooling (must be int)")
+        if type(self.input_width) != int:
+            raise TypeError("Error: input width type in Pooling (must be int)")
+        if type(self.output_channels) != int:
+            raise TypeError("Error: output channels type in Pooling (must be int)")
+        if type(self.output_height) != int:
+            raise TypeError("Error: output height type in Pooling (must be int)")
+        if type(self.output_width) != int:
+            raise TypeError("Error: output width type in Pooling (must be int)")
+        if not isinstance(self.activation_function, ActivationFunctions):
+            raise TypeError("Error: activation function type in Pooling (activation function must be a sub-classe of acetone_nnet Activation Function)")
 
         ### Checking value consistency ###
-        assert self.size == self.output_channels*self.output_height*self.output_width
-        assert self.size == self.output_channels*self.output_height*self.output_width
-        assert self.output_height == math.floor((self.input_height + self.pad_bottom + self.pad_top - self.pool_size)/self.strides) + 1
-        assert self.output_width == math.floor((self.input_width + self.pad_left + self.pad_right - self.pool_size)/self.strides) + 1
+        if self.size != self.output_channels*self.output_height*self.output_width:
+            raise ValueError("Error: size value in Pooling ("+str(self.size)+"!="+str(self.output_channels*self.output_height*self.output_width)+")")
+        if self.output_height != math.floor((self.input_height + self.pad_bottom + self.pad_top - self.pool_size)/self.strides) + 1:
+            raise ValueError("Error: non consistency between the output height and the parameter of the operation in Pooling ("+str(self.output_height)+"!="+str(math.floor((self.input_height + self.pad_bottom + self.pad_top - self.pool_size)/self.strides) + 1)+")")
+        if self.output_width != math.floor((self.input_width + self.pad_left + self.pad_right - self.pool_size)/self.strides) + 1:
+            raise ValueError("Error: non consistency between the output width and the parameter of the operation in Pooling ("+str(self.output_width)+"!="+str(math.floor((self.input_width + self.pad_left + self.pad_right - self.pool_size)/self.strides) + 1)+")")
     
     @abstractmethod    
     def specific_function(self, index:str, input_of_layer:str):
         pass
 
     @abstractmethod    
     def update_local_vars(self):
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files 13% similar despite different names*

```diff
@@ -86,37 +86,62 @@
             self.scale[1] = self.output_channels / self.input_channels #should be 1
             self.scale[2] = self.output_height / self.input_height
             self.scale[3] = self.output_width / self.input_width
 
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-        assert type(self.input_channels) == int
-        assert type(self.input_height) == int
-        assert type(self.input_width) == int
-        assert type(self.coordinate_transformation_mode) == str
-        assert type(axes) == np.ndarray or type(axes) == list
-        assert type(self.exclude_outside) == int
-        assert type(self.keep_aspect_ratio_policy) == str
-        assert type(self.roi) == np.ndarray or type(self.roi) == list
-        assert type(self.extrapolation_value) == float or type(self.extrapolation_value) == int
+        if  type(self.idx)!= int:
+            raise TypeError("Error: idx type in Resize (idx must be int)")
+        if  type(self.size)!= int:
+            raise TypeError("Error: size type in Resize (size must be int)")
+        if type(self.input_channels) != int:
+            raise TypeError("Error: input channels type in Resize (must be int)")
+        if type(self.input_height) != int:
+            raise TypeError("Error: input height type in Resize (must be int)")
+        if type(self.input_width) != int:
+            raise TypeError("Error: input width type in Resize (must be int)")
+        if type(self.coordinate_transformation_mode) != str:
+            raise TypeError("Error: coordinate transformation mode type in Resize (must be str)")
+        if type(axes) != np.ndarray and type(axes) != list:
+            raise TypeError("Error: axes type in Resize (must be numpy array or list)")
+        if type(self.exclude_outside) != int:
+            raise TypeError("Error: exclude outside type in Resize (must be int)")
+        if type(self.keep_aspect_ratio_policy) != str:
+            raise TypeError("Error: keep aspect ratio policy type in Resize (must be str)")
+        if type(self.roi) != np.ndarray and type(self.roi) != list:
+            raise TypeError("Error: roi type in Resize (must be numpy array or list)")
+        if type(self.extrapolation_value) != float and type(self.extrapolation_value) != int:
+            raise TypeError("Error: extrapolation value type in Resize (must be int or float)")
 
         ### Checking value consistency ###
-        assert self.size == self.output_channels*self.output_height*self.output_width
-        assert self.coordinate_transformation_mode in ['half_pixel','half_pixel_symmetric','pytorch_half_pixel','align_corners','asymmetric','tf_crop_and_resize']
-        assert self.keep_aspect_ratio_policy in ['stretch','not_larger','not_smaller']
-        assert self.exclude_outside in [0,1]
-        assert all(axe >=0 and axe < 4 for axe in self.axes)
+        if self.size != self.output_channels*self.output_height*self.output_width:
+            raise ValueError("Error: size value in Resize ("+str(self.size)+"!="+str(self.output_channels*self.output_height*self.output_width)+")")
+        if self.coordinate_transformation_mode not in ['half_pixel','half_pixel_symmetric','pytorch_half_pixel','align_corners','asymmetric','tf_crop_and_resize']:
+            raise ValueError("Error: coordinate transformation mode value in Resize ("+self.coordinate_transformation_mode+")")
+        if self.keep_aspect_ratio_policy not in ['stretch','not_larger','not_smaller']:
+            raise ValueError("Error: keep aspect ratio policy value in Resize ("+self.keep_aspect_ratio_policy+")")
+        if self.exclude_outside not in [0,1]:
+            raise ValueError("Error: exclude outside value in Resize ("+self.exclude_outside+")")
+        for axe in self.axes:
+            if axe < 0 or axe >= 4:
+                raise ValueError("Error: axe out of bound in Resize ("+str(axe)+"for tensor in 4 dimension with first dimension unused)")
         if self.roi:
-            assert len(self.roi) == 2*len(self.axes) if self.axes else len(self.roi) == 8
-            assert all(0 <= indice and indice <= 1 for indice in self.roi)
+            if self.axes:
+                if len(self.roi) != 2*len(self.axes):
+                    raise ValueError("Error: non consistency between the number of roi and the axes given in Resize("+str(len(self.roi))+"!="+str(len(self.axes))+")")
+            else:
+                if len(self.roi) != 8:
+                    raise ValueError("Error: non consistency between the number of roi given and the size of the tensor in Resize ("+str(len(self.roi))+"!=8)")
+            if any(0 > indice and indice > 1 for indice in self.roi):
+                raise ValueError("Error: roi value is not noramlized in Resize ("+str(self.roi)+")")
         assert all(0 < coeff for coeff in self.scale)
-        
+        for coeff in self.scale:
+            if 0 >= coeff:
+                raise ValueError("Error: scale value in Resize ("+str(coeff)+")")        
 
     @abstractmethod
     def forward_path_layer(self, input:np.ndarray):
         pass
     
     @abstractmethod
     def generate_inference_code_layer(self):
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         self.mode = 'cubic'
         self.template_dict = {'1D':self.template_path+'layers/Resize/template_ResizeCubic1D.c.tpl',
                               '2D':self.template_path+'layers/Resize/template_ResizeCubic2D.c.tpl'}
         
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.cubic_coeff_a) == float or type(self.cubic_coeff_a) == int
+        if type(self.cubic_coeff_a) != float and type(self.cubic_coeff_a) != int:
+            raise TypeError("Error: cubic coeff a type in Resize Cubic (must be int or float)")
     
     def cubic_interpolation_1D(self, input:np.ndarray, f:int, x:int, y:int, s:float):
         col_index = max(0,min(self.input_width-1,y))
         f_1 = input[f,max(0,min(self.input_height-1,x-1)),col_index]
         f0 = input[f,max(0,min(self.input_height-1,x)),col_index]
         f1 = input[f,max(0,min(self.input_height-1,x+1)),col_index]
         f2 = input[f,max(0,min(self.input_height-1,x+2)),col_index]
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,18 +39,20 @@
                                             "round_prefer_ceil":self.round_prefer_ceil_implem,
                                             "floor":math.floor,
                                             "ceil":math.ceil}
         
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.nearest_mode) == str
+        if type(self.nearest_mode) != str:
+            raise TypeError("Error: nearest mode in Resize Nearest (must be string)")
 
         ### Checking value consistency ###
-        assert self.nearest_mode in ['round_prefer_floor','round_prefer_ceil','floor','ceil']
+        if self.nearest_mode not in ['round_prefer_floor','round_prefer_ceil','floor','ceil']:
+            raise ValueError("Error: nearest mode value in Resize Nearest ("+self.nearest_mode+")")
     
     #Defining the several method to chose the nearest
     def floor(self, x:str, y:str):
         return x+' = floor('+y+');'
     
     def ceil(self, x:str, y:str):
         return x+' = ceil('+y+');'
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,52 +14,33 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from ..Layer import Layer
+from .Broadcast import Broadcast
 import numpy as np
-import pystache
 
-class Softmax(Layer):
-
-    def __init__(self, idx:int, size:int):
-        
-        super().__init__()
-        self.idx = idx
-        self.size = size
-        self.name = 'Softmax'
-
-        ####### Checking the instantiation#######
-
-        ### Checking argument type ###
-        assert type(self.idx) == int
-        assert type(self.size) == int
-
-    def generate_inference_code_layer(self):
-        output_str = self.previous_layer[0].output_str
-
-        mustach_hash = {}
-
-        mustach_hash['name'] = self.name
-        mustach_hash['idx'] = "{:02d}".format(self.idx)
-        mustach_hash['size'] = self.size
-        mustach_hash['road'] = self.path
-        mustach_hash['output_str'] = output_str
-
-        if (self.fused_layer):
-            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output_'+str(self.path)+'[j]', self.idx, 'j')
-
-        with open(self.template_path+'layers/template_Softmax.c.tpl','r') as template_file:
-            template = template_file.read()
-        template_file.close()
-
-        return pystache.render(template, mustach_hash)
+#Addition of several tensor
+class Add(Broadcast):
     
-    def forward_path_layer(self, input:np.ndarray):
-        
-        exp = np.exp(input, dtype=np.float)
-        output = exp/np.sum(exp)
-
-        return output
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        print('add',self.input_shapes)
+        self.name = 'Add'
+        self.specific_operator = ' + '
+    
+    def forward_path_layer(self, inputs:np.ndarray):
+        if(self.constant is None):
+            constant = np.zeros(1)
+        else: 
+            constant = np.reshape(self.constant,self.input_shapes[-1][1:])
+            self.input_shapes = np.delete(self.input_shapes,-1,axis=0)
+        if(len(self.previous_layer) > 1):
+            output = np.zeros(self.input_shapes[0][1:])
+            for i in range(len(self.input_shapes)):
+                output += np.reshape(inputs[i],self.input_shapes[i][1:])
+        else:
+            output = np.reshape(inputs,self.input_shapes[0][1:])
+        out = self.activation_function.compute(output+constant)
+        return out
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,32 +81,37 @@
         if self.debug_mode:
             self.debug_target = self.load_debug_target(debug_mode)
         ##### Debug Mode #####
             
         ####### Checking the instantiation#######
 
         ### Checking argument type ###
-        assert type(self.file) == str or type(self.file) == onnx.ModelProto or type(self.file) == Functional or type(self.file) == Sequential
-        assert type(test_dataset) == str or type(test_dataset) == np.ndarray or test_dataset == None
-        assert type(self.test_dataset) == np.ndarray
-        assert type(self.function_name) == str
-        assert type(self.conv_algorithm) == str
-        assert self.debug_mode == None or type(self.debug_mode) == str
+        if not (type(self.file) == str or type(self.file) == onnx.ModelProto or type(self.file) == Functional or type(self.file) == Sequential):
+            raise TypeError("Error: model type.\n Format must be: path to model, model ONNX or model Keras")
+        if not (type(test_dataset) == str or type(test_dataset) == np.ndarray or test_dataset == None):
+            raise TypeError("Error: test_dataset type.\n Must be: path to dataset text filen, numpy array or None")
+        if not type(self.function_name) == str:
+            raise TypeError("Error: function name type.\n Must be a string")
+        if not type(self.conv_algorithm) == str:
+            raise TypeError("Error: conv algorihtm type.\n Must be a string")
+        if not (self.debug_mode == None or type(self.debug_mode) == str):
+            raise TypeError("Error: debug mode type.\n Must be: string or None")
         if self.debug_mode:
             assert type(self.debug_target) == list
 
         ### Checking value consistency ###
-        assert self.conv_algorithm in ['6loops',
+        if self.conv_algorithm not in ['6loops',
                                        'indirect_gemm_nn','indirect_gemm_tn','indirect_gemm_nt','indirect_gemm_tt',
-                                       'std_gemm_nn','std_gemm_tn','std_gemm_nt','std_gemm_']
+                                       'std_gemm_nn','std_gemm_tn','std_gemm_nt','std_gemm_tt']:
+            raise ValueError("Error: conv algorithm value.\n Must be one of: 6loops, indirect_gemm_nn, indirect_gemm_tn, indirect_gemm_nt, indirect_gemm_tt, std_gemm_nn, std_gemm_tn, std_gemm_nt, std_gemm_tt")
+        
         ##### Debug Mode #####
         if self.debug_mode:
-            assert self.debug_mode in ['keras','onnx']
-            assert len(self.debug_target) <= len(self.layers)
-            assert all(target <= len(self.layers) for target in self.debug_target)
+            if self.debug_mode not in ['keras','onnx']:
+                raise ValueError("Error: debug mode value.\n Must be one of: keras, onnx")
         ##### Debug Mode #####
     
     def load_debug_target(self, debug_mode:str|None):
         targets = []
         for layer in self.layers[1:]:
             if debug_mode == 'keras' and layer.name == 'Softmax':
                 targets[-1] = layer.idx
@@ -210,16 +215,14 @@
                         # Add the inference result of the layer to debug_output
                         if layer.name != 'Input_layer':
                             if layer.idx in self.debug_target:
                                 debug_output.append(previous_layer_result[layer.path])
                                 if((self.data_format == 'channels_last') and hasattr(layer, 'output_channels')): debug_output[-1] = np.transpose(debug_output[-1], (1,2,0))
                                 debug_output[-1] = debug_output[-1].flatten()
 
-                        # If all the targets are saved, the inference is stopped and the result is given
-                        if len(debug_output) == len(self.debug_target):
                             targets.append(str(layer.name) + " " + str(layer.idx))
                     ##### Debug Mode #####
                         
                 nn_output = previous_layer_result[layer.path]
                 # print(nn_output) # write to file instead
                 
                 # Write results in text files to compare prediction.
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/debug_tools/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/debug_tools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,17 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from .debug_keras import debug_keras, run_model_keras
+from .debug_keras import debug_keras
 
-from .debug_onnx import debug_onnx, run_model_onnx
+from .debug_onnx import debug_onnx
 
 from .debug_tools import compare_result, extract_outputs_c, extract_outputs_python
 
 __all__ = (
-    "debug_keras","run_model_keras",
-    "debug_onnx", "run_model_onnx",
+    "debug_keras", "debug_onnx",
     "compare_result", "extract_outputs_c", "extract_outputs_python"
 )
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/debug_tools/debug_keras.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/debug_tools/debug_keras.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,28 +20,25 @@
 
 import keras
 from keras.engine.functional import Functional
 from keras.engine.sequential import Sequential
 import numpy as np
 
 def extract_node_outputs(model:Sequential|Functional):
-    ouputs_name = []
-    for layer in model.layers:
-        ouputs_name.append(model.get_layer(layer.name).output[0])
-    return ouputs_name
+    return [layer.output for layer in model.layers[1:]]
 
 def extract_targets_indices(model:Functional|Sequential,outputs_name:list[str]):
     targets_indices = []
     for name in outputs_name:
         for i in range(len(model.layers)):
             if model.layers[i].output[0] == name:
                 targets_indices.append(i)
     return targets_indices
 
-def debug_keras(target_model:Sequential|Functional|str, debug_target:list=[], to_save:bool = False, path:str = ''):
+def debug_keras(target_model:Sequential|Functional|str, dataset:np.ndarray, debug_target:list=[], to_save:bool = False, path:str = ''):
     # Loading the model
     if(type(target_model) == str): 
         model = keras.models.load_model(target_model)
     else:
         model = target_model
 
     # Tensor output name and inidce for acetone debug
@@ -49,22 +46,21 @@
         inter_layers = extract_node_outputs(model)
         targets_indices = []
     else:
         inter_layers = debug_target
         targets_indices = extract_targets_indices(model, inter_layers)
     
     # Add an output after each name of inter_layers
-    model = keras.Model(inputs=model.input, outputs=inter_layers)
+    functional = [Functional([model.input],[out]) for out in inter_layers]
 
     # Saving the model
     if to_save:
-        keras.models.save_model(model, path)
-    
-    return model, targets_indices
+        for i in range(len(functional)):
+            keras.models.save_model(model, path+"model_"+str(i)+".h5")
+
+    # Model inference
+    outputs = [func([dataset]) for func in functional]
 
-def run_model_keras(target_model:Sequential|Functional, dataset:np.ndarray):
-    keras_result = target_model.predict(dataset)
+    for i in range(len(outputs)):
+        outputs[i] = outputs[i].ravel().flatten()
 
-    for i in range(len(keras_result)):
-        keras_result[i] = keras_result[i].ravel().flatten()
-        
-    return keras_result
+    return model, targets_indices, outputs
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/debug_tools/debug_onnx.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/debug_tools/debug_onnx.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,27 @@
     targets_indices = []
     for name in outputs_name:
         for i in range(len(model.graph.node)):
             if model.graph.node[i].output[0] == name:
                 targets_indices.append(i)
     return targets_indices
 
-def debug_onnx(target_model:onnx.ModelProto|str, debug_target:list=[], otpimize_inputs:bool = False, to_save:bool = False, path:str = ''):
+def run_model_onnx(model:onnx.ModelProto, dataset:np.ndarray):
+    sess = rt.InferenceSession(model)
+    input_name = sess.get_inputs()[0].name
+    onnx_result = sess.run(None,{input_name: dataset})
+
+    onnx_result.append(onnx_result.pop(0))
+    
+    for i in range(len(onnx_result)):
+        onnx_result[i] = onnx_result[i].ravel().flatten()
+    
+    return onnx_result
+
+def debug_onnx(target_model:onnx.ModelProto|str, dataset:np.ndarray, debug_target:list=[], otpimize_inputs:bool = False, to_save:bool = False, path:str = ''):
     # Loading the model
     if type(target_model) == str:
         model = onnx.load(target_model)
     else:
         model = target_model
 
     # Tensor output name and inidce for acetone debug
@@ -60,38 +72,25 @@
         targets_indices = extract_targets_indices(model, inter_layers)
 
     # Add an output after each name of inter_layers
     value_info_protos = []
     shape_info = onnx.shape_inference.infer_shapes(model)
     for idx, node in enumerate(shape_info.graph.value_info):
         if node.name in inter_layers:
-            print(idx, node)
             value_info_protos.append(node)
     assert len(value_info_protos) == len(inter_layers)
     model.graph.output.extend(value_info_protos)  #  in inference stage, these tensor will be added to output dict.
 
     # Optimizing the model by removing the useless inputs
     if otpimize_inputs:
         clean_inputs(model)
     
     onnx.checker.check_model(model)
 
     # Save the model
     if to_save:
         onnx.save(model,path)
-    
-    return model, targets_indices
-
-def run_model_onnx(model:onnx.ModelProto, dataset:np.ndarray, keep_full_model_result:bool = True):
-    sess = rt.InferenceSession(model)
-    input_name = sess.get_inputs()[0].name
-    onnx_result = sess.run(None,{input_name: dataset})
 
-    if not keep_full_model_result:
-        onnx_result.pop(0)
-    else:
-        onnx_result.append(onnx_result.pop(0))
-    
-    for i in range(len(onnx_result)):
-        onnx_result[i] = onnx_result[i].ravel().flatten()
+    # Model inference
+    outputs = run_model_onnx(model, dataset)
     
-    return onnx_result
+    return model, targets_indices, outputs
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/debug_tools/debug_tools.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/debug_tools/debug_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return False
     
     correct = True
     for i in range(len(acetone_result)):
         print('--------------------------------------------')
         print('Comparing',targets[i])
         try:
-            np.testing.assert_allclose(acetone_result[i],reference_result[i],atol=1e-06)
+            np.testing.assert_allclose(acetone_result[i],reference_result[i],atol=1e-06,rtol=1e-06)
         except AssertionError as msg:
             print("Error: output value of",targets[i],"incorrect")
             correct = False
             if verbose:
                 print(msg)
         print('--------------------------------------------')
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,16 @@
             
         l_temp = current_layer
         layers.append(l_temp)
 
         if add_softmax_layer:
             nb_softmax_layers += 1
             current_layer = Softmax(idx = idx+1,
-                                    size = l_temp.size)
+                                    size = l_temp.size,
+                                    axis = None)
             l_temp.next_layer.append(current_layer)
             current_layer.previous_layer.append(l_temp)
             l_temp = current_layer
             layers.append(l_temp)
         
     layers, listRoad, maxRoad, dict_cst = graph_interpretor.tri_topo(layers)
     layers = list(map(lambda x:x.find_output_str(dict_cst), layers))
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
 
         l_temp = current_layer
         layers.append(current_layer)
 
         # Separeted method to generate softmax
         if add_softmax_layer:
             nb_softmax_layers += 1
-            current_layer = Softmax(idx+1, l_temp.size)
+            current_layer = Softmax(idx+1, l_temp.size, None)
             l_temp.next_layer.append(current_layer)
             current_layer.previous_layer.append(l_temp)
             l_temp = current_layer
             layers.append(current_layer)
 
     layers, listRoad, maxRoad, dict_cst = graph_interpretor.tri_topo(layers)
     layers = list(map(lambda x:x.find_output_str(dict_cst), layers))
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,20 @@
 
 #Create a layer Softmax
 def create_Softmax(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
+    attributs = extract_attribut(node)
+    if 'axis' not in attributs:
+        attributs['axis'] = -1
     return Softmax(idx = idx,
-                            size = size)
+                    size = size,
+                    axis = attributs['axis'])
 
 
 #Create a layer Conv
 def create_Conv(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto, conv_algorithm:str):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
@@ -624,30 +628,30 @@
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     return Maximum(idx=idx,
                     size=size,
-                    input_shapes=input_shapes,
+                    input_shapes=np.array(input_shapes),
                     output_shape=output_shape,
                     activation_function= Linear())
 
 #create a layer Min
 def create_Min(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     return Minimum(idx=idx,
                     size=size,
-                    input_shapes=input_shapes,
+                    input_shapes=np.array(input_shapes),
                     output_shape=output_shape,
                     activation_function= Linear())
 
 #create a layer Average
 def create_Avg(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shapes =[]
     for input in node.input:
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.3
+Version: 0.3.1.dev1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.3/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.3.1.dev1/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*


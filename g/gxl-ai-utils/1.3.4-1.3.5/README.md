# Comparing `tmp/gxl_ai_utils-1.3.4.tar.gz` & `tmp/gxl_ai_utils-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxl_ai_utils-1.3.4.tar", last modified: Mon Apr  8 18:32:05 2024, max compression
+gzip compressed data, was "gxl_ai_utils-1.3.5.tar", last modified: Fri May 24 06:49:47 2024, max compression
```

## Comparing `gxl_ai_utils-1.3.4.tar` & `gxl_ai_utils-1.3.5.tar`

### file list

```diff
@@ -1,513 +1,645 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.131513 gxl_ai_utils-1.3.4/
--rw-rw-rw-   0        0        0      211 2024-04-08 18:32:05.129115 gxl_ai_utils-1.3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.064387 gxl_ai_utils-1.3.4/eggs/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.067226 gxl_ai_utils-1.3.4/eggs/aishell/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/aishell/__init__.py
--rw-rw-rw-   0        0        0      238 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/aishell/do_infer.py
--rw-rw-rw-   0        0        0     1262 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/aishell/do_train.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.069220 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.077203 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/punctuation/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/punctuation/__init__.py
--rw-rw-rw-   0        0        0     5134 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/punctuation/punctuation.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.085177 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/__init__.py
--rw-rw-rw-   0        0        0     1002 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_gigaspeech.py
--rw-rw-rw-   0        0        0      693 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_haoweilai.py
--rw-rw-rw-   0        0        0     1316 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_librispeech.py
--rw-rw-rw-   0        0        0     1037 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_mls.py
--rw-rw-rw-   0        0        0     1702 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/make_shard.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.091161 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.105525 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.110176 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/__init__.py
--rw-rw-rw-   0        0        0    19681 2024-03-29 09:02:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.113176 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/__init__.py
--rw-rw-rw-   0        0        0    21823 2024-03-29 09:10:36.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.116160 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/__init__.py
--rw-rw-rw-   0        0        0    19582 2024-04-01 05:17:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.122144 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/__init__.py
--rw-rw-rw-   0        0        0    19589 2024-04-01 05:17:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.126136 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/__init__.py
--rw-rw-rw-   0        0        0    22007 2024-03-29 09:10:36.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.129125 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/__init__.py
--rw-rw-rw-   0        0        0    15667 2024-03-29 09:02:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.131120 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/__init__.py
--rw-rw-rw-   0        0        0    23624 2024-03-29 09:02:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.138100 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/__init__.py
--rw-rw-rw-   0        0        0    19465 2024-03-23 15:34:56.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.142091 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/
--rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/__init__.py
--rw-rw-rw-   0        0        0    21395 2024-03-26 06:24:07.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/do_handle.py
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.144085 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/
--rw-rw-rw-   0        0        0        0 2024-03-17 07:29:51.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/__init__.py
--rw-rw-rw-   0        0        0    17684 2024-03-17 08:35:12.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/do_handle.py
--rw-rw-rw-   0        0        0    25266 2024-02-29 05:24:42.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle.py
--rw-rw-rw-   0        0        0    25267 2024-03-09 13:06:04.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-1.py
--rw-rw-rw-   0        0        0    24364 2024-03-05 08:12:26.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-2.py
--rw-rw-rw-   0        0        0    26215 2024-02-29 05:24:42.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4redian.py
--rw-rw-rw-   0        0        0     2878 2024-03-23 18:03:36.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_remove.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.149071 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/
--rw-rw-rw-   0        0        0        0 2024-03-26 08:17:34.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/__init__.py
--rw-rw-rw-   0        0        0    10187 2024-04-01 05:17:50.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/common_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.156230 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/
--rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/__init__.py
--rw-rw-rw-   0        0        0    17693 2024-03-17 09:27:53.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.160043 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/
--rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/__init__.py
--rw-rw-rw-   0        0        0    17721 2024-03-17 09:57:21.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/do_handle.py
--rw-rw-rw-   0        0        0     1053 2024-04-01 05:20:49.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/make_shard.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.164106 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/__init__.py
--rw-rw-rw-   0        0        0    18376 2024-03-18 06:39:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.171046 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/__init__.py
--rw-rw-rw-   0        0        0    18374 2024-03-17 08:50:53.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.174005 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/__init__.py
--rw-rw-rw-   0        0        0    18529 2024-03-17 04:31:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.178205 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/__init__.py
--rw-rw-rw-   0        0        0    18757 2024-03-17 04:31:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.181984 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/__init__.py
--rw-rw-rw-   0        0        0    17630 2024-03-18 06:55:25.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.188061 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/__init__.py
--rw-rw-rw-   0        0        0    20020 2024-03-17 04:31:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.191013 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/
--rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/__init__.py
--rw-rw-rw-   0        0        0    17748 2024-03-17 10:02:42.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/do_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.196944 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/
--rw-rw-rw-   0        0        0        0 2024-03-26 11:48:19.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/__init__.py
--rw-rw-rw-   0        0        0     5564 2024-04-08 17:21:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/compute_fbank_common.py
--rw-rw-rw-   0        0        0    11494 2024-04-02 02:44:33.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/icefall_assistant.py
--rw-rw-rw-   0        0        0        0 2024-03-27 06:22:09.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zip_trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.317709 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/
--rw-rw-rw-   0        0        0        0 2024-03-27 06:19:27.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/__init__.py
--rw-rw-rw-   0        0        0    13605 2024-03-27 07:54:26.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/asr_datamodule.py
--rw-rw-rw-   0        0        0   109372 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/beam_search.py
--rw-rw-rw-   0        0        0    27050 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decode.py
--rw-rw-rw-   0        0        0    27656 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_bbpe.py
--rw-rw-rw-   0        0        0     5331 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_stream.py
--rw-rw-rw-   0        0        0     4755 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decoder.py
--rw-rw-rw-   0        0        0     1652 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/encoder_interface.py
--rw-rw-rw-   0        0        0    25164 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx-streaming.py
--rw-rw-rw-   0        0        0    18723 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx.py
--rw-rw-rw-   0        0        0    17410 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/export.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.376497 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/
--rw-rw-rw-   0        0        0     1402 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/__init__.py
--rw-rw-rw-   0        0        0     4780 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ali.py
--rw-rw-rw-   0        0        0     2991 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/bpe_graph_compiler.py
--rw-rw-rw-   0        0        0     4044 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/byte_utils.py
--rw-rw-rw-   0        0        0     3436 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/char_graph_compiler.py
--rw-rw-rw-   0        0        0    15166 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/checkpoint.py
--rw-rw-rw-   0        0        0    22548 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/context_graph.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.389310 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/
--rw-rw-rw-   0        0        0      187 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/__init__.py
--rw-rw-rw-   0        0        0     9561 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/prepare_lang.py
--rw-rw-rw-   0        0        0     3868 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_ctc_topo.py
--rw-rw-rw-   0        0        0     1100 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_prepare_lang.py
--rw-rw-rw-   0        0        0     4628 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/topo.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.393355 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/
--rw-rw-rw-   0        0        0        0 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/__init__.py
--rw-rw-rw-   0        0        0     2002 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/datamodule.py
--rw-rw-rw-   0        0        0    44213 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/decode.py
--rw-rw-rw-   0        0        0    27288 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/diagnostics.py
--rw-rw-rw-   0        0        0     1966 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dist.py
--rw-rw-rw-   0        0        0     3472 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/env.py
--rw-rw-rw-   0        0        0     5508 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/graph_compiler.py
--rw-rw-rw-   0        0        0     3580 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/hooks.py
--rw-rw-rw-   0        0        0     8723 2024-03-28 08:19:43.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lexicon.py
--rw-rw-rw-   0        0        0     7821 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lm_wrapper.py
--rw-rw-rw-   0        0        0     6644 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi.py
--rw-rw-rw-   0        0        0     7859 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi_graph_compiler.py
--rw-rw-rw-   0        0        0     5295 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ngram_lm.py
--rw-rw-rw-   0        0        0     8205 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/otc_graph_compiler.py
--rw-rw-rw-   0        0        0    30754 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/profiler.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.421758 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/
--rw-rw-rw-   0        0        0        0 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/__init__.py
--rw-rw-rw-   0        0        0     3644 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx-streaming.py
--rw-rw-rw-   0        0        0     3205 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx.py
--rw-rw-rw-   0        0        0     7275 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/compute_perplexity.py
--rw-rw-rw-   0        0        0     7647 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/dataset.py
--rw-rw-rw-   0        0        0    11547 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export-onnx.py
--rw-rw-rw-   0        0        0     5747 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export.py
--rw-rw-rw-   0        0        0    10312 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/model.py
--rw-rw-rw-   0        0        0     2238 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset.py
--rw-rw-rw-   0        0        0     2977 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset_ddp.py
--rw-rw-rw-   0        0        0     1842 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_model.py
--rw-rw-rw-   0        0        0    19664 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/train.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.443469 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/
--rw-rw-rw-   0        0        0        0 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/__init__.py
--rw-rw-rw-   0        0        0    22349 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/attention.py
--rw-rw-rw-   0        0        0     5497 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/compute_perplexity.py
--rw-rw-rw-   0        0        0       20 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/dataset.py
--rw-rw-rw-   0        0        0    11234 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/encoder.py
--rw-rw-rw-   0        0        0     4925 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/export.py
--rw-rw-rw-   0        0        0     3396 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/model.py
--rw-rw-rw-   0        0        0       65 2024-02-26 01:52:00.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/scaling.py
--rw-rw-rw-   0        0        0    17243 2024-02-26 01:52:00.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/train.py
--rw-rw-rw-   0        0        0    76655 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/utils.py
--rw-rw-rw-   0        0        0     7709 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained.py
--rw-rw-rw-   0        0        0     7751 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_bbpe.py
--rw-rw-rw-   0        0        0     8146 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_streaming.py
--rw-rw-rw-   0        0        0     2214 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/joiner.py
--rw-rw-rw-   0        0        0    12993 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/model.py
--rw-rw-rw-   0        0        0     7152 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_check.py
--rw-rw-rw-   0        0        0     8300 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_decode.py
--rw-rw-rw-   0        0        0    17464 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained-streaming.py
--rw-rw-rw-   0        0        0    12357 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained.py
--rw-rw-rw-   0        0        0    50893 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/optim.py
--rw-rw-rw-   0        0        0    10603 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained.py
--rw-rw-rw-   0        0        0    11561 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained_bbpe.py
--rw-rw-rw-   0        0        0    70696 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling.py
--rw-rw-rw-   0        0        0     3342 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling_converter.py
--rw-rw-rw-   0        0        0     9817 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_beam_search.py
--rw-rw-rw-   0        0        0    30030 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_decode.py
--rw-rw-rw-   0        0        0    13138 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/subsampling.py
--rw-rw-rw-   0        0        0    43330 2024-03-27 07:55:21.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/train.py
--rw-rw-rw-   0        0        0    29572 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/train_bbpe.py
--rw-rw-rw-   0        0        0    92936 2024-03-27 06:19:30.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/zipformer.py
--rw-rw-rw-   0        0        0       88 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.459484 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/__init__.py
--rw-rw-rw-   0        0        0     5838 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/handle_peoplespeech.py
--rw-rw-rw-   0        0        0     9569 2024-02-22 05:44:59.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.461370 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/
--rw-rw-rw-   0        0        0        0 2024-04-07 06:18:22.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/__init__.py
--rw-rw-rw-   0        0        0      962 2024-02-25 03:33:09.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/make_shard4new_wenetspeech.py
--rw-rw-rw-   0        0        0     1186 2024-03-26 14:51:25.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/shard_from_pachong.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.467391 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_fairseq/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_fairseq/__init__.py
--rw-rw-rw-   0        0        0    13907 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_fairseq/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.482315 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/__init__.py
--rw-rw-rw-   0        0        0    20570 2024-03-27 10:48:34.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/compute-wer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.485359 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/__init__.py
--rw-rw-rw-   0        0        0     1582 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/main.py
--rw-rw-rw-   0        0        0     1931 2024-03-27 10:57:29.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/handle4accent.py
--rw-rw-rw-   0        0        0     6851 2024-02-22 07:15:14.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/main.py
--rw-rw-rw-   0        0        0     2000 2024-04-07 05:51:36.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/prepare_data4prompt_task.py
--rw-rw-rw-   0        0        0     3385 2024-03-17 16:49:11.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/speechio_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.489295 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_TYPE_CHECKING/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_TYPE_CHECKING/__init__.py
--rw-rw-rw-   0        0        0      256 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_TYPE_CHECKING/fun.py
--rw-rw-rw-   0        0        0      125 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_TYPE_CHECKING/test.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.503821 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/__init__.py
--rw-rw-rw-   0        0        0      232 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/download_test.py
--rw-rw-rw-   0        0        0      793 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/format_test.py
--rw-rw-rw-   0        0        0      503 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/gxl_test.py
--rw-rw-rw-   0        0        0      746 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/main.py
--rw-rw-rw-   0        0        0      400 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/test.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.506815 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_sentencepiece/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_sentencepiece/__init__.py
--rw-rw-rw-   0        0        0     1781 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_sentencepiece/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.511863 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/ximalaya/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/ximalaya/__init__.py
--rw-rw-rw-   0        0        0     2525 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/cats_and_dogs/ximalaya/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.514796 gxl_ai_utils-1.3.4/eggs/ch_en_mix/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/ch_en_mix/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.516786 gxl_ai_utils-1.3.4/eggs/ch_en_mix/data_handle/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/ch_en_mix/data_handle/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.521774 gxl_ai_utils-1.3.4/eggs/finetune_llm/
--rw-rw-rw-   0        0        0        0 2024-02-29 06:01:16.000000 gxl_ai_utils-1.3.4/eggs/finetune_llm/__init__.py
--rw-rw-rw-   0        0        0      928 2024-03-13 02:52:18.000000 gxl_ai_utils-1.3.4/eggs/finetune_llm/main.py
--rw-rw-rw-   0        0        0     1858 2024-03-13 07:52:36.000000 gxl_ai_utils-1.3.4/eggs/finetune_llm/main_2B.py
--rw-rw-rw-   0        0        0     1367 2024-03-13 07:36:12.000000 gxl_ai_utils-1.3.4/eggs/finetune_llm/transformers_learning.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.534794 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/__init__.py
--rw-rw-rw-   0        0        0     1635 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_knowledge_distill.py
--rw-rw-rw-   0        0        0     1129 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_paraformer_infer.py
--rw-rw-rw-   0        0        0     2469 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_whisper_infer.py
--rw-rw-rw-   0        0        0     1090 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/handle_cmvn_gxl.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.540203 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/decoder.py
--rw-rw-rw-   0        0        0    27385 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/encoder.py
--rw-rw-rw-   0        0        0      827 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer_infer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.547122 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/whisper_ctc/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/whisper_ctc/__init__.py
--rw-rw-rw-   0        0        0      741 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/knowledge_distillation/whisper_ctc/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.572638 gxl_ai_utils-1.3.4/eggs/spider/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/__init__.py
--rw-rw-rw-   0        0        0      382 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spdier_little_url_get.py
--rw-rw-rw-   0        0        0     9274 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_lizhi_fm.py
--rw-rw-rw-   0        0        0     5810 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_qingting_fm.py
--rw-rw-rw-   0        0        0    16395 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_qingting_fm_new.py
--rw-rw-rw-   0        0        0    24924 2024-04-07 10:46:48.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_voicewiki.py
--rw-rw-rw-   0        0        0    14467 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_ximalaya.py
--rw-rw-rw-   0        0        0    10475 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_ximalaya_new.py
--rw-rw-rw-   0        0        0     7041 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_yunting.py
--rw-rw-rw-   0        0        0     4983 2024-02-25 08:28:39.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_zhihu.py
--rw-rw-rw-   0        0        0     4770 2024-02-25 08:26:09.000000 gxl_ai_utils-1.3.4/eggs/spider/spider_zhihu_2.py
--rw-rw-rw-   0        0        0     3479 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/eggs/spider/test.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.582661 gxl_ai_utils-1.3.4/gxl_ai_utils/
--rw-rw-rw-   0        0        0     1651 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/AiConstant.py
--rw-rw-rw-   0        0        0      556 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.619558 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/
--rw-rw-rw-   0        0        0       35 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/__init__.py
--rw-rw-rw-   0        0        0    14863 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/build_vocab.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.628010 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/classify/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/classify/__init__.py
--rw-rw-rw-   0        0        0     5401 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/classify/data_handler.py
--rw-rw-rw-   0        0        0     6562 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/common_data_handler.py
--rw-rw-rw-   0        0        0     6242 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/gxl_data_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.630485 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/recognition/
--rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/recognition/__init__.py
--rw-rw-rw-   0        0        0    10901 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/recognition/data_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.632511 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_handler/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.633954 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/
--rw-rw-rw-   0        0        0       36 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.643326 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/__init__.py
--rw-rw-rw-   0        0        0    17914 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/ecapa_tdnn.py
--rw-rw-rw-   0        0        0    27764 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/xvector.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.646138 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/
--rw-rw-rw-   0        0        0       50 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.649936 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/deepspeech2/
--rw-rw-rw-   0        0        0       25 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/deepspeech2/__init__.py
--rw-rw-rw-   0        0        0    14593 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/deepspeech2/deepspeech2.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.663036 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/__init__.py
--rw-rw-rw-   0        0        0     6869 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/ctc_decoder.py
--rw-rw-rw-   0        0        0     5452 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/embedding.py
--rw-rw-rw-   0        0        0     8872 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/subsampling.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.667120 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.683889 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.700842 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/__init__.py
--rw-rw-rw-   0        0        0     1942 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/multi_head_attention.py
--rw-rw-rw-   0        0        0     1662 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_encoding.py
--rw-rw-rw-   0        0        0      936 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_wise_feed_forward.py
--rw-rw-rw-   0        0        0     1193 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/scaled_dot_product_attention.py
--rw-rw-rw-   0        0        0     3050 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/decoder.py
--rw-rw-rw-   0        0        0     2386 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/encoder.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.709824 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/__init__.py
--rw-rw-rw-   0        0        0      569 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/padding_mask.py
--rw-rw-rw-   0        0        0      427 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/sequence_mask.py
--rw-rw-rw-   0        0        0     1305 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.712820 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/utils/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/utils/__init__.py
--rw-rw-rw-   0        0        0    14807 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/utils/ctc_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.714830 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/t2s/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/t2s/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.722021 gxl_ai_utils-1.3.4/gxl_ai_utils/config/
--rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/config/__init__.py
--rw-rw-rw-   0        0        0     5179 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/config/gxl_config.py
--rw-rw-rw-   0        0        0      121 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.727866 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/
--rw-rw-rw-   0        0        0        2 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/__init__.py
--rw-rw-rw-   0        0        0     7429 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/gxl_dataset.py
--rw-rw-rw-   0        0        0    18215 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/gxl_processor.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.744901 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/__init__.py
--rw-rw-rw-   0        0        0    10270 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/alignment.py
--rw-rw-rw-   0        0        0     3616 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/average_model.py
--rw-rw-rw-   0        0        0     5604 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/gxl_infer.py
--rw-rw-rw-   0        0        0    12155 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/recognize.py
--rw-rw-rw-   0        0        0    12797 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/recognize_onnx_gpu.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.751783 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_lr_scheduler_wenet/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_lr_scheduler_wenet/__init__.py
--rw-rw-rw-   0        0        0    24245 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_lr_scheduler_wenet/scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.755778 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.761757 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/__init__.py
--rw-rw-rw-   0        0        0     6645 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/cgmlp.py
--rw-rw-rw-   0        0        0    16717 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/encoder.py
--rw-rw-rw-   0        0        0    10038 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/encoder_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.768743 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/cif/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/cif/__init__.py
--rw-rw-rw-   0        0        0    11275 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/cif/predictor.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.774724 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/__init__.py
--rw-rw-rw-   0        0        0    16682 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder.py
--rw-rw-rw-   0        0        0     6840 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.791678 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/__init__.py
--rw-rw-rw-   0        0        0    11117 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/attention.py
--rw-rw-rw-   0        0        0     5905 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/convolution.py
--rw-rw-rw-   0        0        0    26376 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder.py
--rw-rw-rw-   0        0        0     7093 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder_layer.py
--rw-rw-rw-   0        0        0     2749 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/subsampling.py
--rw-rw-rw-   0        0        0     7413 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/init_model.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.794669 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/k2/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/k2/__init__.py
--rw-rw-rw-   0        0        0    11851 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/k2/model.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.817608 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/__init__.py
--rw-rw-rw-   0        0        0     8230 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/attention.py
--rw-rw-rw-   0        0        0    11269 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/cif.py
--rw-rw-rw-   0        0        0     5301 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/convert_paraformer_to_wenet_config.py
--rw-rw-rw-   0        0        0    17521 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/layers.py
--rw-rw-rw-   0        0        0     9883 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/paraformer.py
--rw-rw-rw-   0        0        0     6945 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/search.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.838358 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/__init__.py
--rw-rw-rw-   0        0        0    10509 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/attention.py
--rw-rw-rw-   0        0        0     2636 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/conv2d.py
--rw-rw-rw-   0        0        0     6713 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/convolution.py
--rw-rw-rw-   0        0        0    22398 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder.py
--rw-rw-rw-   0        0        0     4833 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder_layer.py
--rw-rw-rw-   0        0        0     3067 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/positionwise_feed_forward.py
--rw-rw-rw-   0        0        0    11264 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/subsampling.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.848401 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/__init__.py
--rw-rw-rw-   0        0        0     4110 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/joint.py
--rw-rw-rw-   0        0        0    18089 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/predictor.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.853271 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/__init__.py
--rw-rw-rw-   0        0        0     2014 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/greedy_search.py
--rw-rw-rw-   0        0        0     6112 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/prefix_beam_search.py
--rw-rw-rw-   0        0        0    23241 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/transducer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.915216 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/__init__.py
--rw-rw-rw-   0        0        0    18961 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/asr_model.py
--rw-rw-rw-   0        0        0    14383 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/attention.py
--rw-rw-rw-   0        0        0     1533 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/cmvn.py
--rw-rw-rw-   0        0        0     5329 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/convolution.py
--rw-rw-rw-   0        0        0     3084 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/ctc.py
--rw-rw-rw-   0        0        0    12855 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/decoder.py
--rw-rw-rw-   0        0        0     4939 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/decoder_layer.py
--rw-rw-rw-   0        0        0     6339 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/embedding.py
--rw-rw-rw-   0        0        0    20622 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/encoder.py
--rw-rw-rw-   0        0        0     9838 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/encoder_layer.py
--rw-rw-rw-   0        0        0     3806 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/label_smoothing_loss.py
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/paraformer_encoder.py
--rw-rw-rw-   0        0        0     1940 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/positionwise_feed_forward.py
--rw-rw-rw-   0        0        0    18309 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/search.py
--rw-rw-rw-   0        0        0     9512 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/subsampling.py
--rw-rw-rw-   0        0        0     1029 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/swish.py
--rw-rw-rw-   0        0        0     6294 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_decoder.py
--rw-rw-rw-   0        0        0     8366 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder.py
--rw-rw-rw-   0        0        0     2582 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder_gxl.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.950126 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/__init__.py
--rw-rw-rw-   0        0        0     4018 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/checkpoint.py
--rw-rw-rw-   0        0        0     3065 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/cmvn.py
--rw-rw-rw-   0        0        0     7954 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/common.py
--rw-rw-rw-   0        0        0     1516 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/config.py
--rw-rw-rw-   0        0        0     9964 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/context_graph.py
--rw-rw-rw-   0        0        0     5411 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/ctc_utils.py
--rw-rw-rw-   0        0        0     4353 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/executor.py
--rw-rw-rw-   0        0        0     2168 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/file_utils.py
--rw-rw-rw-   0        0        0     1291 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/init_ali_paraformer.py
--rw-rw-rw-   0        0        0     7440 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/init_model.py
--rw-rw-rw-   0        0        0    13020 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/mask.py
--rw-rw-rw-   0        0        0    24245 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/scheduler.py
--rw-rw-rw-   0        0        0     1568 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/tokenize_utils.py
--rw-rw-rw-   0        0        0    26574 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/train_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.962079 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/__init__.py
--rw-rw-rw-   0        0        0    14805 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/attentions.py
--rw-rw-rw-   0        0        0     4860 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/commons.py
--rw-rw-rw-   0        0        0    24767 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/models.py
--rw-rw-rw-   0        0        0    16740 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/modules.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.967648 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_trainer_wenet/
--rw-rw-rw-   0        0        0       35 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_trainer_wenet/__init__.py
--rw-rw-rw-   0        0        0     9889 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_trainer_wenet/gxl_trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.992089 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/
--rw-rw-rw-   0        0        0     7061 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/__init__.py
--rw-rw-rw-   0        0        0       38 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/__main__.py
--rw-rw-rw-   0        0        0     5089 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/audio.py
--rw-rw-rw-   0        0        0    33001 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/decoding.py
--rw-rw-rw-   0        0        0    11165 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/model.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.001099 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/
--rw-rw-rw-   0        0        0      132 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/__init__.py
--rw-rw-rw-   0        0        0     2012 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/basic.py
--rw-rw-rw-   0        0        0    21418 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/english.py
--rw-rw-rw-   0        0        0    12968 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/timing.py
--rw-rw-rw-   0        0        0    12733 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/tokenizer.py
--rw-rw-rw-   0        0        0    23334 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/transcribe.py
--rw-rw-rw-   0        0        0     3583 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/triton_ops.py
--rw-rw-rw-   0        0        0    11363 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/utils.py
--rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/version.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.006040 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.008062 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.012023 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/__init__.py
--rw-rw-rw-   0        0        0      414 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/abs_encoder.py
--rw-rw-rw-   0        0        0     9977 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/conformer_encoder.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.017584 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/fastformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/fastformer/__init__.py
--rw-rw-rw-   0        0        0     2297 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/fastformer/fastformer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.027279 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/__init__.py
--rw-rw-rw-   0        0        0    19543 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/build_asr_model.py
--rw-rw-rw-   0        0        0   102558 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/e2e_asr_paraformer.py
--rw-rw-rw-   0        0        0    79092 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/sanm_decoder.py
--rw-rw-rw-   0        0        0    58681 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/sanm_encoder.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.039246 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/__init__.py
--rw-rw-rw-   0        0        0     6478 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/component.py
--rw-rw-rw-   0        0        0     2953 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/decoder.py
--rw-rw-rw-   0        0        0     2299 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/encoder.py
--rw-rw-rw-   0        0        0     1405 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.052051 gxl_ai_utils-1.3.4/gxl_ai_utils/run/
--rw-rw-rw-   0        0        0       22 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/__init__.py
--rw-rw-rw-   0        0        0     9326 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/base_train_runner.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.057051 gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/__init__.py
--rw-rw-rw-   0        0        0     1061 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/flask_predict.py
--rw-rw-rw-   0        0        0     4263 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/flask_server.py
--rw-rw-rw-   0        0        0     3023 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner.py
--rw-rw-rw-   0        0        0     2602 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner_multi_template.py
--rw-rw-rw-   0        0        0      593 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner_single_template.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.067429 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/
--rw-rw-rw-   0        0        0       76 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/__init__.py
--rw-rw-rw-   0        0        0     4311 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_data.py
--rw-rw-rw-   0        0        0      177 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_data_name.py
--rw-rw-rw-   0        0        0      451 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataloader.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.071000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataset/
--rw-rw-rw-   0        0        0       29 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataset/__init__.py
--rw-rw-rw-   0        0        0     5238 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataset/store_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.076984 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/
--rw-rw-rw-   0        0        0       64 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/__init__.py
--rw-rw-rw-   0        0        0     2072 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.096930 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/
--rw-rw-rw-   0        0        0       33 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/__init__.py
--rw-rw-rw-   0        0        0     6223 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/attention_model.py
--rw-rw-rw-   0        0        0     2438 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/cnn_model.py
--rw-rw-rw-   0        0        0      958 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/mlp_model.py
--rw-rw-rw-   0        0        0     2130 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/rnn_model.py
--rw-rw-rw-   0        0        0     2348 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/store_model_class.py
--rw-rw-rw-   0        0        0      578 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_name.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.100935 gxl_ai_utils-1.3.4/gxl_ai_utils/thread/
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/thread/__init__.py
--rw-rw-rw-   0        0        0     1522 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/thread/my_thread.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:05.126851 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/
--rw-rw-rw-   0        0        0       80 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_coding.py
--rw-rw-rw-   0        0        0    26855 2024-03-27 07:04:56.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_data.py
--rw-rw-rw-   0        0        0      423 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_device.py
--rw-rw-rw-   0        0        0    53528 2024-04-08 18:27:59.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_file.py
--rw-rw-rw-   0        0        0     6520 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_model.py
--rw-rw-rw-   0        0        0     1655 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_showing.py
--rw-rw-rw-   0        0        0     6747 2024-03-24 18:40:27.000000 gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_spider.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:32:04.605550 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/
--rw-rw-rw-   0        0        0      211 2024-04-08 18:32:03.000000 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    22460 2024-04-08 18:32:03.000000 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 18:32:03.000000 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-08 18:32:03.000000 gxl_ai_utils-1.3.4/gxl_ai_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      592 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.4/license.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 18:32:05.131967 gxl_ai_utils-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      518 2024-04-08 18:31:17.000000 gxl_ai_utils-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.201582 gxl_ai_utils-1.3.5/
+-rw-rw-rw-   0        0        0      212 2024-05-24 06:49:47.201582 gxl_ai_utils-1.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.570830 gxl_ai_utils-1.3.5/eggs/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.572824 gxl_ai_utils-1.3.5/eggs/aishell/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/aishell/__init__.py
+-rw-rw-rw-   0        0        0      238 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/aishell/do_infer.py
+-rw-rw-rw-   0        0        0     1262 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/aishell/do_train.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.573821 gxl_ai_utils-1.3.5/eggs/asr_handle_to_tts_mode/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/asr_handle_to_tts_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.574818 gxl_ai_utils-1.3.5/eggs/asr_handle_to_tts_mode/punctuation/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/asr_handle_to_tts_mode/punctuation/__init__.py
+-rw-rw-rw-   0        0        0     5134 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/asr_handle_to_tts_mode/punctuation/punctuation.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.581478 gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/__init__.py
+-rw-rw-rw-   0        0        0     1002 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/handle_gigaspeech.py
+-rw-rw-rw-   0        0        0      693 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/handle_haoweilai.py
+-rw-rw-rw-   0        0        0     1316 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/handle_librispeech.py
+-rw-rw-rw-   0        0        0     1037 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/handle_mls.py
+-rw-rw-rw-   0        0        0     1702 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/make_shard.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.585483 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.591194 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.592500 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/__init__.py
+-rw-rw-rw-   0        0        0    19681 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.593628 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/__init__.py
+-rw-rw-rw-   0        0        0    21823 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.596994 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/__init__.py
+-rw-rw-rw-   0        0        0    19582 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.599111 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/__init__.py
+-rw-rw-rw-   0        0        0    19589 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.601641 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/__init__.py
+-rw-rw-rw-   0        0        0    22007 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.602995 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/__init__.py
+-rw-rw-rw-   0        0        0    15667 2024-03-29 09:02:50.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.604016 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/__init__.py
+-rw-rw-rw-   0        0        0    23624 2024-03-29 09:02:50.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.605058 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/__init__.py
+-rw-rw-rw-   0        0        0    19465 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.606075 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/
+-rw-rw-rw-   0        0        0        0 2024-03-17 03:19:03.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/__init__.py
+-rw-rw-rw-   0        0        0    21395 2024-03-26 06:24:07.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/do_handle.py
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.607274 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/
+-rw-rw-rw-   0        0        0        0 2024-03-17 07:29:51.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/__init__.py
+-rw-rw-rw-   0        0        0    17684 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/do_handle.py
+-rw-rw-rw-   0        0        0    25266 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle.py
+-rw-rw-rw-   0        0        0    25267 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-1.py
+-rw-rw-rw-   0        0        0    24364 2024-05-06 09:10:01.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-2.py
+-rw-rw-rw-   0        0        0    26215 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4redian.py
+-rw-rw-rw-   0        0        0     2878 2024-03-23 18:03:36.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_remove.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.608599 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/
+-rw-rw-rw-   0        0        0        0 2024-03-26 08:17:34.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/__init__.py
+-rw-rw-rw-   0        0        0    10187 2024-04-01 05:17:50.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/common_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.609705 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/__init__.py
+-rw-rw-rw-   0        0        0    17693 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.610758 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/__init__.py
+-rw-rw-rw-   0        0        0    17721 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/do_handle.py
+-rw-rw-rw-   0        0        0     1053 2024-04-01 05:20:49.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/make_shard.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.612839 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/__init__.py
+-rw-rw-rw-   0        0        0    18376 2024-03-18 06:39:10.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.617160 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/__init__.py
+-rw-rw-rw-   0        0        0    18374 2024-03-17 08:50:53.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.618490 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/__init__.py
+-rw-rw-rw-   0        0        0    18529 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.619505 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/__init__.py
+-rw-rw-rw-   0        0        0    18757 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.620982 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/__init__.py
+-rw-rw-rw-   0        0        0    17630 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.621984 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:43:10.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/__init__.py
+-rw-rw-rw-   0        0        0    20020 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.623041 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:24:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/__init__.py
+-rw-rw-rw-   0        0        0    17748 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/do_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.625411 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/
+-rw-rw-rw-   0        0        0        0 2024-03-26 11:48:19.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/__init__.py
+-rw-rw-rw-   0        0        0     5564 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/compute_fbank_common.py
+-rw-rw-rw-   0        0        0     1954 2024-04-27 03:52:56.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/data_handler.py
+-rw-rw-rw-   0        0        0    11494 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/icefall_assistant.py
+-rw-rw-rw-   0        0        0        0 2024-03-27 06:22:09.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zip_trainer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.654343 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/
+-rw-rw-rw-   0        0        0        0 2024-03-27 06:19:27.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/__init__.py
+-rw-rw-rw-   0        0        0    13605 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/asr_datamodule.py
+-rw-rw-rw-   0        0        0   109372 2024-05-06 09:10:01.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/beam_search.py
+-rw-rw-rw-   0        0        0    27050 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/decode.py
+-rw-rw-rw-   0        0        0    27656 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_bbpe.py
+-rw-rw-rw-   0        0        0     5331 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_stream.py
+-rw-rw-rw-   0        0        0     4755 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/decoder.py
+-rw-rw-rw-   0        0        0     1652 2024-03-27 06:19:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/encoder_interface.py
+-rw-rw-rw-   0        0        0    25164 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx-streaming.py
+-rw-rw-rw-   0        0        0    18723 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx.py
+-rw-rw-rw-   0        0        0    17410 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/export.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.679946 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/
+-rw-rw-rw-   0        0        0     1402 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/__init__.py
+-rw-rw-rw-   0        0        0     4780 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ali.py
+-rw-rw-rw-   0        0        0     2991 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/bpe_graph_compiler.py
+-rw-rw-rw-   0        0        0     4044 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/byte_utils.py
+-rw-rw-rw-   0        0        0     3436 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/char_graph_compiler.py
+-rw-rw-rw-   0        0        0    15166 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/checkpoint.py
+-rw-rw-rw-   0        0        0    22548 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/context_graph.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.689381 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/
+-rw-rw-rw-   0        0        0      187 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/__init__.py
+-rw-rw-rw-   0        0        0     9561 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/prepare_lang.py
+-rw-rw-rw-   0        0        0     3868 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_ctc_topo.py
+-rw-rw-rw-   0        0        0     1100 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_prepare_lang.py
+-rw-rw-rw-   0        0        0     4628 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/topo.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.690391 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/
+-rw-rw-rw-   0        0        0        0 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2002 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/datamodule.py
+-rw-rw-rw-   0        0        0    44213 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/decode.py
+-rw-rw-rw-   0        0        0    27288 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/diagnostics.py
+-rw-rw-rw-   0        0        0     1966 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dist.py
+-rw-rw-rw-   0        0        0     3472 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/env.py
+-rw-rw-rw-   0        0        0     5508 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/graph_compiler.py
+-rw-rw-rw-   0        0        0     3580 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/hooks.py
+-rw-rw-rw-   0        0        0     8723 2024-03-28 08:19:43.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lexicon.py
+-rw-rw-rw-   0        0        0     7821 2024-02-26 01:51:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lm_wrapper.py
+-rw-rw-rw-   0        0        0     6644 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi.py
+-rw-rw-rw-   0        0        0     7859 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi_graph_compiler.py
+-rw-rw-rw-   0        0        0     5295 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ngram_lm.py
+-rw-rw-rw-   0        0        0     8205 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/otc_graph_compiler.py
+-rw-rw-rw-   0        0        0    30754 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/profiler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.707207 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/
+-rw-rw-rw-   0        0        0        0 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/__init__.py
+-rw-rw-rw-   0        0        0     3644 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx-streaming.py
+-rw-rw-rw-   0        0        0     3205 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx.py
+-rw-rw-rw-   0        0        0     7275 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/compute_perplexity.py
+-rw-rw-rw-   0        0        0     7647 2024-05-06 09:10:01.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/dataset.py
+-rw-rw-rw-   0        0        0    11547 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export-onnx.py
+-rw-rw-rw-   0        0        0     5747 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export.py
+-rw-rw-rw-   0        0        0    10312 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/model.py
+-rw-rw-rw-   0        0        0     2238 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset.py
+-rw-rw-rw-   0        0        0     2977 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset_ddp.py
+-rw-rw-rw-   0        0        0     1842 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_model.py
+-rw-rw-rw-   0        0        0    19664 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/train.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.718714 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/
+-rw-rw-rw-   0        0        0        0 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/__init__.py
+-rw-rw-rw-   0        0        0    22349 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/attention.py
+-rw-rw-rw-   0        0        0     5497 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/compute_perplexity.py
+-rw-rw-rw-   0        0        0       20 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/dataset.py
+-rw-rw-rw-   0        0        0    11234 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/encoder.py
+-rw-rw-rw-   0        0        0     4925 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/export.py
+-rw-rw-rw-   0        0        0     3396 2024-02-26 01:51:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/model.py
+-rw-rw-rw-   0        0        0       65 2024-02-26 01:52:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/scaling.py
+-rw-rw-rw-   0        0        0    17243 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/train.py
+-rw-rw-rw-   0        0        0    76655 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/utils.py
+-rw-rw-rw-   0        0        0     7709 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained.py
+-rw-rw-rw-   0        0        0     7751 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_bbpe.py
+-rw-rw-rw-   0        0        0     8146 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_streaming.py
+-rw-rw-rw-   0        0        0     2214 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/joiner.py
+-rw-rw-rw-   0        0        0    12993 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/model.py
+-rw-rw-rw-   0        0        0     7152 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_check.py
+-rw-rw-rw-   0        0        0     8300 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_decode.py
+-rw-rw-rw-   0        0        0    17464 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained-streaming.py
+-rw-rw-rw-   0        0        0    12357 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained.py
+-rw-rw-rw-   0        0        0    50893 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/optim.py
+-rw-rw-rw-   0        0        0    10603 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained.py
+-rw-rw-rw-   0        0        0    11561 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained_bbpe.py
+-rw-rw-rw-   0        0        0    70696 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling.py
+-rw-rw-rw-   0        0        0     3342 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling_converter.py
+-rw-rw-rw-   0        0        0     9817 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_beam_search.py
+-rw-rw-rw-   0        0        0    31259 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_decode.py
+-rw-rw-rw-   0        0        0    13138 2024-03-27 06:19:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/subsampling.py
+-rw-rw-rw-   0        0        0    43330 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/train.py
+-rw-rw-rw-   0        0        0    29572 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/train_bbpe.py
+-rw-rw-rw-   0        0        0    92936 2024-03-27 06:19:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/zipformer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.720179 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/inference_paraformer/
+-rw-rw-rw-   0        0        0        0 2024-05-13 05:24:11.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/inference_paraformer/__init__.py
+-rw-rw-rw-   0        0        0     1209 2024-05-19 15:32:02.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/inference_paraformer/inference_paraforemr.py
+-rw-rw-rw-   0        0        0       88 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.722665 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_codec_asr/
+-rw-rw-rw-   0        0        0        0 2024-04-18 04:14:09.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_codec_asr/__init__.py
+-rw-rw-rw-   0        0        0     2708 2024-05-07 13:01:09.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_codec_asr/data_handler.py
+-rw-rw-rw-   0        0        0     1646 2024-05-07 13:52:16.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_codec_asr/get_wav_file.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.727731 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/__init__.py
+-rw-rw-rw-   0        0        0     5838 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/handle_peoplespeech.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.728735 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/
+-rw-rw-rw-   0        0        0        0 2024-04-11 13:48:24.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.729888 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/
+-rw-rw-rw-   0        0        0       47 2024-04-11 14:38:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.732538 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/branchformer/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/branchformer/__init__.py
+-rw-rw-rw-   0        0        0     6526 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/branchformer/cgmlp.py
+-rw-rw-rw-   0        0        0    14430 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/branchformer/encoder.py
+-rw-rw-rw-   0        0        0    10013 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/branchformer/encoder_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.736096 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/cli/__init__.py
+-rw-rw-rw-   0        0        0     3674 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/cli/hub.py
+-rw-rw-rw-   0        0        0     6528 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/cli/model.py
+-rw-rw-rw-   0        0        0     3146 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/cli/paraformer_model.py
+-rw-rw-rw-   0        0        0     3106 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/cli/transcribe.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.742349 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/dataset/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/dataset/__init__.py
+-rw-rw-rw-   0        0        0    13875 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/dataset/datapipes.py
+-rw-rw-rw-   0        0        0     5420 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/dataset/dataset.py
+-rw-rw-rw-   0        0        0    26338 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/dataset/kaldi_io.py
+-rw-rw-rw-   0        0        0    16151 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/dataset/processor.py
+-rw-rw-rw-   0        0        0     9365 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/dataset/wav_distortion.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.751057 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/efficient_conformer/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/efficient_conformer/__init__.py
+-rw-rw-rw-   0        0        0    11153 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/efficient_conformer/attention.py
+-rw-rw-rw-   0        0        0     5751 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/efficient_conformer/convolution.py
+-rw-rw-rw-   0        0        0    25637 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/efficient_conformer/encoder.py
+-rw-rw-rw-   0        0        0     6974 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/efficient_conformer/encoder_layer.py
+-rw-rw-rw-   0        0        0     2665 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/efficient_conformer/subsampling.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.752256 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/k2/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/k2/__init__.py
+-rw-rw-rw-   0        0        0    12177 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/k2/model.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.764385 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:28.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/__init__.py
+-rw-rw-rw-   0        0        0     8291 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/attention.py
+-rw-rw-rw-   0        0        0    11703 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/cif.py
+-rw-rw-rw-   0        0        0    12528 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/convert_paraformer_to_wenet_config_and_ckpt.py
+-rw-rw-rw-   0        0        0      459 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/embedding.py
+-rw-rw-rw-   0        0        0    18379 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/layers.py
+-rw-rw-rw-   0        0        0    16474 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/paraformer.py
+-rw-rw-rw-   0        0        0     8305 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/search.py
+-rw-rw-rw-   0        0        0     1541 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/paraformer/subsampling.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.770816 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/squeezeformer/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/squeezeformer/__init__.py
+-rw-rw-rw-   0        0        0    10492 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/squeezeformer/attention.py
+-rw-rw-rw-   0        0        0     2638 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/squeezeformer/conv2d.py
+-rw-rw-rw-   0        0        0     6778 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/squeezeformer/convolution.py
+-rw-rw-rw-   0        0        0    22230 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/squeezeformer/encoder.py
+-rw-rw-rw-   0        0        0     4693 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/squeezeformer/encoder_layer.py
+-rw-rw-rw-   0        0        0     3026 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/squeezeformer/positionwise_feed_forward.py
+-rw-rw-rw-   0        0        0    11569 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/squeezeformer/subsampling.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.781546 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/text/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/text/__init__.py
+-rw-rw-rw-   0        0        0     1223 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/text/base_tokenizer.py
+-rw-rw-rw-   0        0        0     1742 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/text/bpe_tokenizer.py
+-rw-rw-rw-   0        0        0     2744 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/text/char_tokenizer.py
+-rw-rw-rw-   0        0        0     1842 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/text/hugging_face_tokenizer.py
+-rw-rw-rw-   0        0        0     1825 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/text/paraformer_tokenizer.py
+-rw-rw-rw-   0        0        0     2387 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/text/tokenize_utils.py
+-rw-rw-rw-   0        0        0     3516 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/text/whisper_tokenizer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.784586 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transducer/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transducer/__init__.py
+-rw-rw-rw-   0        0        0     4067 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transducer/joint.py
+-rw-rw-rw-   0        0        0    17809 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transducer/predictor.py
+-rw-rw-rw-   0        0        0    23032 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transducer/transducer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.803788 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/__init__.py
+-rw-rw-rw-   0        0        0    20972 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/asr_model.py
+-rw-rw-rw-   0        0        0    14435 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/attention.py
+-rw-rw-rw-   0        0        0     2209 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/cmvn.py
+-rw-rw-rw-   0        0        0     5223 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/convolution.py
+-rw-rw-rw-   0        0        0     3294 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/ctc.py
+-rw-rw-rw-   0        0        0    16498 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/decoder.py
+-rw-rw-rw-   0        0        0     4807 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/decoder_layer.py
+-rw-rw-rw-   0        0        0    13759 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/embedding.py
+-rw-rw-rw-   0        0        0    21311 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/encoder.py
+-rw-rw-rw-   0        0        0     9739 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/encoder_layer.py
+-rw-rw-rw-   0        0        0     3459 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/label_smoothing_loss.py
+-rw-rw-rw-   0        0        0     4219 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/positionwise_feed_forward.py
+-rw-rw-rw-   0        0        0    19759 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/search.py
+-rw-rw-rw-   0        0        0    11291 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/subsampling.py
+-rw-rw-rw-   0        0        0     1003 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/transformer/swish.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.821731 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/__init__.py
+-rw-rw-rw-   0        0        0     3825 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/checkpoint.py
+-rw-rw-rw-   0        0        0     2334 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/class_utils.py
+-rw-rw-rw-   0        0        0     2968 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/cmvn.py
+-rw-rw-rw-   0        0        0    11307 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/common.py
+-rw-rw-rw-   0        0        0     1477 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/config.py
+-rw-rw-rw-   0        0        0     9702 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/context_graph.py
+-rw-rw-rw-   0        0        0     5968 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/ctc_utils.py
+-rw-rw-rw-   0        0        0     5818 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/executor.py
+-rw-rw-rw-   0        0        0     2102 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/file_utils.py
+-rw-rw-rw-   0        0        0     6605 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/init_model.py
+-rw-rw-rw-   0        0        0     2415 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/init_tokenizer.py
+-rw-rw-rw-   0        0        0    12706 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/mask.py
+-rw-rw-rw-   0        0        0    24421 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/scheduler.py
+-rw-rw-rw-   0        0        0    26478 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/utils/train_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.824971 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/whisper/
+-rw-rw-rw-   0        0        0        0 2024-04-11 14:38:29.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/whisper/__init__.py
+-rw-rw-rw-   0        0        0    12881 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/whisper/convert_whisper_to_wenet_config_and_ckpt.py
+-rw-rw-rw-   0        0        0     3380 2024-04-11 14:38:30.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/inference_with_hlg/wenet/whisper/whisper.py
+-rw-rw-rw-   0        0        0     9569 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.831077 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_HLG/
+-rw-rw-rw-   0        0        0        0 2024-04-19 15:10:49.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_HLG/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_HLG/make_hlg.py
+-rw-rw-rw-   0        0        0     4931 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_HLG/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.832469 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_arpa/
+-rw-rw-rw-   0        0        0        0 2024-04-19 12:01:43.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_arpa/__init__.py
+-rw-rw-rw-   0        0        0      751 2024-04-19 12:30:52.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_arpa/data_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.836035 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/
+-rw-rw-rw-   0        0        0        0 2024-04-07 06:18:22.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/__init__.py
+-rw-rw-rw-   0        0        0      547 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/gxl_main.py
+-rw-rw-rw-   0        0        0     4934 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/make_hlg.py
+-rw-rw-rw-   0        0        0     8765 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/prepare_char.py
+-rw-rw-rw-   0        0        0    11735 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_goutu/prepare_lang.py
+-rw-rw-rw-   0        0        0      962 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_shard4new_wenetspeech.py
+-rw-rw-rw-   0        0        0     1186 2024-03-26 14:51:25.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/shard_from_pachong.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.838133 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_fairseq/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_fairseq/__init__.py
+-rw-rw-rw-   0        0        0    13907 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_fairseq/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.850945 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/__init__.py
+-rw-rw-rw-   0        0        0    20570 2024-03-27 10:48:34.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/compute-wer.py
+-rw-rw-rw-   0        0        0     1284 2024-05-12 10:13:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/copy_wav4test_dir.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.852024 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/__init__.py
+-rw-rw-rw-   0        0        0     1582 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/main.py
+-rw-rw-rw-   0        0        0     1931 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/handle4accent.py
+-rw-rw-rw-   0        0        0     6855 2024-04-18 11:22:23.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/main.py
+-rw-rw-rw-   0        0        0     4026 2024-04-13 05:28:58.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/prepare_data4prompt_task.py
+-rw-rw-rw-   0        0        0     5597 2024-05-14 10:41:49.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/qwen_audio.py
+-rw-rw-rw-   0        0        0     3385 2024-05-06 09:09:59.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/speechio_handle.py
+-rw-rw-rw-   0        0        0     2684 2024-05-06 09:10:00.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/test_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.854089 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_TYPE_CHECKING/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_TYPE_CHECKING/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_TYPE_CHECKING/fun.py
+-rw-rw-rw-   0        0        0      125 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_TYPE_CHECKING/test.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.859007 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_gxl_ai_utils/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_gxl_ai_utils/__init__.py
+-rw-rw-rw-   0        0        0      232 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_gxl_ai_utils/download_test.py
+-rw-rw-rw-   0        0        0      793 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_gxl_ai_utils/format_test.py
+-rw-rw-rw-   0        0        0      503 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_gxl_ai_utils/gxl_test.py
+-rw-rw-rw-   0        0        0      746 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_gxl_ai_utils/main.py
+-rw-rw-rw-   0        0        0      400 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_gxl_ai_utils/test.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.863405 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_sentencepiece/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_sentencepiece/__init__.py
+-rw-rw-rw-   0        0        0     1781 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_sentencepiece/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.865860 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/ximalaya/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/ximalaya/__init__.py
+-rw-rw-rw-   0        0        0     2525 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/cats_and_dogs/ximalaya/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.865860 gxl_ai_utils-1.3.5/eggs/ch_en_mix/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/ch_en_mix/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.866862 gxl_ai_utils-1.3.5/eggs/ch_en_mix/data_handle/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/ch_en_mix/data_handle/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.869233 gxl_ai_utils-1.3.5/eggs/finetune_llm/
+-rw-rw-rw-   0        0        0        0 2024-02-29 06:01:16.000000 gxl_ai_utils-1.3.5/eggs/finetune_llm/__init__.py
+-rw-rw-rw-   0        0        0      928 2024-03-13 02:52:18.000000 gxl_ai_utils-1.3.5/eggs/finetune_llm/main.py
+-rw-rw-rw-   0        0        0     1858 2024-03-13 07:52:36.000000 gxl_ai_utils-1.3.5/eggs/finetune_llm/main_2B.py
+-rw-rw-rw-   0        0        0     1367 2024-03-13 07:36:12.000000 gxl_ai_utils-1.3.5/eggs/finetune_llm/transformers_learning.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.874320 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/__init__.py
+-rw-rw-rw-   0        0        0     1635 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/gxl_knowledge_distill.py
+-rw-rw-rw-   0        0        0     1129 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/gxl_paraformer_infer.py
+-rw-rw-rw-   0        0        0     2469 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/gxl_whisper_infer.py
+-rw-rw-rw-   0        0        0     1090 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/handle_cmvn_gxl.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.878515 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/paraformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/paraformer/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/paraformer/decoder.py
+-rw-rw-rw-   0        0        0    27385 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/paraformer/encoder.py
+-rw-rw-rw-   0        0        0      827 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/paraformer_infer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.883060 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/whisper_ctc/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/whisper_ctc/__init__.py
+-rw-rw-rw-   0        0        0      741 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/knowledge_distillation/whisper_ctc/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.893448 gxl_ai_utils-1.3.5/eggs/spider/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/spider/__init__.py
+-rw-rw-rw-   0        0        0      382 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/spider/spdier_little_url_get.py
+-rw-rw-rw-   0        0        0     9274 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/spider/spider_lizhi_fm.py
+-rw-rw-rw-   0        0        0     5810 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/spider/spider_qingting_fm.py
+-rw-rw-rw-   0        0        0    16395 2024-05-06 09:09:58.000000 gxl_ai_utils-1.3.5/eggs/spider/spider_qingting_fm_new.py
+-rw-rw-rw-   0        0        0    14467 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/spider/spider_ximalaya.py
+-rw-rw-rw-   0        0        0    10475 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/spider/spider_ximalaya_new.py
+-rw-rw-rw-   0        0        0     7041 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/spider/spider_yunting.py
+-rw-rw-rw-   0        0        0     4983 2024-02-25 08:28:39.000000 gxl_ai_utils-1.3.5/eggs/spider/spider_zhihu.py
+-rw-rw-rw-   0        0        0     4770 2024-02-25 08:26:09.000000 gxl_ai_utils-1.3.5/eggs/spider/spider_zhihu_2.py
+-rw-rw-rw-   0        0        0     3479 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/eggs/spider/test.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.899882 gxl_ai_utils-1.3.5/eggs/spider/voicewiki/
+-rw-rw-rw-   0        0        0        0 2024-04-18 14:18:18.000000 gxl_ai_utils-1.3.5/eggs/spider/voicewiki/__init__.py
+-rw-rw-rw-   0        0        0     7137 2024-04-19 06:08:17.000000 gxl_ai_utils-1.3.5/eggs/spider/voicewiki/spider_2.py
+-rw-rw-rw-   0        0        0    24934 2024-04-18 14:19:26.000000 gxl_ai_utils-1.3.5/eggs/spider/voicewiki/spider_voicewiki.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.901054 gxl_ai_utils-1.3.5/eggs/spider/wangyiyun/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:45:49.000000 gxl_ai_utils-1.3.5/eggs/spider/wangyiyun/__init__.py
+-rw-rw-rw-   0        0        0     1256 2024-04-11 09:46:54.000000 gxl_ai_utils-1.3.5/eggs/spider/wangyiyun/spider_wangyiyun.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.903143 gxl_ai_utils-1.3.5/gxl_ai_utils/
+-rw-rw-rw-   0        0        0     1651 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/AiConstant.py
+-rw-rw-rw-   0        0        0      556 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.926568 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/
+-rw-rw-rw-   0        0        0       35 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/__init__.py
+-rw-rw-rw-   0        0        0    14863 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/build_vocab.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.933252 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/classify/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/classify/__init__.py
+-rw-rw-rw-   0        0        0     5401 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/classify/data_handler.py
+-rw-rw-rw-   0        0        0     6562 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/common_data_handler.py
+-rw-rw-rw-   0        0        0     6242 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/gxl_data_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.936344 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/recognition/
+-rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/recognition/__init__.py
+-rw-rw-rw-   0        0        0    10901 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/recognition/data_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.937340 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_handler/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.937340 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/
+-rw-rw-rw-   0        0        0       36 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.939901 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/classify/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/classify/__init__.py
+-rw-rw-rw-   0        0        0    17914 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/classify/ecapa_tdnn.py
+-rw-rw-rw-   0        0        0    27764 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/classify/xvector.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.941345 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/
+-rw-rw-rw-   0        0        0       50 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.950360 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/deepspeech2/
+-rw-rw-rw-   0        0        0       25 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/deepspeech2/__init__.py
+-rw-rw-rw-   0        0        0    14593 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/deepspeech2/deepspeech2.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.955545 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/modules/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/modules/__init__.py
+-rw-rw-rw-   0        0        0     6869 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/modules/ctc_decoder.py
+-rw-rw-rw-   0        0        0     5452 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/modules/embedding.py
+-rw-rw-rw-   0        0        0     8872 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/modules/subsampling.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.956848 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.961949 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.971151 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/__init__.py
+-rw-rw-rw-   0        0        0     1942 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/multi_head_attention.py
+-rw-rw-rw-   0        0        0     1662 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_encoding.py
+-rw-rw-rw-   0        0        0      936 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_wise_feed_forward.py
+-rw-rw-rw-   0        0        0     1193 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/scaled_dot_product_attention.py
+-rw-rw-rw-   0        0        0     3050 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/decoder.py
+-rw-rw-rw-   0        0        0     2386 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/encoder.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.973623 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/utils/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/utils/padding_mask.py
+-rw-rw-rw-   0        0        0      427 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/utils/sequence_mask.py
+-rw-rw-rw-   0        0        0     1305 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.975620 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/utils/__init__.py
+-rw-rw-rw-   0        0        0    14807 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/utils/ctc_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.976618 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/t2s/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/t2s/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.982195 gxl_ai_utils-1.3.5/gxl_ai_utils/config/
+-rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/config/__init__.py
+-rw-rw-rw-   0        0        0     5179 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/config/gxl_config.py
+-rw-rw-rw-   0        0        0      121 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.987168 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_dataset_wenet/
+-rw-rw-rw-   0        0        0        2 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_dataset_wenet/__init__.py
+-rw-rw-rw-   0        0        0     7429 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_dataset_wenet/gxl_dataset.py
+-rw-rw-rw-   0        0        0    18215 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_dataset_wenet/gxl_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.992792 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/__init__.py
+-rw-rw-rw-   0        0        0    10270 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/alignment.py
+-rw-rw-rw-   0        0        0     3616 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/average_model.py
+-rw-rw-rw-   0        0        0     5604 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/gxl_infer.py
+-rw-rw-rw-   0        0        0    12155 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/recognize.py
+-rw-rw-rw-   0        0        0    12797 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/recognize_onnx_gpu.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.998649 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_lr_scheduler_wenet/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_lr_scheduler_wenet/__init__.py
+-rw-rw-rw-   0        0        0    24245 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_lr_scheduler_wenet/scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.002232 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.006241 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/branchformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/branchformer/__init__.py
+-rw-rw-rw-   0        0        0     6645 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/branchformer/cgmlp.py
+-rw-rw-rw-   0        0        0    16717 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/branchformer/encoder.py
+-rw-rw-rw-   0        0        0    10038 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/branchformer/encoder_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.007652 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/cif/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/cif/__init__.py
+-rw-rw-rw-   0        0        0    11275 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/cif/predictor.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.011259 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/e_branchformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/e_branchformer/__init__.py
+-rw-rw-rw-   0        0        0    16682 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder.py
+-rw-rw-rw-   0        0        0     6840 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.021549 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/__init__.py
+-rw-rw-rw-   0        0        0    11117 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/attention.py
+-rw-rw-rw-   0        0        0     5905 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/convolution.py
+-rw-rw-rw-   0        0        0    26376 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder.py
+-rw-rw-rw-   0        0        0     7093 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder_layer.py
+-rw-rw-rw-   0        0        0     2749 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/subsampling.py
+-rw-rw-rw-   0        0        0     7413 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/init_model.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.023621 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/k2/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/k2/__init__.py
+-rw-rw-rw-   0        0        0    11851 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/k2/model.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.036529 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/__init__.py
+-rw-rw-rw-   0        0        0     8230 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/attention.py
+-rw-rw-rw-   0        0        0    11269 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/cif.py
+-rw-rw-rw-   0        0        0     5301 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/convert_paraformer_to_wenet_config.py
+-rw-rw-rw-   0        0        0    17521 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/layers.py
+-rw-rw-rw-   0        0        0     9883 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/paraformer.py
+-rw-rw-rw-   0        0        0     6945 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/search.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.045961 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/__init__.py
+-rw-rw-rw-   0        0        0    10509 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/attention.py
+-rw-rw-rw-   0        0        0     2636 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/conv2d.py
+-rw-rw-rw-   0        0        0     6713 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/convolution.py
+-rw-rw-rw-   0        0        0    22398 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder.py
+-rw-rw-rw-   0        0        0     4833 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder_layer.py
+-rw-rw-rw-   0        0        0     3067 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/positionwise_feed_forward.py
+-rw-rw-rw-   0        0        0    11264 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/subsampling.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.054219 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/__init__.py
+-rw-rw-rw-   0        0        0     4110 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/joint.py
+-rw-rw-rw-   0        0        0    18089 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/predictor.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.056218 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/search/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/search/__init__.py
+-rw-rw-rw-   0        0        0     2014 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/search/greedy_search.py
+-rw-rw-rw-   0        0        0     6112 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/search/prefix_beam_search.py
+-rw-rw-rw-   0        0        0    23241 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/transducer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.085784 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/__init__.py
+-rw-rw-rw-   0        0        0    18961 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/asr_model.py
+-rw-rw-rw-   0        0        0    14383 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/attention.py
+-rw-rw-rw-   0        0        0     1533 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/cmvn.py
+-rw-rw-rw-   0        0        0     5329 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/convolution.py
+-rw-rw-rw-   0        0        0     3084 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/ctc.py
+-rw-rw-rw-   0        0        0    12855 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/decoder.py
+-rw-rw-rw-   0        0        0     4939 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/decoder_layer.py
+-rw-rw-rw-   0        0        0     6339 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/embedding.py
+-rw-rw-rw-   0        0        0    20622 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/encoder.py
+-rw-rw-rw-   0        0        0     9838 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/encoder_layer.py
+-rw-rw-rw-   0        0        0     3806 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/label_smoothing_loss.py
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/paraformer_encoder.py
+-rw-rw-rw-   0        0        0     1940 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/positionwise_feed_forward.py
+-rw-rw-rw-   0        0        0    18309 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/search.py
+-rw-rw-rw-   0        0        0     9512 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/subsampling.py
+-rw-rw-rw-   0        0        0     1029 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/swish.py
+-rw-rw-rw-   0        0        0     6294 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/whisper_decoder.py
+-rw-rw-rw-   0        0        0     8366 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder.py
+-rw-rw-rw-   0        0        0     2582 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder_gxl.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.106630 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/__init__.py
+-rw-rw-rw-   0        0        0     4018 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/checkpoint.py
+-rw-rw-rw-   0        0        0     3065 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/cmvn.py
+-rw-rw-rw-   0        0        0     7954 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/common.py
+-rw-rw-rw-   0        0        0     1516 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/config.py
+-rw-rw-rw-   0        0        0     9964 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/context_graph.py
+-rw-rw-rw-   0        0        0     5411 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/ctc_utils.py
+-rw-rw-rw-   0        0        0     4353 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/executor.py
+-rw-rw-rw-   0        0        0     2168 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/file_utils.py
+-rw-rw-rw-   0        0        0     1291 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/init_ali_paraformer.py
+-rw-rw-rw-   0        0        0     7440 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/init_model.py
+-rw-rw-rw-   0        0        0    13020 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/mask.py
+-rw-rw-rw-   0        0        0    24245 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/scheduler.py
+-rw-rw-rw-   0        0        0     1568 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/tokenize_utils.py
+-rw-rw-rw-   0        0        0    26574 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/train_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.114069 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/__init__.py
+-rw-rw-rw-   0        0        0    14805 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/attentions.py
+-rw-rw-rw-   0        0        0     4860 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/commons.py
+-rw-rw-rw-   0        0        0    24767 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/models.py
+-rw-rw-rw-   0        0        0    16740 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/modules.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.117077 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_trainer_wenet/
+-rw-rw-rw-   0        0        0       35 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_trainer_wenet/__init__.py
+-rw-rw-rw-   0        0        0     9889 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_trainer_wenet/gxl_trainer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.132049 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/
+-rw-rw-rw-   0        0        0     7061 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/__init__.py
+-rw-rw-rw-   0        0        0       38 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/__main__.py
+-rw-rw-rw-   0        0        0     5089 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/audio.py
+-rw-rw-rw-   0        0        0    33001 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/decoding.py
+-rw-rw-rw-   0        0        0    11165 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/model.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.135028 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/normalizers/
+-rw-rw-rw-   0        0        0      132 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/normalizers/__init__.py
+-rw-rw-rw-   0        0        0     2012 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/normalizers/basic.py
+-rw-rw-rw-   0        0        0    21418 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/normalizers/english.py
+-rw-rw-rw-   0        0        0    12968 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/timing.py
+-rw-rw-rw-   0        0        0    12733 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/tokenizer.py
+-rw-rw-rw-   0        0        0    23334 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/transcribe.py
+-rw-rw-rw-   0        0        0     3583 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/triton_ops.py
+-rw-rw-rw-   0        0        0    11363 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/utils.py
+-rw-rw-rw-   0        0        0       26 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/version.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.135028 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.136025 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/asr/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/asr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.138019 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/asr/encoder/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/asr/encoder/__init__.py
+-rw-rw-rw-   0        0        0      414 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/asr/encoder/abs_encoder.py
+-rw-rw-rw-   0        0        0     9977 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/asr/encoder/conformer_encoder.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.139020 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/fastformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/fastformer/__init__.py
+-rw-rw-rw-   0        0        0     2297 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/fastformer/fastformer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.149347 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/__init__.py
+-rw-rw-rw-   0        0        0    19543 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/build_asr_model.py
+-rw-rw-rw-   0        0        0   102558 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/e2e_asr_paraformer.py
+-rw-rw-rw-   0        0        0    79092 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/sanm_decoder.py
+-rw-rw-rw-   0        0        0    58681 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/sanm_encoder.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.152343 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/__init__.py
+-rw-rw-rw-   0        0        0     6478 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/component.py
+-rw-rw-rw-   0        0        0     2953 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/decoder.py
+-rw-rw-rw-   0        0        0     2299 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/encoder.py
+-rw-rw-rw-   0        0        0     1405 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.157324 gxl_ai_utils-1.3.5/gxl_ai_utils/run/
+-rw-rw-rw-   0        0        0       22 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/run/__init__.py
+-rw-rw-rw-   0        0        0     9326 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/run/base_train_runner.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.165712 gxl_ai_utils-1.3.5/gxl_ai_utils/run/flask_template/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/run/flask_template/__init__.py
+-rw-rw-rw-   0        0        0     1061 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/run/flask_template/flask_predict.py
+-rw-rw-rw-   0        0        0     4263 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/run/flask_template/flask_server.py
+-rw-rw-rw-   0        0        0     3023 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/run/runner.py
+-rw-rw-rw-   0        0        0     2602 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/run/runner_multi_template.py
+-rw-rw-rw-   0        0        0      593 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/run/runner_single_template.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.168911 gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/
+-rw-rw-rw-   0        0        0       76 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/__init__.py
+-rw-rw-rw-   0        0        0     4311 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/store_data.py
+-rw-rw-rw-   0        0        0      177 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/store_data_name.py
+-rw-rw-rw-   0        0        0      451 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/store_dataloader.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.171914 gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/store_dataset/
+-rw-rw-rw-   0        0        0       29 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/store_dataset/__init__.py
+-rw-rw-rw-   0        0        0     5238 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/store_dataset/store_dataset.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.177213 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/
+-rw-rw-rw-   0        0        0       64 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/__init__.py
+-rw-rw-rw-   0        0        0     2072 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.185715 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/
+-rw-rw-rw-   0        0        0       33 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/__init__.py
+-rw-rw-rw-   0        0        0     6223 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/attention_model.py
+-rw-rw-rw-   0        0        0     2438 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/cnn_model.py
+-rw-rw-rw-   0        0        0      958 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/mlp_model.py
+-rw-rw-rw-   0        0        0     2130 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/rnn_model.py
+-rw-rw-rw-   0        0        0     2348 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/store_model_class.py
+-rw-rw-rw-   0        0        0      578 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_name.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.186714 gxl_ai_utils-1.3.5/gxl_ai_utils/thread/
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/thread/__init__.py
+-rw-rw-rw-   0        0        0     1522 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/thread/my_thread.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:47.200535 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/
+-rw-rw-rw-   0        0        0       92 2024-04-18 14:02:06.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/__init__.py
+-rw-rw-rw-   0        0        0    20570 2024-03-27 10:48:34.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/compute-wer.py
+-rw-rw-rw-   0        0        0        0 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_coding.py
+-rw-rw-rw-   0        0        0    26855 2024-03-27 07:04:56.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_data.py
+-rw-rw-rw-   0        0        0      423 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_device.py
+-rw-rw-rw-   0        0        0    58529 2024-05-21 15:46:44.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_file.py
+-rw-rw-rw-   0        0        0    26449 2024-05-24 06:43:51.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_file_2.py
+-rw-rw-rw-   0        0        0     6482 2024-05-21 13:54:21.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_model.py
+-rw-rw-rw-   0        0        0     2537 2024-05-21 13:49:43.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_showing.py
+-rw-rw-rw-   0        0        0     6811 2024-05-21 13:49:43.000000 gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_spider.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:49:46.921331 gxl_ai_utils-1.3.5/gxl_ai_utils.egg-info/
+-rw-rw-rw-   0        0        0      212 2024-05-24 06:49:46.000000 gxl_ai_utils-1.3.5/gxl_ai_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    31807 2024-05-24 06:49:46.000000 gxl_ai_utils-1.3.5/gxl_ai_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 06:49:46.000000 gxl_ai_utils-1.3.5/gxl_ai_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-24 06:49:46.000000 gxl_ai_utils-1.3.5/gxl_ai_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      592 2024-02-22 05:19:39.000000 gxl_ai_utils-1.3.5/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 06:49:47.202739 gxl_ai_utils-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      519 2024-05-24 06:47:42.000000 gxl_ai_utils-1.3.5/setup.py
```

### Comparing `gxl_ai_utils-1.3.4/eggs/aishell/do_train.py` & `gxl_ai_utils-1.3.5/eggs/aishell/do_train.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/asr_handle_to_tts_mode/punctuation/punctuation.py` & `gxl_ai_utils-1.3.5/eggs/asr_handle_to_tts_mode/punctuation/punctuation.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_gigaspeech.py` & `gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/handle_gigaspeech.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_haoweilai.py` & `gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/handle_haoweilai.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_librispeech.py` & `gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/handle_librispeech.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/handle_mls.py` & `gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/handle_mls.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/asr_shard_and_format/make_shard.py` & `gxl_ai_utils-1.3.5/eggs/asr_shard_and_format/make_shard.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/0_shenghuo_4/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/1_ertong10T/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/2_jiangkang10T/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/3_jiangkang10T_2/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/4_lizhi_jiankang/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/5_yunting_taihaizhisheng/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/6_yunting_zhongguozhisheng/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/7_liukai_youshengxiaoshuo/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/8_liukai_chuantongguoxue/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/child_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-1.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-1.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-2.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4lishi-2.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4redian.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_handle4redian.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/do_remove.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/do_remove.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/common_utils.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/gxl_common_utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/health_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/lizhi_health_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/make_shard.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/make_shard.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_2/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_3/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shangye_caijing_4/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/shenghuo_2/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/do_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/handle_tts_data_for_asr/yunting_taihaizhisheng_1/do_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/compute_fbank_common.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/compute_fbank_common.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/icefall_assistant.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/icefall_assistant.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/asr_datamodule.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/asr_datamodule.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/beam_search.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/beam_search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decode.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/decode.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_bbpe.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_bbpe.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_stream.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/decode_stream.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/decoder.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/encoder_interface.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/encoder_interface.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx-streaming.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx-streaming.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/export-onnx.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/export.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/export.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/__init__.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/__init__.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ali.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ali.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/bpe_graph_compiler.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/bpe_graph_compiler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/byte_utils.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/byte_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/char_graph_compiler.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/char_graph_compiler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/checkpoint.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/checkpoint.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/context_graph.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/context_graph.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/prepare_lang.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/prepare_lang.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_ctc_topo.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_ctc_topo.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_prepare_lang.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/test_prepare_lang.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/topo.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ctc/topo.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/datamodule.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dataset/datamodule.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/decode.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/decode.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/diagnostics.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/diagnostics.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dist.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/dist.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/env.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/env.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/graph_compiler.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/graph_compiler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/hooks.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/hooks.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lexicon.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lexicon.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lm_wrapper.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/lm_wrapper.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi_graph_compiler.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/mmi_graph_compiler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ngram_lm.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/ngram_lm.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/otc_graph_compiler.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/otc_graph_compiler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/profiler.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/profiler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx-streaming.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx-streaming.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/check-onnx.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/compute_perplexity.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/compute_perplexity.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/dataset.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/dataset.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export-onnx.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export-onnx.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/export.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/model.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset_ddp.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_dataset_ddp.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_model.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/test_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/train.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/rnn_lm/train.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/attention.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/compute_perplexity.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/compute_perplexity.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/encoder.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/export.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/export.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/model.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/train.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/transformer_lm/train.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/utils.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/icefall/utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_bbpe.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_bbpe.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_streaming.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/jit_pretrained_streaming.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/joiner.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/joiner.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/model.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_check.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_check.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_decode.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_decode.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained-streaming.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained-streaming.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/onnx_pretrained.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/optim.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/optim.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained_bbpe.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/pretrained_bbpe.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling_converter.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/scaling_converter.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_beam_search.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_beam_search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_decode.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/streaming_decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
-# Copyright 2022-2023 Xiaomi Corporation (Authors: Wei Kang,
+# Copyright 2022-2024 Xiaomi Corporation (Authors: Wei Kang,
 #                                                  Fangjun Kuang,
-#                                                  Zengwei Yao)
+#                                                  Zengwei Yao,
+#                                                  Zengrui Jin,)
 #
 # See ../../../../LICENSE for clarification regarding multiple authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -19,34 +20,37 @@
 
 """
 Usage:
 ./zipformer/streaming_decode.py \
   --epoch 28 \
   --avg 15 \
   --causal 1 \
-  --chunk-size 16 \
+  --chunk-size 32 \
   --left-context-frames 256 \
   --exp-dir ./zipformer/exp \
   --decoding-method greedy_search \
   --num-decode-streams 2000
 """
 
 import argparse
 import logging
 import math
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
 import k2
 import numpy as np
+import sentencepiece as spm
 import torch
-from asr_datamodule import AishellAsrDataModule
+from asr_datamodule import AsrDataModule
 from decode_stream import DecodeStream
 from kaldifeat import Fbank, FbankOptions
 from lhotse import CutSet
+from lhotse.cut import Cut
+from multi_dataset import MultiDataset
 from streaming_beam_search import (
     fast_beam_search_one_best,
     greedy_search,
     modified_beam_search,
 )
 from torch import Tensor, nn
 from torch.nn.utils.rnn import pad_sequence
@@ -54,31 +58,52 @@
 
 from icefall.checkpoint import (
     average_checkpoints,
     average_checkpoints_with_averaged_model,
     find_checkpoints,
     load_checkpoint,
 )
-from icefall.lexicon import Lexicon
 from icefall.utils import (
     AttributeDict,
     make_pad_mask,
     setup_logger,
     store_transcripts,
     str2bool,
     write_error_stats,
 )
+from icefall import byte_encode, smart_byte_decode, tokenize_by_CJK_char
 
 LOG_EPS = math.log(1e-10)
 
 
 def get_parser():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
+    parser.add_argument(
+        "--train-fbank-dir",
+        type=str,
+    )
+    parser.add_argument(
+        "--valid-fbank-dir",
+        type=str,
+    )
+    parser.add_argument(
+        "--test-parent-dir",
+        type=str,
+    )
+    parser.add_argument(
+        "--train_prefix",
+        type=str,
+    )
+    parser.add_argument(
+        "--valid_prefix",
+        type=str,
+    )
+
 
     parser.add_argument(
         "--epoch",
         type=int,
         default=28,
         help="""It specifies the checkpoint to use for decoding.
         Note: Epoch counts from 1.
@@ -119,18 +144,18 @@
         "--exp-dir",
         type=str,
         default="zipformer/exp",
         help="The experiment dir",
     )
 
     parser.add_argument(
-        "--lang-dir",
+        "--bpe-model",
         type=str,
-        default="data/lang_char",
-        help="Path to the lang dir(containing lexicon, tokens, etc.)",
+        default="data/lang_bpe_500/bpe.model",
+        help="Path to the BPE model",
     )
 
     parser.add_argument(
         "--decoding-method",
         type=str,
         default="greedy_search",
         help="""Supported decoding methods are:
@@ -178,26 +203,14 @@
         "--context-size",
         type=int,
         default=2,
         help="The context size in the decoder. 1 means bigram; 2 means tri-gram",
     )
 
     parser.add_argument(
-        "--blank-penalty",
-        type=float,
-        default=0.0,
-        help="""
-        The penalty applied on blank symbol during decoding.
-        Note: It is a positive value that would be applied to logits like
-        this `logits[:, 0] -= blank_penalty` (suppose logits.shape is
-        [batch_size, vocab] and blank id is 0).
-        """,
-    )
-
-    parser.add_argument(
         "--num-decode-streams",
         type=int,
         default=2000,
         help="The number of streams that can be decoded parallel.",
     )
 
     add_model_arguments(parser)
@@ -490,40 +503,33 @@
         chunk_size=chunk_size,
         left_context_len=left_context_len,
     )
 
     encoder_out = model.joiner.encoder_proj(encoder_out)
 
     if params.decoding_method == "greedy_search":
-        greedy_search(
-            model=model,
-            encoder_out=encoder_out,
-            streams=decode_streams,
-            blank_penalty=params.blank_penalty,
-        )
+        greedy_search(model=model, encoder_out=encoder_out, streams=decode_streams)
     elif params.decoding_method == "fast_beam_search":
         processed_lens = torch.tensor(processed_lens, device=device)
         processed_lens = processed_lens + encoder_out_lens
         fast_beam_search_one_best(
             model=model,
             encoder_out=encoder_out,
             processed_lens=processed_lens,
             streams=decode_streams,
             beam=params.beam,
             max_states=params.max_states,
             max_contexts=params.max_contexts,
-            blank_penalty=params.blank_penalty,
         )
     elif params.decoding_method == "modified_beam_search":
         modified_beam_search(
             model=model,
             streams=decode_streams,
             encoder_out=encoder_out,
             num_active_paths=params.num_active_paths,
-            blank_penalty=params.blank_penalty,
         )
     else:
         raise ValueError(f"Unsupported decoding method: {params.decoding_method}")
 
     states = unstack_states(new_states)
 
     finished_streams = []
@@ -536,28 +542,28 @@
     return finished_streams
 
 
 def decode_dataset(
     cuts: CutSet,
     params: AttributeDict,
     model: nn.Module,
-    lexicon: Lexicon,
+    sp: spm.SentencePieceProcessor,
     decoding_graph: Optional[k2.Fsa] = None,
 ) -> Dict[str, List[Tuple[List[str], List[str]]]]:
     """Decode dataset.
 
     Args:
       cuts:
         Lhotse Cutset containing the dataset to decode.
       params:
         It is returned by :func:`get_params`.
       model:
         The neural model.
-      lexicon:
-        The Lexicon.
+      sp:
+        The BPE model.
       decoding_graph:
         The decoding graph. Can be either a `k2.trivial_graph` or HLG, Used
         only when --decoding_method is fast_beam_search.
     Returns:
       Return a dict, whose key may be "greedy_search" if greedy search
       is used, or it may be "beam_7" if beam size of 7 is used.
       Its value is a list of tuples. Each tuple contains two elements:
@@ -568,15 +574,14 @@
 
     opts = FbankOptions()
     opts.device = device
     opts.frame_opts.dither = 0
     opts.frame_opts.snip_edges = False
     opts.frame_opts.samp_freq = 16000
     opts.mel_opts.num_bins = 80
-    opts.mel_opts.high_freq = -400
 
     log_interval = 100
 
     decode_results = []
     # Contain decode streams currently running.
     decode_streams = []
     for num, cut in enumerate(cuts):
@@ -613,76 +618,89 @@
 
         decode_streams.append(decode_stream)
 
         while len(decode_streams) >= params.num_decode_streams:
             finished_streams = decode_one_chunk(
                 params=params, model=model, decode_streams=decode_streams
             )
+            logging.info('耿雪龙耿雪龙')
             for i in sorted(finished_streams, reverse=True):
+                token_list_i = decode_streams[i].decoding_result()
+                decode_long_str = sp.decode(token_list_i)
+                res_str = smart_byte_decode(decode_long_str).split()
+                res_str = ["".join(res_str)]
+                logging.info(token_list_i)
+                logging.info(decode_long_str)
+                logging.info(res_str)
                 decode_results.append(
                     (
                         decode_streams[i].id,
-                        list(decode_streams[i].ground_truth.strip()),
-                        [
-                            lexicon.token_table[idx]
-                            for idx in decode_streams[i].decoding_result()
-                        ],
+                        decode_streams[i].ground_truth.split(),
+                        res_str
+                        # smart_byte_decode(sp.decode(decode_streams[i].decoding_result()).split()),
                     )
                 )
                 del decode_streams[i]
 
         if num % log_interval == 0:
             logging.info(f"Cuts processed until now is {num}.")
 
     # decode final chunks of last sequences
     while len(decode_streams):
         finished_streams = decode_one_chunk(
             params=params, model=model, decode_streams=decode_streams
         )
+        logging.info('耿雪龙耿雪龙')
         for i in sorted(finished_streams, reverse=True):
+            token_list_i = decode_streams[i].decoding_result()
+            decode_long_str = sp.decode(token_list_i)
+            res_str = smart_byte_decode(decode_long_str).split()
+            res_str = ["".join(res_str)]
+
+            logging.info(token_list_i)
+            logging.info(decode_long_str)
+            logging.info(res_str)
             decode_results.append(
                 (
                     decode_streams[i].id,
                     decode_streams[i].ground_truth.split(),
-                    [
-                        lexicon.token_table[idx]
-                        for idx in decode_streams[i].decoding_result()
-                    ],
+                    res_str
+                    # sp.decode(decode_streams[i].decoding_result()).split(),
                 )
             )
             del decode_streams[i]
 
-    key = f"blank_penalty_{params.blank_penalty}"
     if params.decoding_method == "greedy_search":
-        key = f"greedy_search_{key}"
+        key = "greedy_search"
     elif params.decoding_method == "fast_beam_search":
         key = (
             f"beam_{params.beam}_"
             f"max_contexts_{params.max_contexts}_"
-            f"max_states_{params.max_states}_{key}"
+            f"max_states_{params.max_states}"
         )
     elif params.decoding_method == "modified_beam_search":
-        key = f"num_active_paths_{params.num_active_paths}_{key}"
+        key = f"num_active_paths_{params.num_active_paths}"
     else:
         raise ValueError(f"Unsupported decoding method: {params.decoding_method}")
     return {key: decode_results}
 
 
 def save_results(
     params: AttributeDict,
     test_set_name: str,
     results_dict: Dict[str, List[Tuple[List[str], List[str]]]],
+    sp= None
 ):
     test_set_wers = dict()
     for key, results in results_dict.items():
         recog_path = (
             params.res_dir / f"recogs-{test_set_name}-{key}-{params.suffix}.txt"
         )
         results = sorted(results)
-        store_transcripts(filename=recog_path, texts=results)
+        store_transcripts(filename=recog_path, texts=results,sp=sp)
         logging.info(f"The transcripts are stored in {recog_path}")
 
         # The following prints out WERs, per-word error statistics and aligned
         # ref/hyp pairs.
         errs_filename = (
             params.res_dir / f"errs-{test_set_name}-{key}-{params.suffix}.txt"
         )
@@ -710,15 +728,15 @@
         note = ""
     logging.info(s)
 
 
 @torch.no_grad()
 def main():
     parser = get_parser()
-    AishellAsrDataModule.add_arguments(parser)
+    AsrDataModule.add_arguments(parser)
     args = parser.parse_args()
     args.exp_dir = Path(args.exp_dir)
 
     params = get_params()
     params.update(vars(args))
 
     params.res_dir = params.exp_dir / "streaming" / params.decoding_method
@@ -731,15 +749,14 @@
     assert params.causal, params.causal
     assert "," not in params.chunk_size, "chunk_size should be one value in decoding."
     assert (
         "," not in params.left_context_frames
     ), "left_context_frames should be one value in decoding."
     params.suffix += f"-chunk-{params.chunk_size}"
     params.suffix += f"-left-context-{params.left_context_frames}"
-    params.suffix += f"-blank-penalty-{params.blank_penalty}"
 
     # for fast_beam_search
     if params.decoding_method == "fast_beam_search":
         params.suffix += f"-beam-{params.beam}"
         params.suffix += f"-max-contexts-{params.max_contexts}"
         params.suffix += f"-max-states-{params.max_states}"
 
@@ -751,17 +768,21 @@
 
     device = torch.device("cpu")
     if torch.cuda.is_available():
         device = torch.device("cuda", 0)
 
     logging.info(f"Device: {device}")
 
-    lexicon = Lexicon(params.lang_dir)
-    params.blank_id = lexicon.token_table["<blk>"]
-    params.vocab_size = max(lexicon.tokens) + 1
+    sp = spm.SentencePieceProcessor()
+    sp.load(params.bpe_model)
+
+    # <blk> and <unk> is defined in local/train_bpe_model.py
+    params.blank_id = sp.piece_to_id("<blk>")
+    params.unk_id = sp.piece_to_id("<unk>")
+    params.vocab_size = sp.get_piece_size()
 
     logging.info(params)
 
     logging.info("About to create model")
     model = get_model(params)
 
     if not params.use_averaged_model:
@@ -848,34 +869,48 @@
     decoding_graph = None
     if params.decoding_method == "fast_beam_search":
         decoding_graph = k2.trivial_graph(params.vocab_size - 1, device=device)
 
     num_param = sum([p.numel() for p in model.parameters()])
     logging.info(f"Number of model parameters: {num_param}")
 
-    aishell = AishellAsrDataModule(args)
+    multi_dataset = MultiDataset(args)
 
-    dev_cuts = aishell.valid_cuts()
-    test_cuts = aishell.test_cuts()
+    def remove_short_utt(c: Cut):
+        T = ((c.num_frames - 7) // 2 + 1) // 2
+        if T <= 0:
+            logging.warning(
+                f"Excluding cut with ID: {c.id} from decoding, num_frames: {c.num_frames}"
+            )
+        return T > 0
 
-    test_sets = ["dev", "test"]
-    test_cuts = [dev_cuts, test_cuts]
+    test_sets_cuts = multi_dataset.test_cuts()
 
+    test_sets = test_sets_cuts.keys()
+    test_cuts = [test_sets_cuts[k] for k in test_sets]
+    true_test_set = ['aishell','aishell2','mix_asru','speechio_0','speechio_1','test_net_1','test_meeting','test_net_2']
+    # true_test_set = ['xiaotaicai']
     for test_set, test_cut in zip(test_sets, test_cuts):
+        if not test_set in true_test_set:
+            continue
+        logging.info(f"Decoding {test_set}")
+        test_cut = test_cut.filter(remove_short_utt)
         results_dict = decode_dataset(
             cuts=test_cut,
             params=params,
             model=model,
-            lexicon=lexicon,
+            sp=sp,
             decoding_graph=decoding_graph,
         )
+
         save_results(
             params=params,
             test_set_name=test_set,
             results_dict=results_dict,
+            # sp = sp
         )
 
     logging.info("Done!")
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/subsampling.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/subsampling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/train.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/train.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/train_bbpe.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/train_bbpe.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/icefall_assistant/zipformer/zipformer.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/icefall_assistant/zipformer/zipformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/handle_peoplespeech.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/handle_peoplespeech.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/main.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/make_shard4new_wenetspeech.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/make_shard4new_wenetspeech.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_en_cn/shard_from_pachong.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_en_cn/shard_from_pachong.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_fairseq/main.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_fairseq/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/compute-wer.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/compute-wer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/main.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/data_filter/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/handle4accent.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/handle4accent.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/main.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,10 +160,12 @@
     trainl_dir = "/home/local_data/data4w/shard_1/train_l"
     trainl_list = glob.glob(os.path.join(trainl_dir, "*.tar"))
     gxl_all_list.extend(trainl_list)
     random.shuffle(gxl_all_list)
     utils_file.write_list_to_file(gxl_all_list, gxl_all_path_o)
 
 
+
+
 if __name__ == '__main__':
     """"""
     added_trainl_data_to_gxl_all()
```

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/prepare_data_for_salmonn/speechio_handle.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/prepare_data_for_salmonn/speechio_handle.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/format_test.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_gxl_ai_utils/format_test.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_gxl_ai_utils/main.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_gxl_ai_utils/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/test_sentencepiece/main.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/test_sentencepiece/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/cats_and_dogs/ximalaya/main.py` & `gxl_ai_utils-1.3.5/eggs/cats_and_dogs/ximalaya/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/finetune_llm/main.py` & `gxl_ai_utils-1.3.5/eggs/finetune_llm/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/finetune_llm/main_2B.py` & `gxl_ai_utils-1.3.5/eggs/finetune_llm/main_2B.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/finetune_llm/transformers_learning.py` & `gxl_ai_utils-1.3.5/eggs/finetune_llm/transformers_learning.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_knowledge_distill.py` & `gxl_ai_utils-1.3.5/eggs/knowledge_distillation/gxl_knowledge_distill.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_paraformer_infer.py` & `gxl_ai_utils-1.3.5/eggs/knowledge_distillation/gxl_paraformer_infer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/gxl_whisper_infer.py` & `gxl_ai_utils-1.3.5/eggs/knowledge_distillation/gxl_whisper_infer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/handle_cmvn_gxl.py` & `gxl_ai_utils-1.3.5/eggs/knowledge_distillation/handle_cmvn_gxl.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer/encoder.py` & `gxl_ai_utils-1.3.5/eggs/knowledge_distillation/paraformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/paraformer_infer.py` & `gxl_ai_utils-1.3.5/eggs/knowledge_distillation/paraformer_infer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/knowledge_distillation/whisper_ctc/main.py` & `gxl_ai_utils-1.3.5/eggs/knowledge_distillation/whisper_ctc/main.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/spider_lizhi_fm.py` & `gxl_ai_utils-1.3.5/eggs/spider/spider_lizhi_fm.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/spider_qingting_fm.py` & `gxl_ai_utils-1.3.5/eggs/spider/spider_qingting_fm.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/spider_qingting_fm_new.py` & `gxl_ai_utils-1.3.5/eggs/spider/spider_qingting_fm_new.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/spider_voicewiki.py` & `gxl_ai_utils-1.3.5/eggs/spider/voicewiki/spider_voicewiki.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import glob
 import os
 
 import tqdm
 import sys
-sys.path.insert(0,"../../")
+sys.path.insert(0, "../../../")
 from urllib.parse import unquote
 from gxl_ai_utils.utils import utils_spider, utils_file
 
 SAVE_DIR = '/home/work_nfs14/xlgeng/tts_data_pachong_high_quality/voicewiki_gxl/'
 # SAVE_DIR = './output/voicewiki_gxl/'
 utils_file.makedir(SAVE_DIR)
 
@@ -373,14 +373,17 @@
                 continue
 
 
 class Huangshizhanzheng_spider:
     """
     皇室战争
     """
+
+
+
 if __name__ == '__main__':
     """"""
     # wangzherongyao = WangZhe_spider()
     # wangzherongyao.get_all_result_and_cat()
     save_dir = ''
     res_path_list = glob.glob(os.path.join("/home/work_nfs14/xlgeng/tts_data_pachong_high_quality/voicewiki/audio4persons/侠盗猎车手：罪恶都市", '*file_path.jsonl'))
     utils_file.print_list(res_path_list)
```

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/spider_ximalaya.py` & `gxl_ai_utils-1.3.5/eggs/spider/spider_ximalaya.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/spider_ximalaya_new.py` & `gxl_ai_utils-1.3.5/eggs/spider/spider_ximalaya_new.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/spider_yunting.py` & `gxl_ai_utils-1.3.5/eggs/spider/spider_yunting.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/spider_zhihu.py` & `gxl_ai_utils-1.3.5/eggs/spider/spider_zhihu.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/spider_zhihu_2.py` & `gxl_ai_utils-1.3.5/eggs/spider/spider_zhihu_2.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/eggs/spider/test.py` & `gxl_ai_utils-1.3.5/eggs/spider/test.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/AiConstant.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/AiConstant.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/__init__.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/build_vocab.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/build_vocab.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/classify/data_handler.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/classify/data_handler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/common_data_handler.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/common_data_handler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/gxl_data_handler.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/gxl_data_handler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_dataset/recognition/data_handler.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_dataset/recognition/data_handler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/ecapa_tdnn.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/classify/ecapa_tdnn.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/classify/xvector.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/classify/xvector.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/deepspeech2/deepspeech2.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/deepspeech2/deepspeech2.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/ctc_decoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/modules/ctc_decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/embedding.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/modules/subsampling.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/multi_head_attention.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_encoding.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_wise_feed_forward.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/positional_wise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/competition/scaled_dot_product_attention.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/competition/scaled_dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/decoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/model/utils/padding_mask.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/model/utils/padding_mask.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/transformer/transformer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/audio_model/s2t/utils/ctc_utils.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/audio_model/s2t/utils/ctc_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/config/gxl_config.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/config/gxl_config.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/gxl_dataset.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_dataset_wenet/gxl_dataset.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_dataset_wenet/gxl_processor.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_dataset_wenet/gxl_processor.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/alignment.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/alignment.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/average_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/average_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/gxl_infer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/gxl_infer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/recognize.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/recognize.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_infer_wenet/recognize_onnx_gpu.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_infer_wenet/recognize_onnx_gpu.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_lr_scheduler_wenet/scheduler.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_lr_scheduler_wenet/scheduler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/cgmlp.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/branchformer/cgmlp.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/branchformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/branchformer/encoder_layer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/branchformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/cif/predictor.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/cif/predictor.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder_layer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/e_branchformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/attention.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/convolution.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/convolution.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder_layer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/efficient_conformer/subsampling.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/efficient_conformer/subsampling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/init_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/init_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/k2/model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/k2/model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/attention.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/cif.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/cif.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/convert_paraformer_to_wenet_config.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/convert_paraformer_to_wenet_config.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/layers.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/layers.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/paraformer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/paraformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/paraformer/search.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/paraformer/search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/attention.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/conv2d.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/conv2d.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/convolution.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/convolution.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder_layer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/positionwise_feed_forward.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/squeezeformer/subsampling.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/squeezeformer/subsampling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/joint.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/joint.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/predictor.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/predictor.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/greedy_search.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/search/greedy_search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/search/prefix_beam_search.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/search/prefix_beam_search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transducer/transducer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transducer/transducer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/asr_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/asr_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/attention.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/attention.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/cmvn.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/cmvn.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/convolution.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/convolution.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/ctc.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/ctc.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/decoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/decoder_layer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/embedding.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/embedding.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/encoder_layer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/label_smoothing_loss.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/positionwise_feed_forward.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/search.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/search.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/subsampling.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/subsampling.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/swish.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/swish.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_decoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/whisper_decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder_gxl.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/transformer/whisper_encoder_gxl.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/checkpoint.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/cmvn.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/cmvn.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/common.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/common.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/config.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/config.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/context_graph.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/context_graph.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/ctc_utils.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/ctc_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/executor.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/executor.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/file_utils.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/init_ali_paraformer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/init_ali_paraformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/init_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/init_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/mask.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/mask.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/scheduler.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/tokenize_utils.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/tokenize_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/utils/train_utils.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/attentions.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/attentions.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/commons.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/commons.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/models.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/models.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_model_wenet/vits/modules.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_model_wenet/vits/modules.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_trainer_wenet/gxl_trainer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_trainer_wenet/gxl_trainer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/__init__.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/__init__.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/audio.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/decoding.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/decoding.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/basic.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/normalizers/basic.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/normalizers/english.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/normalizers/english.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/timing.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/tokenizer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/transcribe.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/transcribe.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/triton_ops.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/triton_ops.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/gxl_whisper/utils.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/gxl_whisper/utils.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/asr/encoder/conformer_encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/asr/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/fastformer/fastformer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/fastformer/fastformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/build_asr_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/build_asr_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/e2e_asr_paraformer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/sanm_decoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/paraformer/sanm_encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/paraformer/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/component.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/component.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/decoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/encoder.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/model_warehouse/transformer/transformer.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/model_warehouse/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/run/base_train_runner.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/run/base_train_runner.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/flask_predict.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/run/flask_template/flask_predict.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/run/flask_template/flask_server.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/run/flask_template/flask_server.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/run/runner.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner_multi_template.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/run/runner_multi_template.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/run/runner_single_template.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/run/runner_single_template.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_data.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/store_data.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/store_data/store_dataset/store_dataset.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/store_data/store_dataset/store_dataset.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/attention_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/attention_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/cnn_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/cnn_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/mlp_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/mlp_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/rnn_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/rnn_model.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_class/store_model_class.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_class/store_model_class.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/store_model/store_model_name.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/store_model/store_model_name.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/thread/my_thread.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/thread/my_thread.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_data.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_data.py`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_file.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,42 @@
 import random
 import shutil
 import sys
 import tarfile
 import time
 import urllib
 import warnings
+from collections import defaultdict
 from pathlib import Path
 from datetime import datetime
 import re
 import codecs
-from typing import Optional
+from typing import Optional, Dict, List, Tuple, Any
 
 import jsonlines
 import numpy as np
 import requests
 import torch
 import torchaudio
 import yaml
 import types
 import wave
 from torch import nn
 from tqdm import tqdm
 from ..thread.my_thread import GxlDynamicThreadPool, GxlFixedThreadPool
 
 HAS_SET_LOGGING = False
+from .utils_file_2 import *
+
+sys.path.insert(0, '/home/work_nfs8/xlgeng/new_workspace/icefall')
+try:
+    from lhotse.recipes.utils import read_manifests_if_cached
+    from icefall.utils import get_executor, str2bool
+except ImportError:
+    pass
 
 
 # GLOGGER: logging.Logger = None
 def set_logging():
     """
     设置日志输出的格式
     :return: 
@@ -94,14 +103,18 @@
 
 def load_list_file_clean(path: str):
     """
     得到不包含换行符的str_list
     :param path:
     :return:
     """
+    if not os.path.exists(path):
+        logging_print(f'load_list_file_clean()_{path}文件不存在')
+        return []
+
     with codecs.open(path, 'r', encoding='utf=8') as f:
         cat_to_name: list = f.read().splitlines()
         # cat_to_name: list = f.readlines() -> 包含换行符
         logging_print(f"load_list_file_clean()_数据总条数为:{len(cat_to_name)}")
     return cat_to_name
 
 
@@ -138,14 +151,15 @@
         cat_to_name: dict = json.load(f)
         logging_print("load_dict_from_json()_数据总条数为:", len(cat_to_name))
     return cat_to_name
 
 
 def load_dict_list_from_jsonl(jsonl_file_path) -> list:
     """"""
+    logging_print("开始执行: load_dict_list_from_jsonl")
     with codecs.open(jsonl_file_path, 'r', encoding='utf-8') as f:
         lines = f.readlines()
         lines_res = []
         for line in lines:
             try:
                 line = json.loads(line)
                 lines_res.append(line)
@@ -168,16 +182,17 @@
         except Exception as e:
             print(e)
             return {}
         for line in lines:
             line = line.strip()
             items = line.split()
             if len(items) < 2:
-                logging_print('load_dict_from_scp;warning_gxl:, this row not conform to the regulation of scp(key content) and skip it:',
-                              line)
+                logging_print(
+                    'load_dict_from_scp;warning_gxl:, this row not conform to the regulation of scp(key content) and skip it:',
+                    line)
                 continue
             elif len(items) == 2:
                 res[items[0].strip()] = items[1].strip()
             else:
                 # logging_print(
                 #     'warning_gxl:, this row not conform to the regulation of'
                 #     ' scp(key content) and no skip it,第一个为key,剩下的都是value:',
@@ -247,14 +262,20 @@
 
 
 def write_single_dict_to_jsonl(dic, jsonl_file_path):
     with jsonlines.open(jsonl_file_path, mode='a') as f:
         f.write(dic)
 
 
+def do_remove_last_slash(file_path):
+    if file_path[-1] == '/':
+        file_path = file_path[:-1]
+    return file_path
+
+
 def write_dict_to_scp(dic: dict, scp_file_path: str):
     logging_print("write_dict_to_scp()_数据总条数为:", len(dic))
     os.makedirs(os.path.dirname(scp_file_path), exist_ok=True)
     with codecs.open(scp_file_path, 'w', encoding='utf-8') as f:
         for k, v in dic.items():
             f.write(f"{k} {v}\n")
 
@@ -316,14 +337,17 @@
     while path1[-1] == '/' or path1[-1] == '\\':
         path1 = path1[:-1]
     while path2[0] == '/' or path2[0] == '\\':
         path2 = path2[1:]
     return f'{path1}/{path2}'
 
 
+# def join_path(*args):
+#     os.path.join(*args)
+
 def join_path(*args):
     """
     安全拼接若干路径, 再也不用担心分路径结尾和开头的分隔符的困扰了
     """
     lens = len(args)
     if lens == 0:
         return ""
@@ -344,20 +368,22 @@
     text_dic = load_dict_from_scp(text_scp_file_path)
     if len(wav_dic) != len(text_dic):
         logging_print("warning: wav_scp文件和text_scp文件长度不一致")
     if target_jsonl_file_path is not None:
         makedir_for_file(target_jsonl_file_path)
         if os.path.exists(target_jsonl_file_path):
             os.remove(target_jsonl_file_path)
-        for k, v in wav_dic.items():
+        res_dict_list = []
+        for k, v in tqdm(wav_dic.items(), desc='do_convert_wav_text_scp_to_jsonl', total=len(wav_dic)):
             if k not in text_dic:
                 logging_print('warning: {} not in text_dic'.format(k))
                 continue
             text = text_dic[k]
-            write_single_dict_to_jsonl({'key': k, 'wav': v, 'txt': text}, target_jsonl_file_path)
+            res_dict_list.append({'key': k, 'wav': v, 'txt': text})
+        write_dict_list_to_jsonl(res_dict_list, target_jsonl_file_path)
     else:
         res_list = []
         for k, v in wav_dic.items():
             if k not in text_dic:
                 logging_print('warning: {} not in text_dic'.format(k))
                 continue
             text = text_dic[k]
@@ -829,29 +855,73 @@
         keyword = keyword.lower()
         for key, i in self.index_dict.items():
             if keyword in key:
                 right_dict[key] = i
         print_dict(right_dict)
 
 
-def copy_file(source_path, destination_path):
+def copy_file(source_path, destination_path, buffer_size=1024 * 6, use_shell=False, visualization=True):
+    makedir_for_file(destination_path)
+    if use_shell:
+        _copy_file_shell(source_path, destination_path)
+    else:
+        if visualization:
+            #  6 * 1024 较佳， 750-800MB/s的传输速度, 但没有shell快，略逊于shell(6*1024)
+            _copy_file_visualization(source_path, destination_path, buffer_size)
+        else:
+            _copy_file_no_visualization(source_path, destination_path)
+
+
+def _copy_file_shell(source_path, destination_path):
+    command_line = f"cp {source_path} {destination_path}"
+    os.system(command_line)
+
+
+def _copy_file_visualization(source_path, destination_path, buffer_size=64):
+    buffer_size = buffer_size * 1024
+    logging_print(f'正在复制文件...从 {source_path} 到 {destination_path}')
+    try:
+        """"""
+        with open(source_path, 'rb') as source_file, open(destination_path, 'wb') as destination_file:
+            # 获取源文件的总大小，用于进度条的设置
+            source_size = os.path.getsize(source_path)
+            # 创建进度条
+            with tqdm(total=source_size, unit='B', unit_scale=True, desc=f"正在复制") as pbar:
+                # 流式复制文件内容，同时更新进度条
+                while True:
+                    # 读取缓冲区大小的内容
+                    content = source_file.read(buffer_size)
+                    if not content:
+                        break
+                    # 写入到目标文件
+                    destination_file.write(content)
+                    # 更新进度条
+                    pbar.update(len(content))
+        print(f"文件 {source_path} 已成功复制到 {destination_path}")
+    except Exception as e:
+        print(f"复制文件时发生错误：{e}")
+
+
+def _copy_file_no_visualization(source_path, destination_path):
     makedir_sil(os.path.dirname(destination_path))
+    logging_print(f'正在复制文件...从 {source_path} 到 {destination_path}')
     try:
         with open(source_path, 'rb') as source_file:
             content = source_file.read()
 
         with open(destination_path, 'wb') as destination_file:
             destination_file.write(content)
 
         print(f"文件 {source_path} 已成功复制到 {destination_path}")
     except Exception as e:
         print(f"复制文件时发生错误：{e}")
 
 
 def copy_file2(source_path, target_dir, is_jump=False):
+    makedir_sil(target_dir)
     # 获取源文件的文件名
     file_name = os.path.basename(source_path)
     # 拼接目标文件的完整路径
     destination_file = os.path.join(target_dir, file_name)
     if is_jump:
         if os.path.exists(destination_file):
             logging_print(f"is_jump=True，{destination_file} 已经存在，跳过复制")
@@ -1003,21 +1073,24 @@
     pool.close()
     pool.join()
     logging_print('打shard结束, 保存shard列表')
     with open(os.path.join(output_dir, 'shards_list.txt'), 'w', encoding='utf8') as fout:
         for name in shards_list:
             fout.write(name + '\n')
     logging_print('打shard完全结束')
+    copy_file(wav_scp_file_path, os.path.join(output_dir, 'wav.scp'))
+    copy_file(text_scp_file_path, os.path.join(output_dir, 'text'))
 
 
 def get_random_subdict(source_dict: dict, num_value: int):
     keys = list(source_dict.keys())
     random.shuffle(keys)
     return {key: source_dict[key] for key in keys[:num_value]}
 
+
 def do_get_random_subdict(source_dict: dict, num_value: int):
     keys = list(source_dict.keys())
     random.shuffle(keys)
     return {key: source_dict[key] for key in keys[:num_value]}
 
 
 def get_subdict(source_dict: dict, start_i, end_i):
@@ -1152,15 +1225,16 @@
     chars_set = set()
     for value in tqdm(text_dict.values(), total=len(text_dict), desc='提取chars_dictionary'):
         for char_i in value:
             chars_set.add(char_i)
     with codecs.open(dict_file_path, 'w', encoding='utf-8') as f:
         f.write(f'{blank_sym} 0\n')
         f.write('<unk> 1\n')
-        f.write('<sos/eos> 2\n')
+        f.write('<sos> 2\n')
+        f.write('<eos> 2\n')
         for i, char in enumerate(sorted(chars_set)):
             f.write(f'{char} {i + 3}\n')
 
 
 def get_sample_count(audio_file_path: str):
     """
     得到路径所指音频的采样点数
@@ -1210,15 +1284,18 @@
 def remove_dir(directory_to_delete):
     """递归删除一整个目录"""
     logging_print('remove_dir():开始删除目录:%s' % directory_to_delete)
     shutil.rmtree(directory_to_delete)
     logging_print('remove_dir():目录结束删除:%s' % directory_to_delete)
 
 
-def do_compress_file_by_gzip(input_file, output_file):
+def do_compress_file_by_gzip(input_file, output_file=None):
+    if output_file is None:
+        output_file = input_file + '.gz'
+
     logging_print(f'开始使用gzip压缩文件：{input_file},压缩到:{output_file}')
     with open(input_file, 'rb') as f_in:
         with gzip.open(output_file, 'wb') as f_out:
             f_out.writelines(f_in)
     logging_print(f'完成使用gzip压缩文件：{input_file},压缩到:{output_file}')
 
 
@@ -1262,22 +1339,16 @@
         CutSet,
         Fbank,
         FbankConfig,
         LilcomChunkyWriter,
         WhisperFbank,
         WhisperFbankConfig,
     )
-    from lhotse.recipes.utils import read_manifests_if_cached
-    sys.path.insert(0, '/home/work_nfs8/xlgeng/new_workspace/icefall')
-    try:
-        from icefall.utils import get_executor, str2bool
-    except ImportError:
-        pass
-    torch.set_num_threads(1)
-    torch.set_num_interop_threads(1)
+    # torch.set_num_threads(1)
+    # torch.set_num_interop_threads(1)
     makedir_sil(fbank_dir)
     src_dir = Path(manifests_dir)
     output_dir = Path(fbank_dir)
     num_jobs = min(15, os.cpu_count())
     dataset_parts = (
         f"{partition}",
     )
@@ -1325,18 +1396,19 @@
                 num_jobs=num_jobs if ex is None else 80,
                 executor=ex,
                 storage_type=LilcomChunkyWriter,
             )
             cut_set.to_file(output_dir / f"{prefix}_cuts_{partition}.{suffix}")
 
 
-def _do_convert_scp_to_manifest4icefall(wav_scp_path, text_scp_path, wav_manifest_path, text_manifest_path):
+def _do_convert_scp_to_manifest4icefall(wav_scp_path, text_scp_path, wav_manifest_path, text_manifest_path,
+                                        num_thread=8):
     def build_wav_dict_for_icefall(key, input_wav_path):
         sample_num, sample_rate = get_sample_count(input_wav_path)
-        # file_name = utils_file.get_file_pure_name_from_path(input_wav_path)
+        # file_name = get_file_pure_name_from_path(input_wav_path)
         duration = sample_num / sample_rate
         res_dict = {}
         res_dict['id'] = key
         res_dict['sources'] = [dict(
             type='file',
             channels=[0],
             source=input_wav_path,
@@ -1345,61 +1417,61 @@
         res_dict['num_samples'] = sample_num
         res_dict['duration'] = duration
         res_dict['channel_ids'] = [0]
         return res_dict
 
     def build_text_dict_for_icefall(key, input_text_str, duration_dict):
         if key not in duration_dict:
-            # utils_file.logging_print('key not in duration dict,也就是text中有的key wav.scp没有: ' + key)
+            # logging_print('key not in duration dict,也就是text中有的key wav.scp没有: ' + key)
             return {}
         res_dict = {}
         res_dict['id'] = key
         res_dict['recording_id'] = key
         res_dict['start'] = 0.0
         res_dict['duration'] = duration_dict[key]
         res_dict['channel'] = 0
         res_dict['text'] = input_text_str
         res_dict['language'] = 'Chinese'
         res_dict['speaker'] = 'S0901'
         return res_dict
 
     def little_func4wav_convert(res_list, wav_dict):
         temp_list = []
-        for key, wav_path in tqdm.tqdm(wav_dict.items(), total=len(wav_dict)):
+        for key, wav_path in tqdm(wav_dict.items(), total=len(wav_dict)):
             temp_list.append(build_wav_dict_for_icefall(key, wav_path))
         res_list.extend(temp_list)
 
     def little_func4text_convert(res_list, wav_dict, duration_dict):
         temp_list = []
-        for key, wav_path in tqdm.tqdm(wav_dict.items(), total=len(wav_dict)):
+        for key, wav_path in tqdm(wav_dict.items(), total=len(wav_dict)):
             temp_dict = build_text_dict_for_icefall(key, wav_path, duration_dict)
             if len(temp_dict) > 0:
                 temp_list.append(temp_dict)
         res_list.extend(temp_list)
 
     logging_print('开始 do_convert_scp_to_manifest4icefall')
     makedir_for_file(wav_manifest_path)
     makedir_for_file(text_manifest_path)
     wav_dict = load_dict_from_scp(wav_scp_path)
     res_wav_dict_list = []
     runner = GxlDynamicThreadPool()
-    wav_dict_list = do_split_dict(wav_dict, 32)
+    wav_dict_list = do_split_dict(wav_dict, num_thread)
     for wav_dict_i in wav_dict_list:
         runner.add_task(little_func4wav_convert, [res_wav_dict_list, wav_dict_i])
     logging_print('do_convert_scp_to_manifest():开始执行为wav生成manifest')
     runner.start()
     write_dict_list_to_jsonl(res_wav_dict_list, wav_manifest_path)
     wav_manifest_path_gz = wav_manifest_path + '.gz'
     do_compress_file_by_gzip(wav_manifest_path, wav_manifest_path_gz)
-    # res_wav_dict_list = utils_file.load_dict_list_from_jsonl(wav_manifest_path)
+    # res_wav_dict_list = load_dict_list_from_jsonl(wav_manifest_path)
 
     # 得到duration信息的字典
     logging_print('do_convert_scp_to_manifest():开始生成duration字典')
     duration_dict = {}
-    for dict_i in tqdm.tqdm(res_wav_dict_list, total=len(res_wav_dict_list)):
+    for dict_i in tqdm(res_wav_dict_list, total=len(res_wav_dict_list)):
         id = dict_i['id']
         duration = dict_i['duration']
         duration_dict[id] = duration
     logging_print('do_convert_scp_to_manifest():生成duration字典完成')
 
     res_text_dict_list = []
     text_dict = load_dict_from_scp(text_scp_path)
@@ -1410,19 +1482,23 @@
     logging_print('do_convert_scp_to_manifest():开始执行为text生成manifest')
     runner.start()
     write_dict_list_to_jsonl(res_text_dict_list, text_manifest_path)
     text_manifest_path_gz = text_manifest_path + '.gz'
     do_compress_file_by_gzip(text_manifest_path, text_manifest_path_gz)
 
 
+def get_jsonl_filename4icefall(prefix: str = 'gxldata', partition: str = 'train'):
+    return f'{prefix}_recordings_{partition}.jsonl', f'{prefix}_supervisions_{partition}.jsonl'
+
+
 def do_make_data4icefall(wav_scp_path,
                          text_scp_path,
                          manifest_dir=None,
                          fbank_dir=None,
-                         parent_dir= None,
+                         parent_dir=None,
                          partition: str = 'train',
                          prefix: str = 'gxldata',
                          only_manifest: bool = False,
                          only_fbank: bool = False):
     """
 
     :param wav_scp_path:
@@ -1430,19 +1506,18 @@
     :param manifest_dir:
     :param fbank_dir:
     :param parent_dir: 如果设置了parent_dir,则manifest_dir 和 fbank_dir无效, 使用parent_dir和默认的目录名
     :param partition:
     :param prefix:
     :return:
     """
-
-    def get_jsonl_filename4icefall(prefix: str = 'gxldata', partition: str = 'train'):
-        return f'{prefix}_recordings_{partition}.jsonl', f'{prefix}_supervisions_{partition}.jsonl'
-
     logging_print('开始处理{}的数据'.format(partition))
+    if parent_dir is not None:
+        manifest_dir = os.path.join(parent_dir, 'manifest')
+        fbank_dir = os.path.join(parent_dir, 'fbank')
     makedir_sil(manifest_dir)
     makedir_sil(fbank_dir)
     if not only_fbank:
         logging_print('首先得到manifest,文件为.jsonl.gz')
         manifest_wav_filename, manifest_text_filename = get_jsonl_filename4icefall(prefix, partition)
         manifest_wav_path = os.path.join(manifest_dir, manifest_wav_filename)
         manifest_text_path = os.path.join(manifest_dir, manifest_text_filename)
@@ -1460,7 +1535,81 @@
             prefix=prefix,
             perturb_speed=(partition == 'train')
         )
         logging_print('生成fbank完成')
     else:
         logging_print(f'only_manifest={only_manifest}')
         return
+
+
+class GxlTimer:
+    def __init__(self):
+        self.start_time = None
+        self.end_time = None
+        self.start()
+
+    def start(self):
+        """Start the timer."""
+        self.start_time = time.time()
+
+    def stop(self):
+        """Stop the timer."""
+        self.end_time = time.time()
+
+    def stop_halfway(self, is_sec=True):
+        self.stop()
+        elapsed_time = self.elapsed_time()
+        self.start()
+        logging_print(f"Elapsed time: {elapsed_time}")
+        if is_sec:
+            return elapsed_time / 1000
+        return elapsed_time
+
+    def elapsed_time(self):
+        """Return the elapsed time in seconds."""
+        if self.start_time is None:
+            raise ValueError("Timer has not been started")
+        if self.end_time is None:
+            raise ValueError("Timer has not been stopped")
+        return self.end_time - self.start_time
+
+
+def hello_gxl():
+    print('hello gxl')
+
+
+def do_extract_gz(file_path, output_dir):
+    # 创建目标目录（如果不存在）
+    os.makedirs(output_dir, exist_ok=True)
+
+    # 打开.gz文件并解压到目标目录
+    with gzip.open(file_path, 'rb') as f_in:
+        file_name = os.path.basename(file_path)
+        output_file_path = os.path.join(output_dir, os.path.splitext(file_name)[0])
+        with open(output_file_path, 'wb') as f_out:
+            shutil.copyfileobj(f_in, f_out)
+
+
+class LimitPrinter:
+    def __init__(self):
+        self.max = 300
+        self.now = 0
+
+    def print(self, *args):
+        text = ' '.join([str(x) for x in args])
+        if self.now < self.max:
+            logging_print("LIMIT_PRINT: ", text)
+            self.now += 1
+
+    def set_max(self, max_in):
+        self.max = max_in
+
+    def reset(self):
+        self.now = 0
+
+
+global_limit_printer = LimitPrinter()
+
+
+def logging_limit_print(*text):
+    global global_limit_printer
+    global_limit_printer.print(*text)
```

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_model.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os.path
 import random
 
-import dataclasses
 
-import netron
 import numpy as np
 import torch
 from torch import nn
 import time
 
 
 def set_parameter_requires_grad(model, feature_extracting):
@@ -119,15 +117,15 @@
     assert len(kernel_sizes) > 0 and len(strides) > 0
     res = kernel_sizes[0]
     for kernel_size, stride in zip(kernel_sizes[1:], strides[1:]):
         res = (kernel_size - 1) * stride + res
     return res
 
 
-@dataclasses.dataclass
+
 class FormalCheckpoint:
     model_name: str
     model_state_dict: dict
     optimizer_state_dict: dict
     scheduler_state_dict: dict
     epoch: int
     step: int
@@ -179,14 +177,15 @@
     model.load_state_dict(params_ready)
     optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
     scheduler.load_state_dict(checkpoint['scheduler_state_dict'])
     return epoch, step
 
 
 def get_model_structure_chart_by_netron(model: torch.nn.Module, input_data: torch.Tensor):
+    import netron
     onnx_path = "./onnx_model_name.onnx"
     torch.onnx.export(model, input_data, onnx_path)
     netron.start(onnx_path)
 
 
 def make_freeze_all_params(model):
     for param in model.parameters():
```

### Comparing `gxl_ai_utils-1.3.4/gxl_ai_utils/utils/utils_spider.py` & `gxl_ai_utils-1.3.5/gxl_ai_utils/utils/utils_spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os
 import time
 import traceback
 from enum import Enum
 
-import requests
-from lxml import etree
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
+try:
+    import requests
+    from lxml import etree
+    from selenium import webdriver
+    from selenium.webdriver.chrome.options import Options
+    from selenium.webdriver.common.by import By
+except Exception as e:
+    print(e)
 
 COMMON_HEADER = {
     "Accept": "text.txt/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
     "Accept-Encoding": "gzip, deflate, br",
     "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
     "Cache-Control": "max-age=0",
     "Connection": "keep-alive",
```

### Comparing `gxl_ai_utils-1.3.4/license.txt` & `gxl_ai_utils-1.3.5/license.txt`

 * *Files identical despite different names*

### Comparing `gxl_ai_utils-1.3.4/setup.py` & `gxl_ai_utils-1.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # from distutils.core import setup
 from setuptools import setup, find_packages
 
 # packages = ['gxl_ai_utils', 'gxl_ai_utils.utils',
 #             'gxl_ai_utils.config', 'gxl_ai_utils.run',
 #             'gxl_ai_utils.thread' ]
 setup(name='gxl_ai_utils',
-      version='1.3.4',
+      version='1.3.5',
       author='Xuelong Geng',
-      description='这个是耿雪龙的工具包模块, update time: 2024-4-9',
+      description='这个是耿雪龙的工具包模块, update time: 2024-5-24',
       author_email='3349495429@qq.com',
       packages=find_packages(),
       package_dir={'requests': 'requests'}, )
```


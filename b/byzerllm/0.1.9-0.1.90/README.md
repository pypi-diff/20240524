# Comparing `tmp/byzerllm-0.1.9.tar.gz` & `tmp/byzerllm-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byzerllm-0.1.9.tar", last modified: Sat Oct 14 14:43:15 2023, max compression
+gzip compressed data, was "byzerllm-0.1.90.tar", last modified: Fri May 24 09:09:44 2024, max compression
```

## Comparing `byzerllm-0.1.9.tar` & `byzerllm-0.1.90.tar`

### file list

```diff
@@ -1,502 +1,583 @@
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      762 2023-10-14 14:43:15.219375 byzerllm-0.1.9/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      449 2023-10-11 00:54:35.000000 byzerllm-0.1.9/README.md
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       38 2023-10-14 14:43:15.219375 byzerllm-0.1.9/setup.cfg
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1254 2023-05-15 03:02:58.000000 byzerllm-0.1.9/setup.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.179374 byzerllm-0.1.9/src/
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3025 2023-09-11 11:02:01.000000 byzerllm-0.1.9/src/byzerllm/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/alpha_moss/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29048 2023-07-07 08:01:34.000000 byzerllm-0.1.9/src/byzerllm/alpha_moss/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/apps/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      466 2023-07-04 14:50:28.000000 byzerllm-0.1.9/src/byzerllm/apps/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3942 2023-09-06 06:02:21.000000 byzerllm-0.1.9/src/byzerllm/apps/builder.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3350 2023-09-06 06:06:45.000000 byzerllm-0.1.9/src/byzerllm/apps/client.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6276 2023-09-06 06:07:35.000000 byzerllm-0.1.9/src/byzerllm/apps/qa.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4934 2023-09-01 16:22:38.000000 byzerllm-0.1.9/src/byzerllm/apps/qa_strategy.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1687 2023-09-06 06:19:12.000000 byzerllm-0.1.9/src/byzerllm/apps/vector_db.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/auto/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12154 2023-10-04 02:30:28.000000 byzerllm-0.1.9/src/byzerllm/auto/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7577 2023-07-31 02:07:12.000000 byzerllm-0.1.9/src/byzerllm/auto/backend_ds.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/baichuan/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4018 2023-09-12 08:55:25.000000 byzerllm-0.1.9/src/byzerllm/baichuan/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/bark/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4243 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/api.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.179374 byzerllm-0.1.9/src/byzerllm/bark/assets/
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.195374 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16794 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/announcer.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20316 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31724 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    59348 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25116 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33860 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38124 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    13436 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18980 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25436 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24420 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34820 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30604 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29324 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36364 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44044 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43564 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    53908 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31244 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23036 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26820 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28684 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33004 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    46604 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45268 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    52684 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    41268 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29964 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44148 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24796 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37964 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22716 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    50548 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29540 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24156 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29004 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21916 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42284 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42548 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45324 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36364 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32420 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    58492 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    49004 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34444 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30284 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    58652 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1943 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/readme.md
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    57852 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24260 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51668 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29164 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45748 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42924 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19676 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    54548 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22556 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24156 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21276 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35724 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23196 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28524 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26236 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34980 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25540 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22716 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25116 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26236 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25700 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25436 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45804 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25700 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    52204 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    50764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    49908 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45108 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    55932 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32524 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43244 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25860 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29804 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51404 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39404 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33804 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40788 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30444 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29644 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43724 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42708 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37644 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24420 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31244 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26716 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40788 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20260 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31140 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26556 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26340 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19196 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39564 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23140 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23196 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27884 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31140 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23676 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    41428 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38820 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30980 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27724 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36844 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26980 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28260 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28524 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39884 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28204 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44628 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22076 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28684 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33164 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    17220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25276 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20260 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28204 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20636 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19836 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29964 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    17436 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16156 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19676 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    54548 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22556 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3759 2023-08-26 08:52:44.000000 byzerllm-0.1.9/src/byzerllm/bark/bark_voice.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33373 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/generation.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     9139 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/model.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5955 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/model_fine.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/bge/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1022 2023-09-04 13:38:16.000000 byzerllm-0.1.9/src/byzerllm/bge/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/chatglm2/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2108 2023-08-31 04:23:44.000000 byzerllm-0.1.9/src/byzerllm/chatglm2/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/chatglm6b/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-04 03:55:05.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8182 2023-04-04 03:55:05.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/arguments.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21286 2023-05-04 08:53:10.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/finetune.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11575 2023-04-04 03:55:05.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/trainer_seq2seq.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3000 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/finetune.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1404 2023-05-12 05:48:30.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/infer.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      277 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16907 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/common.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7620 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/config.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6263 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/other.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11082 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/dolly/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-25 12:20:22.000000 byzerllm-0.1.9/src/byzerllm/dolly/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2029 2023-04-25 12:20:22.000000 byzerllm-0.1.9/src/byzerllm/dolly/consts.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1112 2023-04-25 12:45:20.000000 byzerllm-0.1.9/src/byzerllm/dolly/dolly_inference.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10065 2023-04-25 12:44:37.000000 byzerllm-0.1.9/src/byzerllm/dolly/generate.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12156 2023-04-25 12:27:32.000000 byzerllm-0.1.9/src/byzerllm/dolly/trainer.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/falcon/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4080 2023-09-12 08:34:55.000000 byzerllm-0.1.9/src/byzerllm/falcon/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/llama/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6141 2023-09-12 08:34:55.000000 byzerllm-0.1.9/src/byzerllm/llama/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/llama2/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6310 2023-09-12 08:34:55.000000 byzerllm-0.1.9/src/byzerllm/llama2/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/m3e/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      189 2023-07-16 01:34:12.000000 byzerllm-0.1.9/src/byzerllm/m3e/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/moss/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-06 15:03:50.000000 byzerllm-0.1.9/src/byzerllm/moss/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12657 2023-04-23 13:04:50.000000 byzerllm-0.1.9/src/byzerllm/moss/finetune_moss.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/moss/models/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-22 10:54:54.000000 byzerllm-0.1.9/src/byzerllm/moss/models/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5097 2023-05-19 09:07:29.000000 byzerllm-0.1.9/src/byzerllm/moss/models/configuration_moss.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6735 2023-04-23 12:11:45.000000 byzerllm-0.1.9/src/byzerllm/moss/models/custom_autotune.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31351 2023-04-23 12:11:45.000000 byzerllm-0.1.9/src/byzerllm/moss/models/modeling_moss.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18866 2023-04-23 12:11:45.000000 byzerllm-0.1.9/src/byzerllm/moss/models/quantization.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15952 2023-04-23 12:11:45.000000 byzerllm-0.1.9/src/byzerllm/moss/models/tokenization_moss.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16919 2023-06-26 08:47:30.000000 byzerllm-0.1.9/src/byzerllm/moss/moss_inference.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/processor/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      577 2023-08-14 06:44:47.000000 byzerllm-0.1.9/src/byzerllm/processor/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/qwen_vl_chat/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3579 2023-08-26 08:55:00.000000 byzerllm-0.1.9/src/byzerllm/qwen_vl_chat/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/records/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2893 2023-10-14 13:04:39.000000 byzerllm-0.1.9/src/byzerllm/records/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/saas/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-02 02:17:52.000000 byzerllm-0.1.9/src/byzerllm/saas/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/saas/azure_openai/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1724 2023-08-01 03:13:16.000000 byzerllm-0.1.9/src/byzerllm/saas/azure_openai/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/saas/chatglm/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2136 2023-06-27 05:23:44.000000 byzerllm-0.1.9/src/byzerllm/saas/chatglm/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/saas/sparkdesk/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5273 2023-06-27 05:38:38.000000 byzerllm-0.1.9/src/byzerllm/saas/sparkdesk/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6217 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/pipelines/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/pipelines/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4720 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1701 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1006 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/generation.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/models/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/models/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1260 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/models/diffusion.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      173 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/plugin.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1136 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/config.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3127 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/embeddings.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3567 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8214 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31226 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10680 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8276 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5247 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3104 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/utils.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      673 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/images.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/diffusers/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/diffusers/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1246 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      434 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/logger.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4681 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/model.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      540 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/shared.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      928 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/utils.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/starcode/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1553 2023-08-10 10:02:48.000000 byzerllm-0.1.9/src/byzerllm/starcode/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2422 2023-09-25 10:15:36.000000 byzerllm-0.1.9/src/byzerllm/store.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4838 2023-10-12 01:43:30.000000 byzerllm-0.1.9/src/byzerllm/utils/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/config/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1059 2023-10-04 03:01:23.000000 byzerllm-0.1.9/src/byzerllm/utils/config/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4042 2023-09-04 13:26:00.000000 byzerllm-0.1.9/src/byzerllm/utils/emb.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/fulltune/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2637 2023-06-30 09:41:26.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-28 06:59:34.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2929 2023-07-27 13:14:08.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30037 2023-07-27 13:14:08.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12755 2023-06-30 09:40:41.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/deepspeed_trainner.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4826 2023-06-29 13:00:23.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/launch.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28394 2023-09-19 06:47:44.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2406 2023-09-20 03:09:31.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6924 2023-06-29 02:54:39.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/trainner.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/inference/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3134 2023-07-11 13:03:47.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/inference/models/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10094 2023-07-08 03:06:41.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2699 2023-07-08 03:36:34.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/bloom.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21538 2023-07-08 03:28:59.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/causal_lm.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-08 03:03:28.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34973 2023-07-08 03:29:53.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/bloom_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11952 2023-07-08 03:32:19.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_llama_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12421 2023-07-08 03:35:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_neox_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19256 2023-07-08 03:45:37.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_rw_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15720 2023-07-08 03:35:18.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_santacoder_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44270 2023-07-08 03:35:23.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/mpt_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30556 2023-07-08 03:35:31.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/neox_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33490 2023-07-08 03:35:36.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/opt_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    47248 2023-07-08 03:35:42.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/t5_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40651 2023-07-10 05:08:26.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_causal_lm.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2405 2023-07-08 03:38:20.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_llama.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2081 2023-07-08 03:38:45.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_neox.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2035 2023-07-08 03:14:25.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_rw.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2584 2023-07-08 03:39:14.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_santacoder.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4457 2023-07-08 08:25:04.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/galactica.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2436 2023-07-08 03:40:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/gpt_neox.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3038 2023-07-08 03:23:26.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/model.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2504 2023-07-08 03:40:50.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/mpt.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2354 2023-07-08 03:41:08.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/opt.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3026 2023-07-08 03:41:14.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/rw.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2186 2023-07-08 03:41:23.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/santacoder.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23774 2023-07-08 03:42:39.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/seq2seq_lm.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2945 2023-07-08 03:43:05.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/t5.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6341 2023-07-11 09:12:44.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/types.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      886 2023-07-08 05:35:37.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3865 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/convert.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2163 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/dist.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-08 08:23:13.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10077 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/custom_autotune.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12464 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/quant_linear.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26942 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/quantize.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6251 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/hub.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    13654 2023-07-08 03:44:02.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/layers.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    14905 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/logits_process.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10645 2023-07-10 05:00:01.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/tokens.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3523 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/watermark.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5731 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/weights.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/metrics/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1216 2023-10-04 02:30:32.000000 byzerllm-0.1.9/src/byzerllm/utils/metrics/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      367 2023-10-09 11:02:19.000000 byzerllm-0.1.9/src/byzerllm/utils/object_store_ref_util.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/rayinfer/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4124 2023-07-22 10:08:11.000000 byzerllm-0.1.9/src/byzerllm/utils/rayinfer/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/retrieval/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6104 2023-10-14 14:11:39.000000 byzerllm-0.1.9/src/byzerllm/utils/retrieval/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6019 2023-10-14 14:35:52.000000 byzerllm-0.1.9/src/byzerllm/utils/retrieval/rest.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/sft/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10052 2023-09-18 01:54:43.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1203 2023-06-26 02:16:27.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/argument.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2029 2023-09-18 01:37:01.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/collator.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3248 2023-09-18 01:39:14.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/dataset.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1614 2023-06-25 10:28:20.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/loss.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2295 2023-09-13 09:14:56.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/merge_lora.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2611 2023-06-25 10:22:30.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/model.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8381 2023-10-03 02:06:56.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/qlora.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3395 2023-06-21 10:59:30.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/trainer.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1288 2023-09-18 08:24:25.000000 byzerllm-0.1.9/src/byzerllm/utils/testing.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7111 2023-09-18 16:23:56.000000 byzerllm-0.1.9/src/byzerllm/utils/text_generator.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       22 2023-10-14 14:42:41.000000 byzerllm-0.1.9/src/byzerllm/version.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/visualglm/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2462 2023-07-16 01:34:31.000000 byzerllm-0.1.9/src/byzerllm/visualglm/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/whisper/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-05-11 01:44:23.000000 byzerllm-0.1.9/src/byzerllm/whisper/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1254 2023-05-11 07:07:58.000000 byzerllm-0.1.9/src/byzerllm/whisper/whisper_inference.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm.egg-info/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      762 2023-10-14 14:43:15.000000 byzerllm-0.1.9/src/byzerllm.egg-info/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21231 2023-10-14 14:43:15.000000 byzerllm-0.1.9/src/byzerllm.egg-info/SOURCES.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-10-14 14:43:15.000000 byzerllm-0.1.9/src/byzerllm.egg-info/dependency_links.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        9 2023-10-14 14:43:15.000000 byzerllm-0.1.9/src/byzerllm.egg-info/top_level.txt
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.897934 byzerllm-0.1.90/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11558 2024-03-31 13:19:57.000000 byzerllm-0.1.90/LICENSE
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    83884 2024-05-24 09:09:44.897461 byzerllm-0.1.90/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    83553 2024-05-14 06:52:28.000000 byzerllm-0.1.90/README.md
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2024-05-24 09:09:44.898015 byzerllm-0.1.90/setup.cfg
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1377 2024-04-23 10:08:12.000000 byzerllm-0.1.90/setup.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.404599 byzerllm-0.1.90/src/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.443620 byzerllm-0.1.90/src/byzerllm/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16451 2024-05-24 08:57:11.000000 byzerllm-0.1.90/src/byzerllm/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.446900 byzerllm-0.1.90/src/byzerllm/alpha_moss/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29048 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/alpha_moss/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.451832 byzerllm-0.1.90/src/byzerllm/apps/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      466 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.456814 byzerllm-0.1.90/src/byzerllm/apps/agent/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5003 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2629 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28758 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/conversable_agent.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.469657 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6643 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/assistant_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3586 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/byzer_engine_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1725 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/common_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10177 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/data_analysis.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19116 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/data_analysis_pipeline_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4293 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/llama_index_retrieval_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5254 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/load_data_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2877 2023-12-19 05:48:54.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/output_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1598 2023-12-19 05:48:54.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/planner.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7840 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/preview_file_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8416 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/python_codesandbox_agent.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.473783 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      284 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3578 2024-01-19 04:16:39.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/condition.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2860 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/context.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3850 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/rhetorical.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2864 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/time.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7281 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/retrieval_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6494 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/rhetorical_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11826 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/simple_retrieval_client.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    14880 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/spark_sql_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4980 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/sql_reviewer_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4190 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/subquestion_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6760 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/visualization_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10100 2023-12-19 05:48:54.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/groupchat.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1071 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/registry.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.475814 byzerllm-0.1.90/src/byzerllm/apps/agent/store/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      439 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/store/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1307 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/store/memory_store.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1016 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/store/stores.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5584 2023-12-19 05:48:54.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/user_proxy_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3942 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/builder.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.476336 byzerllm-0.1.90/src/byzerllm/apps/byzer_sql/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6184 2024-05-14 06:51:51.000000 byzerllm-0.1.90/src/byzerllm/apps/byzer_sql/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.478990 byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-05-10 08:09:49.000000 byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8507 2024-05-10 09:06:58.000000 byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/command.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5747 2024-05-11 01:14:09.000000 byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/env.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3350 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/client.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.485509 byzerllm-0.1.90/src/byzerllm/apps/llama_index/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1506 2024-04-16 10:36:39.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4081 2024-05-14 09:17:42.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1218 2024-04-16 10:34:46.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_docstore.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1467 2024-04-22 02:58:54.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_embedding.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1199 2024-04-24 04:47:48.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_index_store.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4237 2024-04-24 05:29:47.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_kvstore.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6734 2024-04-25 06:57:07.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_vectordb.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2693 2024-05-01 12:00:48.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/collection_manager.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    14057 2024-04-24 05:31:49.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/simple_retrieval.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6276 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/qa.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4934 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/qa_strategy.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1687 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/vector_db.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.487823 byzerllm-0.1.90/src/byzerllm/auto/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20799 2024-05-06 06:30:19.000000 byzerllm-0.1.90/src/byzerllm/auto/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7577 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/auto/backend_ds.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10678 2024-04-26 07:58:28.000000 byzerllm-0.1.90/src/byzerllm/auto/backend_llama_cpp.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.488961 byzerllm-0.1.90/src/byzerllm/baichuan/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4370 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/baichuan/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.492664 byzerllm-0.1.90/src/byzerllm/bark/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4243 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/api.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.407679 byzerllm-0.1.90/src/byzerllm/bark/assets/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.666622 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16794 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/announcer.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20316 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31724 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    59348 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25116 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33860 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38124 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    15516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    13436 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18980 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25436 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24420 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34820 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30604 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29324 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    44044 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43564 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    53908 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31244 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23036 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26820 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28684 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33004 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    46604 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45268 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    52684 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    41268 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29964 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    44148 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24796 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    37964 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22716 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    50548 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29540 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29004 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21916 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42284 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42548 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45324 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    37380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32420 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    58492 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    49004 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34444 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30284 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    58652 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1943 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/readme.md
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    57852 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51668 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29164 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45748 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42924 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21276 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35724 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.794759 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23196 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    40100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28524 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26236 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34980 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25540 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22716 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25116 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26236 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25700 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25436 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45804 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25700 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    52204 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    50764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    49908 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45108 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    55932 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32524 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43244 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25860 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29804 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51404 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39404 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33804 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    40788 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30444 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29644 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43724 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42708 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    37644 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24420 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31244 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26716 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    40788 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31140 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26556 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26340 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19196 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39564 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23140 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23196 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27884 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31140 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23676 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    41428 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38820 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30980 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27724 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    36844 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26980 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28524 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39884 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28204 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    44628 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22076 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28684 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33164 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    17220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25276 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28204 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20636 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19836 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29964 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    17436 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16156 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3759 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/bark_voice.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33373 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/generation.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     9139 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/model.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5955 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/model_fine.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.795727 byzerllm-0.1.90/src/byzerllm/bge/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1022 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bge/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.796179 byzerllm-0.1.90/src/byzerllm/bge_rerank/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      929 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/bge_rerank/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5748 2024-05-11 00:58:40.000000 byzerllm-0.1.90/src/byzerllm/byzerllm_command.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.797088 byzerllm-0.1.90/src/byzerllm/chatglm2/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2439 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/chatglm2/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.799317 byzerllm-0.1.90/src/byzerllm/chatglm6b/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/arguments.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/finetune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/trainer_seq2seq.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.800872 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3000 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/finetune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1404 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/infer.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.803253 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      277 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16907 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/common.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/config.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6263 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/other.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11082 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7984 2024-05-11 00:58:29.000000 byzerllm-0.1.90/src/byzerllm/command_args.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.806188 byzerllm-0.1.90/src/byzerllm/dolly/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/consts.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1112 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/dolly_inference.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10065 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/generate.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12156 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/trainer.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.806769 byzerllm-0.1.90/src/byzerllm/falcon/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4414 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/falcon/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2362 2024-05-11 00:55:17.000000 byzerllm-0.1.90/src/byzerllm/lang.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.807395 byzerllm-0.1.90/src/byzerllm/llama/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6504 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/llama/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.807944 byzerllm-0.1.90/src/byzerllm/llama2/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6675 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/llama2/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2010 2024-04-01 10:03:54.000000 byzerllm-0.1.90/src/byzerllm/log.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.808623 byzerllm-0.1.90/src/byzerllm/m3e/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      189 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/m3e/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.810358 byzerllm-0.1.90/src/byzerllm/moss/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12657 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/finetune_moss.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.814472 byzerllm-0.1.90/src/byzerllm/moss/models/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5097 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/configuration_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6735 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/custom_autotune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31351 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/modeling_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18866 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/quantization.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    15952 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/tokenization_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16919 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/moss_inference.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.815208 byzerllm-0.1.90/src/byzerllm/processor/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      577 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/processor/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.815923 byzerllm-0.1.90/src/byzerllm/qwen/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6510 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/qwen/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.816540 byzerllm-0.1.90/src/byzerllm/qwen_vl_chat/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3792 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/qwen_vl_chat/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.817203 byzerllm-0.1.90/src/byzerllm/records/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6824 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/records/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.817953 byzerllm-0.1.90/src/byzerllm/saas/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/saas/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.818205 byzerllm-0.1.90/src/byzerllm/saas/aws_bedrock/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11871 2024-05-11 12:03:07.000000 byzerllm-0.1.90/src/byzerllm/saas/aws_bedrock/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.818872 byzerllm-0.1.90/src/byzerllm/saas/azure/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     9857 2024-05-11 11:58:25.000000 byzerllm-0.1.90/src/byzerllm/saas/azure/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.819524 byzerllm-0.1.90/src/byzerllm/saas/azure_openai/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3454 2024-05-11 11:57:58.000000 byzerllm-0.1.90/src/byzerllm/saas/azure_openai/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.820142 byzerllm-0.1.90/src/byzerllm/saas/baichuan/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5331 2024-05-11 11:56:58.000000 byzerllm-0.1.90/src/byzerllm/saas/baichuan/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.820759 byzerllm-0.1.90/src/byzerllm/saas/chatglm/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2306 2023-12-26 06:22:53.000000 byzerllm-0.1.90/src/byzerllm/saas/chatglm/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.821783 byzerllm-0.1.90/src/byzerllm/saas/claude/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5753 2024-05-11 11:54:49.000000 byzerllm-0.1.90/src/byzerllm/saas/claude/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.822338 byzerllm-0.1.90/src/byzerllm/saas/gemini/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4517 2024-05-11 11:54:20.000000 byzerllm-0.1.90/src/byzerllm/saas/gemini/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.823106 byzerllm-0.1.90/src/byzerllm/saas/minimax/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11064 2024-05-11 11:53:21.000000 byzerllm-0.1.90/src/byzerllm/saas/minimax/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.823726 byzerllm-0.1.90/src/byzerllm/saas/official_openai/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16675 2024-05-17 14:21:16.000000 byzerllm-0.1.90/src/byzerllm/saas/official_openai/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.824923 byzerllm-0.1.90/src/byzerllm/saas/openai/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       83 2024-04-14 14:38:04.000000 byzerllm-0.1.90/src/byzerllm/saas/openai/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.825684 byzerllm-0.1.90/src/byzerllm/saas/qianfan/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6147 2024-05-11 11:49:15.000000 byzerllm-0.1.90/src/byzerllm/saas/qianfan/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.826623 byzerllm-0.1.90/src/byzerllm/saas/qianwen/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6830 2024-05-11 11:42:52.000000 byzerllm-0.1.90/src/byzerllm/saas/qianwen/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.827518 byzerllm-0.1.90/src/byzerllm/saas/qianwen_vl/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7083 2024-05-17 14:16:35.000000 byzerllm-0.1.90/src/byzerllm/saas/qianwen_vl/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.828585 byzerllm-0.1.90/src/byzerllm/saas/sparkdesk/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6707 2024-05-11 11:47:59.000000 byzerllm-0.1.90/src/byzerllm/saas/sparkdesk/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.829234 byzerllm-0.1.90/src/byzerllm/saas/volcengine/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     9214 2024-05-11 11:50:42.000000 byzerllm-0.1.90/src/byzerllm/saas/volcengine/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.829910 byzerllm-0.1.90/src/byzerllm/saas/zhipu/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5039 2024-05-11 11:51:47.000000 byzerllm-0.1.90/src/byzerllm/saas/zhipu/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.834705 byzerllm-0.1.90/src/byzerllm/stable_diffusion/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6453 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.835785 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.836529 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.837393 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/pipelines/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/pipelines/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4720 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.839186 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1701 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1006 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/generation.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.840197 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/models/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/models/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/models/diffusion.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      173 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/plugin.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1136 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/config.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.841966 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3127 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/embeddings.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.843665 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3567 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8214 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.846622 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31226 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10680 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.848580 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8276 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5247 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3104 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      673 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/images.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.849264 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.849848 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/diffusers/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/diffusers/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1246 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      434 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/logger.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4681 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/model.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      540 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/shared.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      928 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/utils.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.850504 byzerllm-0.1.90/src/byzerllm/starcode/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1882 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/starcode/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2422 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/store.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.859448 byzerllm-0.1.90/src/byzerllm/utils/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25659 2024-04-26 09:09:23.000000 byzerllm-0.1.90/src/byzerllm/utils/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.865830 byzerllm-0.1.90/src/byzerllm/utils/client/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      884 2024-04-18 06:47:05.000000 byzerllm-0.1.90/src/byzerllm/utils/client/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    65237 2024-05-24 08:19:48.000000 byzerllm-0.1.90/src/byzerllm/utils/client/byzerllm_client.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19055 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/utils/client/code_utils.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.866783 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.872020 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8922 2024-04-18 09:44:41.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/api_server.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    14198 2024-04-01 10:03:54.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/protocol.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6707 2024-04-23 09:24:35.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serve.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8887 2024-04-26 08:07:36.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serving_chat.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7581 2024-04-26 08:08:28.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serving_completion.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5854 2024-04-23 05:50:42.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serving_engine.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8573 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/tool.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5777 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/utils/client/img_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10008 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/utils/client/math_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4275 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/utils/client/message_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1017 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/utils/client/parallel_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12377 2024-04-26 01:43:44.000000 byzerllm-0.1.90/src/byzerllm/utils/client/types.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.872773 byzerllm-0.1.90/src/byzerllm/utils/config/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1059 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/config/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2194 2024-05-10 09:22:55.000000 byzerllm-0.1.90/src/byzerllm/utils/connect_ray.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4042 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/emb.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.875888 byzerllm-0.1.90/src/byzerllm/utils/fulltune/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2637 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.877784 byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2929 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30037 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12755 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/deepspeed_trainner.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4826 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/launch.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.880158 byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28458 2023-12-23 13:24:00.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2406 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6924 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/trainner.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    14303 2024-04-08 04:52:43.000000 byzerllm-0.1.90/src/byzerllm/utils/json_repaire.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5187 2024-05-11 00:40:06.000000 byzerllm-0.1.90/src/byzerllm/utils/langutil.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.881024 byzerllm-0.1.90/src/byzerllm/utils/metrics/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1216 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/metrics/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      367 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/object_store_ref_util.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2346 2023-12-26 06:22:53.000000 byzerllm-0.1.90/src/byzerllm/utils/openai_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1446 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/ray_utils.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.883202 byzerllm-0.1.90/src/byzerllm/utils/retrieval/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    13613 2024-04-16 13:20:54.000000 byzerllm-0.1.90/src/byzerllm/utils/retrieval/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6019 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/utils/retrieval/rest.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1970 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/utils/retrieval/udf.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.888327 byzerllm-0.1.90/src/byzerllm/utils/sft/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10331 2023-12-23 13:24:00.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1203 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/argument.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/collator.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3248 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/dataset.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1614 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/loss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2295 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/merge_lora.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2611 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/model.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8381 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/qlora.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3395 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/trainer.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1288 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/testing.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10903 2024-05-11 01:56:39.000000 byzerllm-0.1.90/src/byzerllm/utils/text_generator.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1633 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/tokenizer.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5394 2024-04-27 05:50:08.000000 byzerllm-0.1.90/src/byzerllm/utils/types.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       23 2024-05-24 08:58:48.000000 byzerllm-0.1.90/src/byzerllm/version.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.888794 byzerllm-0.1.90/src/byzerllm/visualglm/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2462 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/visualglm/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.889617 byzerllm-0.1.90/src/byzerllm/whisper/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/whisper/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1254 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/whisper/whisper_inference.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.890269 byzerllm-0.1.90/src/byzerllm/zephyr/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5628 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/zephyr/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.896762 byzerllm-0.1.90/src/byzerllm.egg-info/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    83884 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23396 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/SOURCES.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/dependency_links.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       60 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/entry_points.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/top_level.txt
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.896155 byzerllm-0.1.90/tests/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1603 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_data_analysis.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3235 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_deepseek_code.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1248 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_deploy.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2041 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_emb_rerank.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1187 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_model_meta.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1413 2024-04-15 08:05:56.000000 byzerllm-0.1.90/tests/test_prompt.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3522 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_template.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_transformers_deploy.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1664 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_yi.py
```

### Comparing `byzerllm-0.1.9/setup.py` & `byzerllm-0.1.90/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 setup(
     name="byzerllm",
     version=__version__,
     description="ByzerLLM: Byzer LLM",
     author="allwefantasy",
     long_description=readme_contents,
     long_description_content_type="text/markdown",
+    entry_points={
+        'console_scripts': [
+            'byzerllm = byzerllm.byzerllm_command:main',
+        ],
+    },
     package_dir={"": "src"},
     packages=find_packages("src"),    
     package_data={
         "byzerllm":['bark/assets/**/*']
     },
     install_requires=install_requires,
     classifiers=[
```

### Comparing `byzerllm-0.1.9/src/byzerllm/alpha_moss/__init__.py` & `byzerllm-0.1.90/src/byzerllm/alpha_moss/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/apps/builder.py` & `byzerllm-0.1.90/src/byzerllm/apps/builder.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/apps/client.py` & `byzerllm-0.1.90/src/byzerllm/apps/client.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/apps/qa.py` & `byzerllm-0.1.90/src/byzerllm/apps/qa.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/apps/qa_strategy.py` & `byzerllm-0.1.90/src/byzerllm/apps/qa_strategy.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/apps/vector_db.py` & `byzerllm-0.1.90/src/byzerllm/apps/vector_db.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/auto/__init__.py` & `byzerllm-0.1.90/src/byzerllm/saas/aws_bedrock/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,270 +1,350 @@
-from transformers import AutoTokenizer, AutoModelForCausalLM,BitsAndBytesConfig
-import ray
-import torch
-import os
-import ray
-from typing import Any,Any,Dict, List,Tuple,Generator,Optional,Union
-import types
-
-from pyjava.api.mlsql import DataServer
-from byzerllm.utils.metrics import Metric
-from .. import BlockRow
-
-
-INFERENCE_NAME = "auto"
-INFER_TOKEN_METRICS = Metric()
-
-def stream_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
-        max_length:int=1024, 
-        top_p:float=0.95,
-        temperature:float=0.1,**kwargs):
-        
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    tokens = tokenizer(ins, return_token_type_ids=False,return_tensors="pt").to(device)
-    response = self.generate(
-        input_ids=tokens["input_ids"],
-        max_new_tokens=max_length,
-        repetition_penalty=1.05,
-        temperature=temperature,
-        attention_mask=tokens.attention_mask        
-    )
-    answer = tokenizer.decode(response[0][tokens["input_ids"].shape[1]:], skip_special_tokens=True)
-    return [(answer,"")]
-
-
-def ray_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
-        max_length:int=4096, 
-        top_p:float=0.95,
-        temperature:float=0.1,**kwargs):
-    from aviary.backend.server.models import Prompt
-    model = self
-    response = ray.get(model.generate_text.remote(prompt=Prompt(
-        prompt=ins,
-        use_prompt_format=False
-    ),request=None))
-    return [(response.generated_text,"")]
-
-async def async_vllm_chat(model,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
-        max_length:int=4096, 
-        top_p:float=0.95,
-        temperature:float=0.1,**kwargs):
-    from vllm import  SamplingParams
-    from vllm.utils import random_uuid
-    request_id = random_uuid()
-    
-    n: int = 1
-    best_of: Optional[int] =  kwargs["best_of"] if "best_of" in kwargs else None
-    presence_penalty: float = float(kwargs.get("presence_penalty",0.0))
-    frequency_penalty: float = float(kwargs.get("frequency_penalty",0.0))
-    top_k: int = int(kwargs.get("top_k",-1))
-    use_beam_search: bool = kwargs.get("use_beam_search","false") == "true"
-    stop: Union[None, str, List[str]] = kwargs["stop"] if "stop" in kwargs else None
-    ignore_eos: bool = kwargs.get("ignore_eos","false") == "true"
-    max_tokens: int = max_length
-    logprobs: Optional[int] = kwargs["logprobs"] if "logprobs" in kwargs else None
-    
-    sampling_params = SamplingParams(temperature=temperature, 
-                                     n = n,
-                                     best_of=best_of,
-                                     presence_penalty=presence_penalty,
-                                     frequency_penalty=frequency_penalty,
-                                     top_k=top_k,
-                                     use_beam_search=use_beam_search,
-                                     stop = stop,
-                                     ignore_eos=ignore_eos,
-                                     logprobs=logprobs,
-                                     top_p=top_p, 
-                                     max_tokens=max_tokens)
-    
-    results_generator = model.generate(ins, sampling_params,request_id) 
-    final_output = None
-    async for request_output in results_generator:        
-        final_output = request_output
-    assert final_output is not None    
-    
-    text_outputs = [output for output in final_output.outputs]
-    generated_text = text_outputs[0].text
-    
-    
-    input_tokens_count = len(final_output.prompt_token_ids)
-    generated_tokens_count = len(text_outputs[0].token_ids) 
-    
-    print(f"total_tokens_count:{input_tokens_count + generated_tokens_count} request_id:{final_output.request_id}  input_tokens_count:{input_tokens_count} generated_tokens_count:{generated_tokens_count}",flush=True)    
-    INFER_TOKEN_METRICS.inc(f"infer_{INFERENCE_NAME}_input_tokens_num",input_tokens_count,tags={"request_id":final_output.request_id})
-    INFER_TOKEN_METRICS.inc(f"infer_{INFERENCE_NAME}_output_tokens_num", generated_tokens_count,tags={"request_id":final_output.request_id})
-    INFER_TOKEN_METRICS.push()
-    return [(generated_text,"")]   
-
-def block_vllm_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
-        max_length:int=4096, 
-        top_p:float=0.95,
-        temperature:float=0.1,**kwargs):
-    from vllm import  SamplingParams        
-    n: int = 1
-    best_of: Optional[int] =  kwargs["best_of"] if "best_of" in kwargs else None
-    presence_penalty: float = float(kwargs.get("presence_penalty",0.0))
-    frequency_penalty: float = float(kwargs.get("frequency_penalty",0.0))
-    top_k: int = int(kwargs.get("top_k",-1))
-    use_beam_search: bool = kwargs.get("use_beam_search","false") == "true"
-    stop: Union[None, str, List[str]] = kwargs["stop"] if "stop" in kwargs else None
-    ignore_eos: bool = kwargs.get("ignore_eos","false") == "true"
-    max_tokens: int = max_length
-    logprobs: Optional[int] = kwargs["logprobs"] if "logprobs" in kwargs else None
-
-    model = self
-    sampling_params = SamplingParams(temperature=temperature, 
-                                     n = n,
-                                     best_of=best_of,
-                                     presence_penalty=presence_penalty,
-                                     frequency_penalty=frequency_penalty,
-                                     top_k=top_k,
-                                     use_beam_search=use_beam_search,
-                                     stop = stop,
-                                     ignore_eos=ignore_eos,
-                                     logprobs=logprobs,
-                                     top_p=top_p, 
-                                     max_tokens=max_tokens)
-    
-    outputs = model.generate([ins], sampling_params)    
-
-    output = outputs[0].outputs[0]
-    generated_text = output.text
-        
-    input_tokens_count = len(outputs[0].prompt_token_ids)
-    generated_tokens_count = len(output.token_ids) 
-    print(f"total_tokens_count:{input_tokens_count + generated_tokens_count} request_id:{outputs[0].request_id} output_num:{len(outputs)}/{len(outputs[0].outputs)}  input_tokens_count:{input_tokens_count} generated_tokens_count:{generated_tokens_count}",flush=True)
-
-    return [(generated_text,"")]   
-
-
-def vllm_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
-        max_length:int=4096, 
-        top_p:float=0.95,
-        temperature:float=0.1,**kwargs):
-    model = self        
-    return block_vllm_chat(model,model,tokenizer,ins,his,max_length,top_p,temperature,**kwargs)   
-
-def init_model(model_dir,infer_params:Dict[str,str]={},sys_conf:Dict[str,str]={}): 
-    infer_mode = sys_conf.get("infer_backend","transformers")
-    quatization = infer_params.get("quatization","false") == "true"
-    
-    if infer_mode == "transformers":
-        raise Exception('''
-transformers backend is not supported in pretrainedModelType: auto.
-Try to use ray/tgi or ray/deepspeed or ray/vllm.
-
-For example:
-
-!byzerllm setup "infer_backend=ray/vllm";
-''')
-    
-
-    if infer_mode == "tgi":
-        import byzerllm.utils.inference as TGI
-        return TGI.init_model(model_dir,infer_params)                
-    
-    if infer_mode in ["aviary/deepspeed","aviary/devicemap"]:   
-        num_workers = int(sys_conf.get("num_gpus",1))   
-        udfName = infer_params["udfName"]
-        mode = infer_mode.split("/")[1]
-        from byzerllm.utils.rayinfer import build_model_serving
-        model = build_model_serving(udfName,model_dir, mode=mode, num_workers=num_workers)        
-        model.stream_chat = types.MethodType(ray_chat, model) 
-        return (model,None) 
-
-    if infer_mode == "ray/vllm":        
-        num_gpus = int(sys_conf.get("num_gpus",1))
-        print(f"infer_mode:{infer_mode} tensor_parallel_size: {num_gpus}")
-        global INFERENCE_NAME
-        INFERENCE_NAME = infer_params.get("udfName","auto")
-        
-        # use_np_weights: bool = infer_params.get("backend.use_np_weights","false") == "true"
-        # use_dummy_weights: bool = infer_params.get("backend.use_dummy_weights","false") == "true"
-        dtype: str = infer_params.get("backend.dtype","auto")
-        seed: int = int(infer_params.get("backend.seed",0))
-        worker_use_ray: bool = infer_params.get("backend.worker_use_ray","false") == "false"
-        pipeline_parallel_size: int = int(infer_params.get("backend.pipeline_parallel_size",1))
-        tensor_parallel_size: int = num_gpus
-        block_size: int = int(infer_params.get("backend.block_size",16))
-        swap_space: int = int(infer_params.get("backend.swap_space",4))  # GiB
-        gpu_memory_utilization: float = float(infer_params.get("backend.gpu_memory_utilization",0.90))
-        max_num_batched_tokens: int = int(infer_params.get("backend.max_num_batched_tokens",2560))
-        max_num_seqs: int = int(infer_params.get("backend.max_num_seqs",256))
-        disable_log_stats: bool = infer_params.get("backend.disable_log_stats","false") == "true"
-
-        from vllm.engine.async_llm_engine import AsyncLLMEngine,AsyncEngineArgs     
-        engine_args = AsyncEngineArgs(
-            engine_use_ray=False,
-            disable_log_requests=False,
-            model=model_dir,
-            tokenizer=None,tokenizer_mode="auto",
-            trust_remote_code=True,    
-            worker_use_ray=worker_use_ray,                                        
-            dtype=dtype,
-            seed=seed,
-            pipeline_parallel_size=pipeline_parallel_size,
-            tensor_parallel_size=tensor_parallel_size,
-            block_size=block_size,
-            swap_space=swap_space,
-            gpu_memory_utilization=gpu_memory_utilization,
-            max_num_batched_tokens=max_num_batched_tokens,
-            max_num_seqs=max_num_seqs,
-            disable_log_stats=disable_log_stats
+import json
+import time
+from abc import ABC
+from typing import List, Tuple, Dict, Optional
+
+import boto3
+
+from byzerllm.log import init_logger
+from byzerllm.utils import random_uuid
+from byzerllm.utils.langutil import asyncfy_with_semaphore
+
+logger = init_logger(__name__)
+
+
+class SupportModelProviders:
+    Anthropic = "anthropic"
+    Meta = "meta"
+
+
+class CustomSaasAPI:
+    def __init__(self, infer_params: Dict[str, str]) -> None:
+        self.aws_access_key = infer_params["saas.aws_access_key"]
+        self.aws_secret_key = infer_params["saas.aws_secret_key"]
+        self.region_name = infer_params["saas.region_name"]
+        self.model = infer_params["saas.model"]
+        self.model_api_version = infer_params.get("saas.model_api_version", None)
+        self.model_provider = self.model.split(".")[0]
+
+        if self.model_provider == SupportModelProviders.Anthropic and self.model_api_version is None:
+            self.model_api_version = "bedrock-2023-05-31"
+
+        self.model_provider = AwsBedrockModelFactory.get_bedrock_model(
+            model_provider=self.model_provider,
+            model_api_version=self.model_api_version,
+            model_id=self.model,
+            aws_access_key=self.aws_access_key,
+            aws_secret_key=self.aws_secret_key,
+            region_name=self.region_name
         )
-        llm = AsyncLLMEngine.from_engine_args(engine_args)                       
-        # llm.stream_chat = types.MethodType(vllm_chat, llm) 
-        llm.async_stream_chat = types.MethodType(async_vllm_chat, llm) 
-        return (llm,None)  
-
-    if  infer_mode == "ray/deepspeed":
-        from .backend_ds import DeepSpeedInference,ParallelConfig        
-        num_gpus = int(sys_conf.get("num_gpus",1))
-        model = DeepSpeedInference(ParallelConfig(num_workers=num_gpus,model_dir=model_dir))    
-        return (model,None)                     
-
-    pretrained_model_dir = os.path.join(model_dir,"pretrained_model")
-    adaptor_model_dir = model_dir
-    is_adaptor_model = os.path.exists(pretrained_model_dir)
-    
-    if not is_adaptor_model:        
-        pretrained_model_dir = model_dir
-
-    tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir)    
 
-    if quatization:
-        nf4_config = BitsAndBytesConfig(
-            load_in_4bit=True,
-            bnb_4bit_quant_type="nf4",
-            bnb_4bit_use_double_quant=False,
-            bnb_4bit_compute_dtype=torch.bfloat16,
+    # saas/proprietary
+    def get_meta(self):
+        return [{
+            "model_deploy_type": "saas",
+            "backend": "saas",
+        }]
+    
+    async def async_get_meta(self):
+        return await asyncfy_with_semaphore(self.get_meta)()
+    
+    async def async_stream_chat(
+            self,
+            tokenizer,
+            ins: str,
+            his: List[Tuple[str, str]] = [],
+            max_length: int = 4096,
+            top_p: float = 0.7,
+            temperature: float = 0.9,
+            **kwargs
+    ):
+        return await asyncfy_with_semaphore(self.stream_chat)(tokenizer, ins, his, max_length, top_p, temperature, **kwargs)
+
+    def stream_chat(
+            self,
+            tokenizer,
+            ins: str,
+            his: List[Tuple[str, str]] = [],
+            max_length: int = 4096,
+            top_p: float = 0.7,
+            temperature: float = 0.9,
+            **kwargs
+    ):
+        try:
+            return self.model_provider.generate(
+                ins=ins,
+                his=his,
+                max_length=max_length,
+                top_p=top_p,
+                temperature=temperature,
+                **kwargs
+            )
+        except Exception as e:
+            logger.error(f"request aws bedrock failed: {e}")
+        return None
+
+
+class AWSBedrockModel(ABC):
+    bedrock_client = None
+    model_id = None
+    model_api_version = None
+
+    def __init__(
+            self,
+            model_id: str,
+            region_name: str = None,
+            aws_access_key: str = None,
+            aws_secret_key: str = None,
+            model_api_version: Optional[str] = None,
+
+    ):
+        self.model_id = model_id
+        self.model_api_version = model_api_version
+        self.bedrock = boto3.client(
+            service_name='bedrock-runtime',
+            aws_access_key_id=aws_access_key,
+            aws_secret_access_key=aws_secret_key,
+            region_name=region_name,
         )
-        model = AutoModelForCausalLM.from_pretrained(
-            pretrained_model_dir,
-            trust_remote_code=True,            
-            device_map="auto",
-            quantization_config=nf4_config,
-        )
-
-    else:
-        model = AutoModelForCausalLM.from_pretrained(pretrained_model_dir,trust_remote_code=True,
-                                                device_map='auto',                                                
-                                                torch_dtype=torch.bfloat16                                                
-                                                )
-    if is_adaptor_model:
-        from peft import PeftModel
-        model = PeftModel.from_pretrained(model, adaptor_model_dir)
-
-    model.eval()  
-    if quatization:
-        model = torch.compile(model)   
-
-    model.stream_chat = types.MethodType(stream_chat, model)     
-    return (model,tokenizer)
-
-
-def sft_train(data_refs:List[DataServer],
-              train_params:Dict[str,str],
-              conf: Dict[str, str])->Generator[BlockRow,Any,Any]:
-    from ..utils.sft import sft_train as common_sft_train
-    return common_sft_train(data_refs,train_params,conf) 
 
+    def generate(
+            self,
+            ins: str,
+            his: List[Tuple[str, str]] = [],
+            max_length: int = 4096,
+            top_p: float = 0.7,
+            temperature: float = 0.9,
+            **kwargs):
+        pass
+
+
+class AnthropicModel(AWSBedrockModel):
+
+    def generate(
+            self,
+            ins: str,
+            his: List[Tuple[str, str]] = [],
+            max_length: int = 4096,
+            top_p: float = 0.7,
+            temperature: float = 0.9,
+            **kwargs
+    ):
+        body = self._generate_anthropic_request_body(ins, his)
+
+        logger.info(f"【Byzer --> AWS-Bedrock({self.model_id})】:\n{body}")
+
+        answer = None
+        input_tokens = 0
+        output_tokens = 0
+        time_taken = 0
+        start_time = time.monotonic()
+
+        try:
+            api_res = self.bedrock.invoke_model(
+                body=json.dumps(body),
+                modelId=self.model_id,
+                accept='application/json',
+                contentType='application/json'
+            )
+            time_taken = time.monotonic() - start_time
+            response_body = json.loads(api_res.get('body').read())
+            logger.info(
+                f"【AWS-Bedrock({self.model_id}) --> Byzer】:\n{response_body}"
+            )
+            answer = response_body['content'][0]['text']
+            input_tokens = response_body['usage']['input_tokens']
+            output_tokens = response_body['usage']['output_tokens']
+        except Exception as e:
+            logger.error(f"request aws bedrock failed: {e}")
+            answer = f"Exception occurred during the request, please try again: {e}" if not answer else answer
+
+        return [(
+            answer,
+            {
+                "metadata": {
+                    "request_id": "",
+                    "input_tokens_count": input_tokens,
+                    "generated_tokens_count": output_tokens,
+                    "time_cost": time_taken,
+                    "first_token_time": -1.0,
+                    "speed": float(output_tokens) / time_taken * 1000 if time_taken > 0 else 0,
+                }
+            }
+        )]
+
+    def _generate_anthropic_request_body(
+            self,
+            ins: str,
+            his: List[Tuple[str, str]] = [],
+            max_length: int = 4096,
+            temperature: float = 0.9,
+    ):
+        messages = []
+        for item in his:
+            role, content = item["role"], item["content"]
+            if role == "system":
+                messages.append({"role": "user", "content": [{"type": "text", "text": content}]})
+                messages.append({"role": "assistant", "content": [{"type": "text", "text": "OK"}]})
+                continue
+            messages.append({"role": role, "content": [{"type": "text", "text": content}]})
+
+        if ins and len(messages) == 0:
+            messages.append({"role": "user", "content": [{"type": "text", "text": ins}]})
+
+        if ins and len(messages) > 0:
+            last_message_role = messages[-1]["role"]
+            if last_message_role == "user":
+                messages.append({"role": "assistant", "content": [{"type": "text", "text": "OK"}]})
+            messages.append({"role": "user", "content": [{"type": "text", "text": ins}]})
+
+        anthropic_request_body = {
+            "anthropic_version": self.model_api_version,
+            "temperature": temperature,
+            "max_tokens": max_length,
+            "messages": messages
+        }
+
+        return anthropic_request_body
+
+
+class MetaModel(AWSBedrockModel):
+
+    def generate(
+            self,
+            ins: str,
+            his: List[Tuple[str, str]] = [],
+            max_length: int = 4096,
+            top_p: float = 0.7,
+            temperature: float = 0.9,
+            **kwargs
+    ):
+        request_id = random_uuid() if "request_id" not in kwargs else kwargs["request_id"]
+
+        fin_ins = self._generate_meta_instruction_from_history(ins, his)
+
+        max_length = min(2048, max_length)
+
+        meta_request_body = json.dumps({
+            "prompt": fin_ins,
+            "max_gen_len": max_length,
+            "temperature": temperature,
+            "top_p": top_p,
+        })
+
+        logger.info(f"Receiving request model: {self.model_id} messages: {meta_request_body}")
+
+        answer = None
+        input_tokens = 0
+        output_tokens = 0
+        time_taken = 0
+        start_time = time.monotonic()
+
+        try:
+            api_res = self.bedrock.invoke_model(
+                body=meta_request_body,
+                modelId=self.model_id,
+                accept='application/json',
+                contentType='application/json'
+            )
+            time_taken = time.monotonic() - start_time
+            response_body = json.loads(api_res.get('body').read())
+            logger.info(
+                f"Completed request {request_id}: "
+                f"model: {self.model_id} "
+                f"cost: {time_taken} "
+                f"result: {response_body}"
+            )
+            answer = response_body['generation']
+            input_tokens = response_body['prompt_token_count']
+            output_tokens = response_body['generation_token_count']
+        except Exception as e:
+            logger.error(f"request aws bedrock failed: {e}")
+            answer = f"Exception occurred during the request, please try again: {e}" if not answer else answer
+
+        return [(
+            answer,
+            {
+                "metadata": {
+                    "request_id": "",
+                    "input_tokens_count": input_tokens,
+                    "generated_tokens_count": output_tokens,
+                    "time_cost": time_taken,
+                    "first_token_time": -1.0,
+                    "speed": float(output_tokens) / time_taken * 1000 if time_taken > 0 else 0,
+                }
+            }
+        )]
+
+    def _generate_meta_instruction_from_history(
+            self,
+            ins: str,
+            his: List[Dict[str, str]],
+            role_mapping: Dict[str, str] = {
+                "user": "Human",
+                "assistant": "Assistant",
+            }
+    ):
+        # if len(his) == 1 and ins == "":
+        #     return his[0]['content'].strip() + "\n"
+
+        new_his = []
+        for item in his:
+            if item["role"] == "system":
+                new_his.append(item["content"])
+                continue
+            if item["role"] == "user":
+                new_his.append(
+                    f"[INST]{role_mapping[item['role']]}: {item['content']}")
+                continue
+            if item["role"] == "assistant":
+                new_his.append(
+                    f"{role_mapping[item['role']]}: {item['content']}[/INST]")
+                continue
+
+        # here we should make sure the user build the conversation string manually also
+        # works. This means if the user do not provide  the history, then
+        # we should treat ins as conversation string which the user build manually
+        if len(new_his) > 0 and ins != "":
+            new_his.append(f"[INST]{role_mapping['user']}: {ins}")
+            new_his.append(f"{role_mapping['assistant']}:[/INST]")
+
+        if len(new_his) > 0 and ins == "":
+            new_his.append(f"{role_mapping['assistant']}[/INST]:")
+
+        if len(new_his) == 0:
+            new_his.append(ins)
+
+        fin_ins = "\n".join(new_his)
+        return fin_ins
+
+
+class AwsBedrockModelFactory:
+    @staticmethod
+    def get_bedrock_model(
+            model_provider: str,
+            model_id: str,
+            region_name: str = None,
+            aws_access_key: str = None,
+            aws_secret_key: str = None,
+            model_api_version: Optional[str] = None,
+    ) -> AWSBedrockModel:
+        model_provider = model_provider.lower()
+        logger.info(f"Using model_provider: {model_provider}")
+        if SupportModelProviders.Anthropic == model_provider:
+            return AnthropicModel(
+                model_id=model_id,
+                model_api_version=model_api_version,
+                region_name=region_name,
+                aws_access_key=aws_access_key,
+                aws_secret_key=aws_secret_key
+            )
+        elif SupportModelProviders.Meta == model_provider:
+            return MetaModel(
+                model_id=model_id,
+                model_api_version=model_api_version,
+                region_name=region_name,
+                aws_access_key=aws_access_key,
+                aws_secret_key=aws_secret_key
+            )
+        else:
+            raise ValueError(f"Unsupported model_provider: {model_provider}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `byzerllm-0.1.9/src/byzerllm/auto/backend_ds.py` & `byzerllm-0.1.90/src/byzerllm/auto/backend_ds.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/baichuan/__init__.py` & `byzerllm-0.1.90/src/byzerllm/baichuan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from transformers import AutoTokenizer, AutoModelForCausalLM,GenerationConfig,BitsAndBytesConfig
 from pyjava.api.mlsql import DataServer
 import torch
 import os
 from typing import Any,Any,Dict, List,Tuple,Generator
 from .. import BlockRow
 
+def get_meta(self): 
+    config = self.config   
+    return [{
+        "model_deploy_type": "proprietary",
+        "backend":"transformers",
+        "max_model_len":getattr(config, "model_max_length", -1),
+        "architectures":getattr(config, "architectures", [])
+    }]
+
 def stream_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
         max_length:int=4096, 
         top_p:float=0.95,
         temperature:float=0.1,**kwargs):
         
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     tokens = tokenizer(ins, return_token_type_ids=False,return_tensors="pt").to(device)
@@ -64,25 +73,28 @@
             device_map="auto",
             quantization_config=quantization_config,
         )
     else:
         model = AutoModelForCausalLM.from_pretrained(pretrained_model_dir,trust_remote_code=True,
                                                 device_map='auto',                                                
                                                 torch_dtype=torch.bfloat16                                                
-                                                )    
+                                                )         
+           
     
     model.generation_config = GenerationConfig.from_pretrained(pretrained_model_dir)
     
     if is_adaptor_model:
         from peft import PeftModel
         model = PeftModel.from_pretrained(model, adaptor_model_dir)
 
     model.eval() 
     import types
+    
     model.stream_chat = types.MethodType(stream_chat, model)     
+    model.get_meta = types.MethodType(get_meta, model)
     return (model,tokenizer)
 
 def sft_train(data_refs:List[DataServer],
               train_params:Dict[str,str],
               conf: Dict[str, str])->Generator[BlockRow,Any,Any]:
     from ..utils.sft import sft_train as common_sft_train
     return common_sft_train(data_refs,train_params,conf)
```

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/api.py` & `byzerllm-0.1.90/src/byzerllm/bark/api.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/announcer.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/announcer.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/readme.md` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/readme.md`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz` & `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/bark_voice.py` & `byzerllm-0.1.90/src/byzerllm/bark/bark_voice.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/generation.py` & `byzerllm-0.1.90/src/byzerllm/bark/generation.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/model.py` & `byzerllm-0.1.90/src/byzerllm/bark/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bark/model_fine.py` & `byzerllm-0.1.90/src/byzerllm/bark/model_fine.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/bge/__init__.py` & `byzerllm-0.1.90/src/byzerllm/bge/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm2/__init__.py` & `byzerllm-0.1.90/src/byzerllm/chatglm2/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 from typing import Any,Any,Dict, List,Tuple,Generator
 
 
 from pyjava.api.mlsql import DataServer
 from .. import BlockRow
 from .. import parse_params
 
-
+  
+def get_meta(self): 
+    config = self.config   
+    return [{
+        "model_deploy_type": "proprietary",
+        "backend":"transformers",
+        "max_model_len":getattr(config, "model_max_length", -1),
+        "architectures":getattr(config, "architectures", [])
+    }]
 
 def stream_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
         max_length:int=4096, 
         top_p:float=0.95,
         temperature:float=0.1,**kwargs):
         
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
@@ -43,16 +51,17 @@
     tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir,trust_remote_code=True)    
     model = AutoModel.from_pretrained(pretrained_model_dir,trust_remote_code=True ).half().cuda()
     if is_adaptor_model:
         from peft import PeftModel
         model = PeftModel.from_pretrained(model, adaptor_model_dir)
         
     model.eval()       
-    # import types
-    # model.stream_chat = types.MethodType(stream_chat, model)     
+    import types
+    # model.stream_chat = types.MethodType(stream_chat, model)  
+    model.get_meta = types.MethodType(get_meta, model)     
     return (model,tokenizer)
 
 
 def sft_train(data_refs:List[DataServer],
               train_params:Dict[str,str],
               conf: Dict[str, str])->Generator[BlockRow,Any,Any]:
     from ..utils.sft import sft_train as common_sft_train
```

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm6b/arguments.py` & `byzerllm-0.1.90/src/byzerllm/chatglm6b/arguments.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm6b/finetune.py` & `byzerllm-0.1.90/src/byzerllm/chatglm6b/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm6b/trainer_seq2seq.py` & `byzerllm-0.1.90/src/byzerllm/chatglm6b/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/finetune.py` & `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/infer.py` & `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/infer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/common.py` & `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/common.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/config.py` & `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/config.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/other.py` & `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/other.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py` & `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/dolly/consts.py` & `byzerllm-0.1.90/src/byzerllm/dolly/consts.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/dolly/dolly_inference.py` & `byzerllm-0.1.90/src/byzerllm/dolly/dolly_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/dolly/generate.py` & `byzerllm-0.1.90/src/byzerllm/dolly/generate.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/dolly/trainer.py` & `byzerllm-0.1.90/src/byzerllm/dolly/trainer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/falcon/__init__.py` & `byzerllm-0.1.90/src/byzerllm/falcon/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 from typing import Any,Any,Dict, List,Tuple,Generator
 import types
 from byzerllm.utils import generate_instruction_from_history,compute_max_new_tokens
 
 from pyjava.api.mlsql import DataServer
 from .. import BlockRow
 
+def get_meta(self): 
+    config = self.config   
+    return [{
+        "model_deploy_type": "proprietary",
+        "backend":"transformers",
+        "max_model_len":getattr(config, "model_max_length", -1),
+        "architectures":getattr(config, "architectures", [])
+    }]
+
 def stream_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
         max_length:int=1024, 
         top_p:float=0.95,
         temperature:float=0.1,**kwargs):
         
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")    
     role_mapping = {        
@@ -89,15 +98,16 @@
 
     model.eval()  
     if quatization:
         model = torch.compile(model)
     
     # falcon is not support yet in optimum
     # model = model.to_bettertransformer()    
-    model.stream_chat = types.MethodType(stream_chat, model)     
+    model.stream_chat = types.MethodType(stream_chat, model) 
+    model.get_meta = types.MethodType(get_meta, model)        
     return (model,tokenizer)
 
 
 def sft_train(data_refs:List[DataServer],
               train_params:Dict[str,str],
               conf: Dict[str, str])->Generator[BlockRow,Any,Any]:
     from ..utils.sft import sft_train as common_sft_train
```

### Comparing `byzerllm-0.1.9/src/byzerllm/llama/__init__.py` & `byzerllm-0.1.90/src/byzerllm/llama/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 from transformers import AutoTokenizer, AutoModelForCausalLM,BitsAndBytesConfig,StoppingCriteriaList
 import transformers
 import torch
 from typing import Dict,List,Any,Generator
 from pyjava.api.mlsql import DataServer
 from byzerllm import BlockRow
 from byzerllm.utils import (generate_instruction_from_history,
-compute_max_new_tokens,tokenize_stopping_sequences,StopSequencesCriteria)
+compute_max_new_tokens,tokenize_stopping_sequences)
+from byzerllm.utils.types import StopSequencesCriteria
 import os
 import time
 
+def get_meta(self): 
+    config = self.config   
+    return [{
+        "model_deploy_type": "proprietary",
+        "backend":"transformers",
+        "max_model_len":getattr(config, "model_max_length", -1),
+        "architectures":getattr(config, "architectures", [])
+    }]
+
 def stream_chat(self,tokenizer,ins:str, his:List[Dict[str,str]]=[],  
         max_length:int=4090, 
         top_p:float=0.95,
         temperature:float=0.1,**kwargs):
         
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu") 
     timeout_s = float(kwargs.get("timeout_s",60*5)) 
@@ -127,15 +137,16 @@
         from peft import PeftModel
         model = PeftModel.from_pretrained(model, adaptor_model_dir)
 
     model.eval()  
     if quatization:
         model = torch.compile(model)      
     import types
-    model.stream_chat = types.MethodType(stream_chat, model)     
+    model.stream_chat = types.MethodType(stream_chat, model) 
+    model.get_meta = types.MethodType(get_meta, model)    
     return (model,tokenizer)
 
 def sft_train(data_refs:List[DataServer],
               train_params:Dict[str,str],
               conf: Dict[str, str])->Generator[BlockRow,Any,Any]:
     from ..utils.sft import sft_train as common_sft_train
     return common_sft_train(data_refs,train_params,conf)
```

### Comparing `byzerllm-0.1.9/src/byzerllm/llama2/__init__.py` & `byzerllm-0.1.90/src/byzerllm/qwen/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 from transformers import AutoTokenizer, AutoModelForCausalLM,BitsAndBytesConfig,StoppingCriteriaList
 import transformers
 import torch
 from typing import Dict,List,Tuple
 from byzerllm.utils import (generate_instruction_from_history,
-compute_max_new_tokens,tokenize_stopping_sequences,StopSequencesCriteria)
+compute_max_new_tokens,tokenize_stopping_sequences)
+from byzerllm.utils.types import StopSequencesCriteria
 
 from typing import Dict, Any,List,Generator
 from pyjava.storage import streaming_tar as STar
 from pyjava import RayContext
 from pyjava.api.mlsql import DataServer
 from byzerllm import BlockRow
 import os
 import time
 
+def get_meta(self): 
+    config = self.config   
+    return [{
+        "model_deploy_type": "proprietary",
+        "backend":"transformers",
+        "max_model_len":getattr(config, "model_max_length", -1),
+        "architectures":getattr(config, "architectures", [])
+    }]
+
 def stream_chat(self,tokenizer,ins:str, his:List[Dict[str,str]]=[],  
         max_length:int=4090, 
         top_p:float=0.95,
         temperature:float=0.1,**kwargs):
         
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu") 
     timeout_s = float(kwargs.get("timeout_s",60*5)) 
@@ -63,41 +73,40 @@
     new_tokens = response[0][tokens["input_ids"].shape[1]:]
     print(f"generate took {time_taken} s to complete. tokens/s:{len(new_tokens)/time_taken}",flush=True)
     answer = tokenizer.decode(new_tokens, skip_special_tokens=True)
     return [(answer,"")]
 
 
 def init_model(model_dir,infer_params:Dict[str,str]={},sys_conf:Dict[str,str]={}):
-    longContextMode = infer_params.get("longContextMode","true") == "true"    
-    if longContextMode:
-        old_init = transformers.models.llama.modeling_llama.LlamaRotaryEmbedding.__init__
-        def ntk_scaled_init(self, dim, max_position_embeddings=4096, base=10000, device=None):
-
-            #The method is just these three lines
-            max_position_embeddings = 16384
-            a = 8 #Alpha value
-            base = base * a ** (dim / (dim-2)) #Base change formula
+    # longContextMode = infer_params.get("longContextMode","true") == "true"    
+    # if longContextMode:
+    #     old_init = transformers.models.llama.modeling_llama.LlamaRotaryEmbedding.__init__
+    #     def ntk_scaled_init(self, dim, max_position_embeddings=4096, base=10000, device=None):
+
+    #         #The method is just these three lines
+    #         max_position_embeddings = 16384
+    #         a = 8 #Alpha value
+    #         base = base * a ** (dim / (dim-2)) #Base change formula
 
-            old_init(self, dim, max_position_embeddings, base, device)    
+    #         old_init(self, dim, max_position_embeddings, base, device)    
         
-        transformers.models.llama.modeling_llama.LlamaRotaryEmbedding.__init__ = ntk_scaled_init
+    #     transformers.models.llama.modeling_llama.LlamaRotaryEmbedding.__init__ = ntk_scaled_init
 
     pretrained_model_dir = os.path.join(model_dir,"pretrained_model")
     adaptor_model_dir = model_dir
     is_adaptor_model = os.path.exists(pretrained_model_dir)
 
     if not is_adaptor_model:        
         pretrained_model_dir = model_dir
 
     tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir,trust_remote_code=True)
     tokenizer.padding_side="right"
     tokenizer.pad_token_id=0
     tokenizer.bos_token_id = 1
 
-    print(f"longContextMode:{longContextMode}", flush=True)
 
     quatization = infer_params.get("quatization", "false")
 
     if quatization in ["4", "8", "true"]:
         print(f"enable [{quatization}] quatization.", flush=True)
         load_in_8bit = quatization == "8"
         # default using int4
@@ -121,27 +130,27 @@
             trust_remote_code=True,
             device_map="auto",
             quantization_config=quantization_config,
         )
     else:
         model = AutoModelForCausalLM.from_pretrained(pretrained_model_dir,trust_remote_code=True,
                                                 device_map='auto',                                                
-                                                torch_dtype=torch.bfloat16                                                
                                                 )
     if is_adaptor_model:
         from peft import PeftModel
         model = PeftModel.from_pretrained(model, adaptor_model_dir)
 
     model.eval()  
     if quatization:
         model = torch.compile(model)     
 
-    model = model.to_bettertransformer()     
+    # model = model.to_bettertransformer()     
     import types
-    model.stream_chat = types.MethodType(stream_chat, model)     
+    model.stream_chat = types.MethodType(stream_chat, model) 
+    model.get_meta = types.MethodType(get_meta, model)        
     return (model,tokenizer)
 
 
 
 def sft_train(data_refs:List[DataServer],
               train_params:Dict[str,str],
               conf: Dict[str, str])->Generator[BlockRow,Any,Any]:
@@ -150,13 +159,7 @@
 
 
 def sfft_train(data_refs:List[DataServer],
               train_params:Dict[str,str],
               conf: Dict[str, str])->Generator[BlockRow,Any,Any]:
     from ..utils.fulltune.pretrain import sfft_train as common_sfft_train
     return common_sfft_train(data_refs,train_params,conf) 
-
-
-
-
-
-
```

### Comparing `byzerllm-0.1.9/src/byzerllm/moss/finetune_moss.py` & `byzerllm-0.1.90/src/byzerllm/moss/finetune_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/moss/models/configuration_moss.py` & `byzerllm-0.1.90/src/byzerllm/moss/models/configuration_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/moss/models/custom_autotune.py` & `byzerllm-0.1.90/src/byzerllm/moss/models/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/moss/models/modeling_moss.py` & `byzerllm-0.1.90/src/byzerllm/moss/models/modeling_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/moss/models/quantization.py` & `byzerllm-0.1.90/src/byzerllm/moss/models/quantization.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/moss/models/tokenization_moss.py` & `byzerllm-0.1.90/src/byzerllm/moss/models/tokenization_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/moss/moss_inference.py` & `byzerllm-0.1.90/src/byzerllm/moss/moss_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/processor/__init__.py` & `byzerllm-0.1.90/src/byzerllm/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/qwen_vl_chat/__init__.py` & `byzerllm-0.1.90/src/byzerllm/qwen_vl_chat/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from transformers import AutoModelForCausalLM, AutoTokenizer,GenerationConfig
-import transformers
-import torch
 import json
 import os
 import io
 from typing import Any,Any,Dict, List,Tuple,Generator
 import base64
 import uuid
 import tempfile
 
-from pyjava.api.mlsql import DataServer
-from .. import BlockRow
-from .. import parse_params
+def get_meta(self): 
+    config = self.config   
+    return [{
+        "model_deploy_type": "proprietary",
+        "backend":"transformers",
+        "max_model_len":getattr(config, "model_max_length", -1),
+        "architectures":getattr(config, "architectures", []),
+        "message_format":True,
+    }]
 
-
-
-def stream_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
+def stream_chat(self,tokenizer,ins:str, his:List[Dict[str,str]]=[],  
         max_length:int=4096, 
         top_p:float=0.95,
         temperature:float=0.1,**kwargs):
     image = kwargs["image"]
     image_b = base64.b64decode(image)
 
     temp_image_dir = os.path.join(tempfile.gettempdir(),"byzerllm","visualglm","images")
@@ -34,44 +36,42 @@
     if "input_image_path" in kwargs:
         image_file = kwargs["input_image_path"]
 
     with open(image_file,"wb") as f:
         f.write(image_b)
 
     # history format [('Picture 1:<img>https://qianwen-res.oss-cn-beijing.aliyuncs.com/Qwen-VL/assets/demo.jpeg</img>\n这是什么?',
-    # '图中是一名女子和她的狗在沙滩上玩耍，狗的品种应该是一只拉布拉多犬。')] 
-    base64_new_image = None
+    # '图中是一名女子和她的狗在沙滩上玩耍，狗的品种应该是一只拉布拉多犬。')]     
     input_history = None
     if "history" in kwargs:
-        input_history = json.loads(kwargs["history"])
-
+        input_history = []
+        temp_input_history = json.loads(kwargs["history"]) 
+        temp_input_history_length = len(temp_input_history)
+        for i in range(0,temp_input_history_length,2):
+            input_history.append((temp_input_history[i]["content"],temp_input_history[i+1]["content"]))
+            
     if not input_history:           
         query = tokenizer.from_list_format([
         {'image': image_file}, 
         {'text': ins},])
         response, history = self.chat(tokenizer, query=query, history=None)                            
     else:        
-        response, history = self.chat(tokenizer, ins, history=input_history)         
-        # try:
-        #     import matplotlib.pyplot as plt
-        #     plt.clf() 
-        #     plt.close()
-        # except:
-        #     pass
-
-        new_image = tokenizer.draw_bbox_on_latest_picture(response, history)        
-        if new_image:
-            byte_io = io.BytesIO()
-            new_image.save(byte_io)
-            base64_new_image = base64.b64encode(byte_io.getvalue()).decode('utf-8')
-        else:
-            print("no new image",flush=True)    
+        response, history = self.chat(tokenizer, ins, history=input_history)                            
     
-    output = json.dumps({"response":response,"history":history,"image":base64_new_image,"input_image":image,"input_image_path":image_file})
-    return [(output,"")]
+    temp_history = []
+    for item in history:
+        temp_history.append(
+            {"role":"user","content":item[0]},
+        )
+        temp_history.append(
+            {"role":"assistant","content":item[1]},
+        )
+        
+    output = json.dumps({"response":response,"history":temp_history},ensure_ascii=False)
+    return [(output,{"metadata":{}})] 
 
 
 def init_model(model_dir,infer_params:Dict[str,str]={},sys_conf:Dict[str,str]={}): 
     pretrained_model_dir = os.path.join(model_dir,"pretrained_model")
     adaptor_model_dir = model_dir
     is_adaptor_model = os.path.exists(pretrained_model_dir)
     
@@ -88,14 +88,15 @@
         from peft import PeftModel
         model = PeftModel.from_pretrained(model, adaptor_model_dir)
         
     model.eval()
     model.generation_config = GenerationConfig.from_pretrained(pretrained_model_dir, trust_remote_code=True)       
     import types
     model.stream_chat = types.MethodType(stream_chat, model)     
+    model.get_meta = types.MethodType(get_meta, model)
     return (model,tokenizer)
```

### Comparing `byzerllm-0.1.9/src/byzerllm/saas/chatglm/__init__.py` & `byzerllm-0.1.90/src/byzerllm/saas/chatglm/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 from wudao.api_request import executeSSE, getToken, queryTaskResult
 from random import randint
 import time
 import uuid
 
-from typing import Union, List, Tuple, Optional, Dict
+from typing import Union, List, Tuple, Optional, Dict,Any
 
 def randomTaskCode():
     return "%019d" % randint(0, 10**19)
 
 class ChatGLMAPI:
     def __init__(self,api_key:str, public_key:str,params:Dict[str,str]={}) -> None:
         self.api_key = api_key if api_key else params.get("saas.api_key","")
         self.public_key = public_key if public_key else params.get("saas.public_key","")
         self.ability_type = "chatGLM"
         self.engine_type = "chatGLM"
         self.temp_token = None
 
+     # saas/proprietary
+    def get_meta(self):
+        return [{
+            "model_deploy_type": "saas",
+            "backend":"saas"
+        }]    
+
     def get_token_or_refresh(self):
         token_result = getToken(self.api_key, self.public_key)
         if token_result and token_result["code"] == 200:
             token = token_result["data"]
             self.temp_token = token
         else:
             raise Exception("Fail to get token from ChatGLMAPI. Check api_key/public_key")    
         return self.temp_token    
     
-    def stream_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
+    def stream_chat(self,tokenizer,ins:str, his:List[Dict[str,Any]]=[],  
         max_length:int=4096, 
         top_p:float=0.7,
         temperature:float=0.9,**kwargs): 
 
         q = []
         for item in his:    
-            q.append(item[0])
-            q.append(item[1])
+            q.append(item["user"])
+            q.append(item["assistant"])
 
         data = {
                     "top_p": top_p,
                     "temperature": temperature,                    
                     "risk": 0.15,                    
                     "requestTaskNo": randomTaskCode(),                                        
                     "prompt": ins,
```

### Comparing `byzerllm-0.1.9/src/byzerllm/saas/sparkdesk/__init__.py` & `byzerllm-0.1.90/src/byzerllm/saas/sparkdesk/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 import json
 from urllib.parse import urlparse
 import ssl
 from datetime import datetime
 from time import mktime
 from urllib.parse import urlencode
 from wsgiref.handlers import format_date_time
-from typing import List, Tuple,Dict
-import time
+from typing import List, Tuple,Dict,Any
+from byzerllm.utils.langutil import asyncfy_with_semaphore
 import queue
 
 import websocket
 
 reponse_queue = queue.Queue()
 
 class SparkDeskAPIParams(object):
     # 初始化
-    def __init__(self, APPID, APIKey, APISecret, gpt_url):
+    def __init__(self, APPID, APIKey, APISecret, gpt_url, DOMAIN):
         self.APPID = APPID
         self.APIKey = APIKey
         self.APISecret = APISecret
         self.host = urlparse(gpt_url).netloc
         self.path = urlparse(gpt_url).path
         self.gpt_url = gpt_url
+        self.DOMAIN = DOMAIN
 
-    # 生成url
+        # 生成url
     def create_url(self):
         # 生成RFC1123格式的时间戳
         now = datetime.now()
         date = format_date_time(mktime(now.timetuple()))
 
         # 拼接字符串
         signature_origin = "host: " + self.host + "\n"
@@ -56,109 +57,137 @@
             "host": self.host
         }
         # 拼接鉴权参数，生成url
         url = self.gpt_url + '?' + urlencode(v)
         # 此处打印出建立连接时候的url,参考本demo的时候可取消上方打印的注释，比对相同参数时生成的url与自己代码生成的url是否一致
         return url
 
-class SparkDeskAPI:
 
-    def __init__(self,appid, api_key, api_secret,params:Dict[str,str]={}) -> None:
-        appid = appid if appid else params.get("saas.appid","")
-        api_key = api_key if api_key else params.get("saas.api_key","")
-        api_secret = api_secret if api_secret else params.get("saas.api_secret","")
-        gpt_url = params.get("gpt_url","ws://spark-api.xf-yun.com/v1.1/chat")
-        self.config = SparkDeskAPIParams(appid, api_key, api_secret, gpt_url)
-    
+class CustomSaasAPI:
+
+    def __init__(self, infer_params: Dict[str, str]) -> None:
+        required_params = [ "saas.appid", "saas.api_key", "saas.api_secret"]
+        for param in required_params:
+            if list(infer_params.keys()).count(param) < 1:
+                raise ValueError("The parameter %s is a required field, please configure it"% param)
+        for value in self.get_value(infer_params,required_params):
+            if value is None or value == "":
+                raise ValueError("The mandatory model parameters cannot be empty.")
+        self.appid: str = infer_params["saas.appid"]
+        self.api_key: str = infer_params["saas.api_key"]
+        self.api_secret: str = infer_params["saas.api_secret"]
+        self.gpt_url: str = infer_params.get("saas.gpt_url","wss://spark-api.xf-yun.com/v3.1/chat")
+        self.domain: str = infer_params.get("saas.domain","generalv3")
+        self.config = SparkDeskAPIParams(self.appid, self.api_key, self.api_secret, self.gpt_url, self.domain)
+        self.timeout = int(infer_params.get("saas.timeout",30))
+        self.debug = infer_params.get("saas.debug",False)
+
     @staticmethod
     def on_error(ws, error):
         pass
 
 
     @staticmethod
-    def on_close(ws,a,b):        
+    def on_close(ws,a,b):
         pass
 
 
     @staticmethod
     def on_open(ws):
-        thread.start_new_thread(SparkDeskAPI.run, (ws,))
+        thread.start_new_thread(CustomSaasAPI.run, (ws,))
 
     @staticmethod
     def run(ws, *args):
         # 8192
         data = {
             "header": {
                 "app_id": ws.appid,
                 "uid": "1234"
             },
             "parameter": {
                 "chat": {
-                    "domain": "general",
+                    "domain": ws.domain,
                     "random_threshold": ws.temperature,
                     "max_tokens": ws.max_length,
                     "auditing": "default"
                 }
             },
             "payload": {
                 "message": {
                     "text": ws.question
                 }
             }
         }
-        data = json.dumps(data)
+        data = json.dumps(data)        
         ws.send(data)
 
-   
+
     @staticmethod
     def on_message(ws, message):
-        data = json.loads(message)
+        data = json.loads(message)        
         code = data['header']['code']
-        if code != 0:            
+        if code != 0:
             reponse_queue.put(f'请求错误: {code}, {data}')
             reponse_queue.put(None)
             ws.close()
         else:
             choices = data["payload"]["choices"]
             status = choices["status"]
-            content = choices["text"][0]["content"]            
+            content = choices["text"][0]["content"]
             reponse_queue.put(content)
             if status == 2:
                 reponse_queue.put(None)
                 ws.close()
-    
 
-    def stream_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
-        max_length:int=4096, 
-        top_p:float=0.7,
-        temperature:float=0.9): 
-
-        q = [] 
-        for item in his:
-           q.append({"role": "user", "content": item[0]})
-           q.append({"role": "assistant", "content": item[1]})
 
+    # saas/proprietary
+    def get_meta(self):
+        return [{
+            "model_deploy_type": "saas",
+            "backend":"saas"
+        }]
+    
+    async def async_get_meta(self):
+        return await asyncfy_with_semaphore(self.get_meta)()
+
+    def get_value(self,infer_params: Dict[str, str],keys_to_get):
+        values = []
+        for key in keys_to_get:
+            if key in infer_params.keys():
+                values.append(infer_params[key])
+        return values
+    
+    async def async_stream_chat(self,tokenizer,ins:str, his:List[Dict[str,Any]]=[],
+                    max_length:int=4096,
+                    top_p:float=0.7,
+                    temperature:float=0.9):
+        return await asyncfy_with_semaphore(self.stream_chat)(tokenizer,ins,his,max_length,top_p,temperature)
+
+    def stream_chat(self,tokenizer,ins:str, his:List[Dict[str,Any]]=[],
+                    max_length:int=4096,
+                    top_p:float=0.7,
+                    temperature:float=0.9):
 
-        q.append({"role": "user", "content": ins})        
-        websocket.enableTrace(False)
+        q = his + [{"role": "user", "content": ins}]
+        websocket.enableTrace(self.debug)
         wsUrl = self.config.create_url()
-        ws = websocket.WebSocketApp(wsUrl, 
-                                    on_message=SparkDeskAPI.on_message, 
-                                    on_error=SparkDeskAPI.on_error, 
-                                    on_close=SparkDeskAPI.on_close, 
-                                    on_open=SparkDeskAPI.on_open)
+        ws = websocket.WebSocketApp(wsUrl,
+                                    on_message=CustomSaasAPI.on_message,
+                                    on_error=CustomSaasAPI.on_error,
+                                    on_close=CustomSaasAPI.on_close,
+                                    on_open=CustomSaasAPI.on_open)
         ws.appid = self.config.APPID
+        ws.domain = self.config.DOMAIN
         ws.question = q
         ws.max_length = max_length
         ws.top_p = top_p
-        ws.temperature = temperature        
+        ws.temperature = temperature
         ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
-        
+
         result = []
 
-        t  = reponse_queue.get(timeout=30)
+        t  = reponse_queue.get(timeout=self.timeout)
         while t is not None:
             result.append(t)
-            t  = reponse_queue.get(timeout=30)
-           
-
-        return [("".join(result),"")]
+            t  = reponse_queue.get(timeout=self.timeout)       
+         
+        return [("".join(result),"")]
```

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/__init__.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 from byzerllm.stable_diffusion.config import stableDiffusionConfig
 
 from byzerllm.stable_diffusion.model import DiffusersModel
 from byzerllm.stable_diffusion.utils import b642img
 
 # model_name = "runwayml/stable-diffusion-v1-5"
 
+def get_meta(self): 
+      
+    return [{
+        "model_deploy_type": "proprietary",
+        "backend":"transformers",    
+        "message_format":True,
+    }]
 
 def stream_chat(
     self,
     tokenizer,
     ins: str,
     his: List[Dict[str, str]] = [],
     max_length: int = 4090,
@@ -69,15 +76,15 @@
         views_batch_size=views_batch_size,
         window_size=window_size,
         stride=stride,
         init_image=init_image,
         strength=strength,
     )
     flatten = lambda l: [item for sublist in l for item in sublist]
-    content = json.dumps(flatten(images))
+    content = json.dumps(flatten(images),ensure_ascii=False)
     return [(content, "")]
 
 
 def init_model(
     model_dir, infer_params: Dict[str, str] = {}, sys_conf: Dict[str, str] = {}
 ):
     stableDiffusionConfig.set_model_dir(model_dir)
@@ -98,14 +105,15 @@
     stableDiffusionConfig.set_precision(precision)
 
     model = DiffusersModel(model_id=model_dir, variant=variant, checkpoint=checkpoint)
     model.activate()
     import types
 
     model.stream_chat = types.MethodType(stream_chat, model)
+    model.get_meta = types.MethodType(get_meta, model)
     return (model, None)
 
 
 # sampler_name SCHEDULERS.keys()
 # samping_steps min=1,max=100
 # batch_size min=1,max=50
 # batch_count min=1,max=50
```

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/__init__.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/generation.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/generation.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/models/diffusion.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/models/diffusion.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/config.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/embeddings.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/embeddings.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/utils.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/images.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/images.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/model.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/shared.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/shared.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/stable_diffusion/utils.py` & `byzerllm-0.1.90/src/byzerllm/stable_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/starcode/__init__.py` & `byzerllm-0.1.90/src/byzerllm/starcode/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from transformers import AutoTokenizer, AutoModelForCausalLM
 import transformers
 import torch
 from typing import Dict,List,Tuple
 
 
+def get_meta(self): 
+    config = self.config   
+    return [{
+        "model_deploy_type": "proprietary",
+        "backend":"transformers",
+        "max_model_len":getattr(config, "model_max_length", -1),
+        "architectures":getattr(config, "architectures", [])
+    }]
 
 def stream_chat(self,tokenizer,ins:str, his:List[Tuple[str,str]]=[],  
         max_length:int=4096, 
         top_p:float=0.95,
         temperature:float=0.1,**kwargs):
         
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
@@ -29,11 +37,12 @@
     tokenizer.pad_token_id=0 
     model = AutoModelForCausalLM.from_pretrained(model_dir,trust_remote_code=True,
                                                 device_map='auto',                                                
                                                 torch_dtype=torch.bfloat16                                                
                                                 )
     model.eval()       
     import types
-    model.stream_chat = types.MethodType(stream_chat, model)     
+    model.stream_chat = types.MethodType(stream_chat, model)  
+    model.get_meta = types.MethodType(get_meta, model)   
     return (model,tokenizer)
```

### Comparing `byzerllm-0.1.9/src/byzerllm/store.py` & `byzerllm-0.1.90/src/byzerllm/store.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/config/__init__.py` & `byzerllm-0.1.90/src/byzerllm/utils/config/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/emb.py` & `byzerllm-0.1.90/src/byzerllm/utils/emb.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/fulltune/__init__.py` & `byzerllm-0.1.90/src/byzerllm/utils/fulltune/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py` & `byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py` & `byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/fulltune/deepspeed_trainner.py` & `byzerllm-0.1.90/src/byzerllm/utils/fulltune/deepspeed_trainner.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/fulltune/launch.py` & `byzerllm-0.1.90/src/byzerllm/utils/fulltune/launch.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/__init__.py` & `byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,14 +659,15 @@
     if detached:        
         options["lifetime"] = "detached"
                 
     worker_cls = ray.remote(**options)(DeepSpeedTrainer).remote
     trainer = worker_cls(name=sft_name)
 
     if detached:
+        print_flush(f"[{sft_name}] Detached mode is enabled. ")
         trainer.sfft_train.remote(data_refs,train_params,sys_conf)        
         return []
         
     chunks,obj_count = ray.get(trainer.sfft_train.remote(data_refs,train_params,sys_conf))    
     checkpoint_path = ray.get(trainer.get_checkpoint_path.remote())
     node = ray.get(trainer.dst.resource_workers[0].get_node_ip_address.remote())
     print_flush(f"The model is finised training, Please check the path: {node}:{checkpoint_path}")
```

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py` & `byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/fulltune/trainner.py` & `byzerllm-0.1.90/src/byzerllm/utils/fulltune/trainner.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/metrics/__init__.py` & `byzerllm-0.1.90/src/byzerllm/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/retrieval/rest.py` & `byzerllm-0.1.90/src/byzerllm/utils/retrieval/rest.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/sft/__init__.py` & `byzerllm-0.1.90/src/byzerllm/utils/sft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,42 +91,43 @@
             os.makedirs(os.path.dirname(train_file))
 
         if "localModelDir" not in self.train_params:
             restore_model(self.conf,self.sft_config["model_name_or_path"])                                  
         
         
         # prepare data
-        with open(train_file,"w") as f: 
-            count = 0
-            for item in RayContext.collect_from(self.data_refs):                
-                if "conversation" in item:
-                    item["conversation"] = item["conversation"].tolist()
-                    s = json.dumps(item,ensure_ascii=False)               
-                    f.write(s+"\n")                    
-                elif "instruction" in item and "output" in item :
-                    # support alpaca format data
-                    history = item.get("history",[]) 
-                    
-                    if hasattr(history,"tolist"):
-                        history = history.tolist()
-
-                    input = item.get("input","")
-                    conversation = [sub.tolist() for sub in history]
-                    conversation = [{"human":x[0],"assistant":x[1]} for x in conversation]
-                    latest_conversation = [{"human":item["instruction"]+"\n"+input,"assistant":item["output"]}] if "instruction" in item and item["instruction"] else []
-                    s = json.dumps({
-                        "category":"",
-                        "conversation":conversation + latest_conversation,
-                        "conversation_id":count,
-                        "dataset":"",                
-                    },ensure_ascii=False)               
-                    f.write(s+"\n") 
-                else:
-                    raise Exception(f"Unknown data format: {item}")                                            
-                count += 1       
+        if self.data_refs:
+            with open(train_file,"w") as f: 
+                count = 0
+                for item in RayContext.collect_from(self.data_refs):                
+                    if "conversation" in item:
+                        item["conversation"] = item["conversation"].tolist()
+                        s = json.dumps(item,ensure_ascii=False)               
+                        f.write(s+"\n")                    
+                    elif "instruction" in item and "output" in item :
+                        # support alpaca format data
+                        history = item.get("history",[]) 
+                        
+                        if hasattr(history,"tolist"):
+                            history = history.tolist()
+
+                        input = item.get("input","")
+                        conversation = [sub.tolist() for sub in history]
+                        conversation = [{"human":x[0],"assistant":x[1]} for x in conversation]
+                        latest_conversation = [{"human":item["instruction"]+"\n"+input,"assistant":item["output"]}] if "instruction" in item and item["instruction"] else []
+                        s = json.dumps({
+                            "category":"",
+                            "conversation":conversation + latest_conversation,
+                            "conversation_id":count,
+                            "dataset":"",                
+                        },ensure_ascii=False)               
+                        f.write(s+"\n") 
+                    else:
+                        raise Exception(f"Unknown data format: {item}")                                            
+                    count += 1       
         
         ip,port = self.setup_tensorboard()
         print_flush(f"[{sft_name}] Tensorboard is running at: {ip}:{port}")
 
         final_path = QLoraTrainer.train(json.dumps(self.sft_config,ensure_ascii=False), args, {
             "model_type": self.train_params.get("model_type","casual_lm"),"sft_name":sft_name
         })
@@ -174,14 +175,18 @@
 
     if "localModelDir" in train_params:
         model_dir = train_params["localModelDir"]
 
     output_dir = os.path.join(localPathPrefix,rd,"finetune_model")
     logging_dir = os.path.join(localPathPrefix,rd,"logging")
     data_dir = os.path.join(localPathPrefix,rd,"finetune_data")
+    
+    if "data_dir" in train_params:
+        data_dir = train_params["data_dir"]
+
     data_file = os.path.join(data_dir,"data.jsonl")
 
     train_worker_conf = {}
     if "num_cpus" in sys_conf:
         train_worker_conf["num_cpus"] = float(sys_conf["num_cpus"])
 
     if "num_gpus" in sys_conf:
@@ -225,18 +230,19 @@
        **{
            "output_dir":output_dir,
            "logging_dir": logging_dir,
            "model_name_or_path":model_dir,
            "train_file":data_file,
        }
     }         
-        
-    detached = train_params.get("detached","false") == "true"
+    
+    detached = train_params.get("detached","true") == "true"
     
     if detached:
+        print_flush(f"[{sft_name}] Detached mode is enabled. ")
         train_actor = SFT.options(name=sft_name,lifetime="detached", **train_worker_conf).remote(data_refs,sft_config,train_params,sys_conf)
         train_actor.train.remote([])
         return [] 
 
     train_actor = SFT.options(name=sft_name,**train_worker_conf).remote(data_refs,sft_config,train_params,sys_conf)
     try:        
         items,obj_count = ray.get(train_actor.train.remote([]))
```

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/sft/argument.py` & `byzerllm-0.1.90/src/byzerllm/utils/sft/argument.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/sft/collator.py` & `byzerllm-0.1.90/src/byzerllm/utils/sft/collator.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/sft/dataset.py` & `byzerllm-0.1.90/src/byzerllm/utils/sft/dataset.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/sft/loss.py` & `byzerllm-0.1.90/src/byzerllm/utils/sft/loss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/sft/merge_lora.py` & `byzerllm-0.1.90/src/byzerllm/utils/sft/merge_lora.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/sft/model.py` & `byzerllm-0.1.90/src/byzerllm/utils/sft/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/sft/qlora.py` & `byzerllm-0.1.90/src/byzerllm/utils/sft/qlora.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/sft/trainer.py` & `byzerllm-0.1.90/src/byzerllm/utils/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/utils/testing.py` & `byzerllm-0.1.90/src/byzerllm/utils/testing.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/visualglm/__init__.py` & `byzerllm-0.1.90/src/byzerllm/visualglm/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.9/src/byzerllm/whisper/whisper_inference.py` & `byzerllm-0.1.90/src/byzerllm/whisper/whisper_inference.py`

 * *Files identical despite different names*


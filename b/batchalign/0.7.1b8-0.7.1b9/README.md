# Comparing `tmp/batchalign-0.7.1b8.tar.gz` & `tmp/batchalign-0.7.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchalign-0.7.1b8.tar", last modified: Thu May 23 08:37:55 2024, max compression
+gzip compressed data, was "batchalign-0.7.1b9.tar", last modified: Fri May 24 05:10:54 2024, max compression
```

## Comparing `batchalign-0.7.1b8.tar` & `batchalign-0.7.1b9.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.573701 batchalign-0.7.1b8/
--rw-r--r--   0 houjun     (501) staff       (20)     1464 2024-01-21 18:39:49.000000 batchalign-0.7.1b8/LICENSE
--rw-r--r--   0 houjun     (501) staff       (20)      149 2024-04-04 00:32:13.000000 batchalign-0.7.1b8/MANIFEST.in
--rw-r--r--   0 houjun     (501) staff       (20)    11951 2024-05-23 08:37:55.573429 batchalign-0.7.1b8/PKG-INFO
--rw-r--r--   0 houjun     (501) staff       (20)     9074 2024-05-12 20:56:18.000000 batchalign-0.7.1b8/README.md
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.552982 batchalign-0.7.1b8/batchalign/
--rw-r--r--   0 houjun     (501) staff       (20)      497 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)       63 2023-12-17 23:06:14.000000 batchalign-0.7.1b8/batchalign/__main__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.554148 batchalign-0.7.1b8/batchalign/cli/
--rw-r--r--   0 houjun     (501) staff       (20)       28 2023-12-17 01:12:36.000000 batchalign-0.7.1b8/batchalign/cli/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)    10089 2024-05-21 16:25:29.000000 batchalign-0.7.1b8/batchalign/cli/cli.py
--rw-r--r--   0 houjun     (501) staff       (20)     7568 2024-04-14 17:16:00.000000 batchalign-0.7.1b8/batchalign/cli/dispatch.py
--rw-r--r--   0 houjun     (501) staff       (20)      777 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/constants.py
--rw-r--r--   0 houjun     (501) staff       (20)    14798 2024-04-20 21:56:18.000000 batchalign-0.7.1b8/batchalign/document.py
--rw-r--r--   0 houjun     (501) staff       (20)      199 2023-12-17 07:10:18.000000 batchalign-0.7.1b8/batchalign/errors.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.554618 batchalign-0.7.1b8/batchalign/formats/
--rw-r--r--   0 houjun     (501) staff       (20)       62 2024-03-18 04:57:14.000000 batchalign-0.7.1b8/batchalign/formats/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      246 2023-12-18 07:14:44.000000 batchalign-0.7.1b8/batchalign/formats/base.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.555907 batchalign-0.7.1b8/batchalign/formats/chat/
--rw-r--r--   0 houjun     (501) staff       (20)       27 2024-03-18 04:57:14.000000 batchalign-0.7.1b8/batchalign/formats/chat/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     4676 2024-04-05 17:07:15.000000 batchalign-0.7.1b8/batchalign/formats/chat/file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3701 2024-04-05 17:08:43.000000 batchalign-0.7.1b8/batchalign/formats/chat/generator.py
--rw-r--r--   0 houjun     (501) staff       (20)     7481 2023-12-28 03:10:19.000000 batchalign-0.7.1b8/batchalign/formats/chat/lexer.py
--rw-r--r--   0 houjun     (501) staff       (20)    12453 2024-05-20 21:27:23.000000 batchalign-0.7.1b8/batchalign/formats/chat/parser.py
--rw-r--r--   0 houjun     (501) staff       (20)     5217 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/formats/chat/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.556881 batchalign-0.7.1b8/batchalign/formats/textgrid/
--rw-r--r--   0 houjun     (501) staff       (20)       31 2023-12-18 07:14:59.000000 batchalign-0.7.1b8/batchalign/formats/textgrid/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3340 2024-03-18 04:57:14.000000 batchalign-0.7.1b8/batchalign/formats/textgrid/file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3485 2023-12-18 07:35:03.000000 batchalign-0.7.1b8/batchalign/formats/textgrid/generator.py
--rw-r--r--   0 houjun     (501) staff       (20)     3888 2023-12-18 05:59:42.000000 batchalign-0.7.1b8/batchalign/formats/textgrid/parser.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.557563 batchalign-0.7.1b8/batchalign/models/
--rw-r--r--   0 houjun     (501) staff       (20)      195 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      454 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/models/resolve.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.558470 batchalign-0.7.1b8/batchalign/models/speaker/
--rw-r--r--   0 houjun     (501) staff       (20)       36 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/speaker/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     5583 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/speaker/config.yaml
--rw-r--r--   0 houjun     (501) staff       (20)     3246 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/speaker/infer.py
--rw-r--r--   0 houjun     (501) staff       (20)     1808 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/speaker/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.558874 batchalign-0.7.1b8/batchalign/models/training/
--rw-r--r--   0 houjun     (501) staff       (20)       22 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/models/training/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      576 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/training/run.py
--rw-r--r--   0 houjun     (501) staff       (20)     3357 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/models/training/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     3081 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/models/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.559718 batchalign-0.7.1b8/batchalign/models/utterance/
--rw-r--r--   0 houjun     (501) staff       (20)       39 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/utterance/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     5447 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/utterance/dataset.py
--rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/utterance/execute.py
--rw-r--r--   0 houjun     (501) staff       (20)     3179 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/utterance/infer.py
--rw-r--r--   0 houjun     (501) staff       (20)     3057 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/utterance/prep.py
--rw-r--r--   0 houjun     (501) staff       (20)     4359 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/utterance/train.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.560121 batchalign-0.7.1b8/batchalign/models/whisper/
--rw-r--r--   0 houjun     (501) staff       (20)       76 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/whisper/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     7340 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/models/whisper/infer_asr.py
--rw-r--r--   0 houjun     (501) staff       (20)     5264 2024-04-08 19:13:44.000000 batchalign-0.7.1b8/batchalign/models/whisper/infer_fa.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.561037 batchalign-0.7.1b8/batchalign/pipelines/
--rw-r--r--   0 houjun     (501) staff       (20)      449 2024-04-14 00:00:03.000000 batchalign-0.7.1b8/batchalign/pipelines/__init__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.561420 batchalign-0.7.1b8/batchalign/pipelines/analysis/
--rw-r--r--   0 houjun     (501) staff       (20)       35 2024-02-05 03:35:25.000000 batchalign-0.7.1b8/batchalign/pipelines/analysis/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     2557 2024-02-05 03:35:25.000000 batchalign-0.7.1b8/batchalign/pipelines/analysis/eval.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.562467 batchalign-0.7.1b8/batchalign/pipelines/asr/
--rw-r--r--   0 houjun     (501) staff       (20)       99 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/pipelines/asr/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3723 2024-04-14 05:49:03.000000 batchalign-0.7.1b8/batchalign/pipelines/asr/rev.py
--rw-r--r--   0 houjun     (501) staff       (20)     7227 2024-04-14 04:23:55.000000 batchalign-0.7.1b8/batchalign/pipelines/asr/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     2063 2024-04-14 05:49:03.000000 batchalign-0.7.1b8/batchalign/pipelines/asr/whisper.py
--rw-r--r--   0 houjun     (501) staff       (20)     4403 2024-04-14 05:49:03.000000 batchalign-0.7.1b8/batchalign/pipelines/asr/whisperx.py
--rw-r--r--   0 houjun     (501) staff       (20)     1994 2024-02-05 03:35:25.000000 batchalign-0.7.1b8/batchalign/pipelines/base.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.563540 batchalign-0.7.1b8/batchalign/pipelines/cleanup/
--rw-r--r--   0 houjun     (501) staff       (20)       52 2023-12-16 19:37:43.000000 batchalign-0.7.1b8/batchalign/pipelines/cleanup/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)       93 2023-12-17 00:16:09.000000 batchalign-0.7.1b8/batchalign/pipelines/cleanup/cleanup.py
--rw-r--r--   0 houjun     (501) staff       (20)      579 2024-02-05 03:35:25.000000 batchalign-0.7.1b8/batchalign/pipelines/cleanup/disfluencies.py
--rw-r--r--   0 houjun     (501) staff       (20)     2161 2023-12-08 20:58:29.000000 batchalign-0.7.1b8/batchalign/pipelines/cleanup/parse_support.py
--rw-r--r--   0 houjun     (501) staff       (20)     2624 2024-02-05 03:35:25.000000 batchalign-0.7.1b8/batchalign/pipelines/cleanup/retrace.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.564470 batchalign-0.7.1b8/batchalign/pipelines/cleanup/support/
--rw-r--r--   0 houjun     (501) staff       (20)      141 2023-12-09 06:23:35.000000 batchalign-0.7.1b8/batchalign/pipelines/cleanup/support/filled_pauses.eng
--rw-r--r--   0 houjun     (501) staff       (20)      213 2023-12-09 06:23:34.000000 batchalign-0.7.1b8/batchalign/pipelines/cleanup/support/replacements.eng
--rw-r--r--   0 houjun     (501) staff       (20)      203 2024-03-18 04:54:03.000000 batchalign-0.7.1b8/batchalign/pipelines/cleanup/support/test.test
--rw-r--r--   0 houjun     (501) staff       (20)     4135 2024-05-17 19:29:50.000000 batchalign-0.7.1b8/batchalign/pipelines/dispatch.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.564986 batchalign-0.7.1b8/batchalign/pipelines/fa/
--rw-r--r--   0 houjun     (501) staff       (20)       40 2023-12-16 01:03:14.000000 batchalign-0.7.1b8/batchalign/pipelines/fa/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     7492 2024-04-20 18:30:40.000000 batchalign-0.7.1b8/batchalign/pipelines/fa/whisper_fa.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.565472 batchalign-0.7.1b8/batchalign/pipelines/morphosyntax/
--rw-r--r--   0 houjun     (501) staff       (20)       29 2023-12-16 23:54:03.000000 batchalign-0.7.1b8/batchalign/pipelines/morphosyntax/__init__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.565619 batchalign-0.7.1b8/batchalign/pipelines/morphosyntax/fr/
--rw-r--r--   0 houjun     (501) staff       (20)     1147 2023-12-29 00:44:35.000000 batchalign-0.7.1b8/batchalign/pipelines/morphosyntax/fr/case.py
--rw-r--r--   0 houjun     (501) staff       (20)    31445 2024-05-23 08:36:28.000000 batchalign-0.7.1b8/batchalign/pipelines/morphosyntax/ud.py
--rw-r--r--   0 houjun     (501) staff       (20)     7482 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/pipelines/pipeline.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.565990 batchalign-0.7.1b8/batchalign/pipelines/speaker/
--rw-r--r--   0 houjun     (501) staff       (20)       44 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/pipelines/speaker/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     2367 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/batchalign/pipelines/speaker/nemo_speaker.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.566675 batchalign-0.7.1b8/batchalign/pipelines/utr/
--rw-r--r--   0 houjun     (501) staff       (20)       76 2024-01-03 22:34:21.000000 batchalign-0.7.1b8/batchalign/pipelines/utr/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3525 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/pipelines/utr/rev_utr.py
--rw-r--r--   0 houjun     (501) staff       (20)     2303 2024-04-19 03:00:06.000000 batchalign-0.7.1b8/batchalign/pipelines/utr/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     1559 2024-02-05 03:35:25.000000 batchalign-0.7.1b8/batchalign/pipelines/utr/whisper_utr.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.567139 batchalign-0.7.1b8/batchalign/pipelines/utterance/
--rw-r--r--   0 houjun     (501) staff       (20)       48 2024-04-13 19:17:01.000000 batchalign-0.7.1b8/batchalign/pipelines/utterance/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)    10922 2024-04-16 21:19:29.000000 batchalign-0.7.1b8/batchalign/pipelines/utterance/ud_utterance.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.567742 batchalign-0.7.1b8/batchalign/tests/
--rw-r--r--   0 houjun     (501) staff       (20)        0 2023-11-18 22:44:12.000000 batchalign-0.7.1b8/batchalign/tests/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     1497 2024-03-18 04:54:03.000000 batchalign-0.7.1b8/batchalign/tests/conftest.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.550953 batchalign-0.7.1b8/batchalign/tests/formats/
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.568659 batchalign-0.7.1b8/batchalign/tests/formats/chat/
--rw-r--r--   0 houjun     (501) staff       (20)      999 2024-03-18 04:57:14.000000 batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3913 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_generator.py
--rw-r--r--   0 houjun     (501) staff       (20)      714 2023-12-24 23:29:13.000000 batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_lexer.py
--rw-r--r--   0 houjun     (501) staff       (20)    10624 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_parser.py
--rw-r--r--   0 houjun     (501) staff       (20)     1046 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.568786 batchalign-0.7.1b8/batchalign/tests/formats/textgrid/
--rw-r--r--   0 houjun     (501) staff       (20)     2699 2024-03-18 04:54:03.000000 batchalign-0.7.1b8/batchalign/tests/formats/textgrid/test_textgrid.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.569358 batchalign-0.7.1b8/batchalign/tests/pipelines/
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.569527 batchalign-0.7.1b8/batchalign/tests/pipelines/analysis/
--rw-r--r--   0 houjun     (501) staff       (20)      604 2024-02-05 03:35:25.000000 batchalign-0.7.1b8/batchalign/tests/pipelines/analysis/test_eval.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.570015 batchalign-0.7.1b8/batchalign/tests/pipelines/asr/
--rw-r--r--   0 houjun     (501) staff       (20)      938 2024-03-18 04:54:03.000000 batchalign-0.7.1b8/batchalign/tests/pipelines/asr/test_asr_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)     1570 2024-01-02 20:37:42.000000 batchalign-0.7.1b8/batchalign/tests/pipelines/asr/test_asr_utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.570417 batchalign-0.7.1b8/batchalign/tests/pipelines/cleanup/
--rw-r--r--   0 houjun     (501) staff       (20)     2716 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/tests/pipelines/cleanup/test_disfluency.py
--rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-03-18 04:54:03.000000 batchalign-0.7.1b8/batchalign/tests/pipelines/cleanup/test_parse_support.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.570547 batchalign-0.7.1b8/batchalign/tests/pipelines/fa/
--rw-r--r--   0 houjun     (501) staff       (20)      261 2024-04-08 19:15:55.000000 batchalign-0.7.1b8/batchalign/tests/pipelines/fa/test_fa_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)      977 2024-03-18 04:54:03.000000 batchalign-0.7.1b8/batchalign/tests/pipelines/fixures.py
--rw-r--r--   0 houjun     (501) staff       (20)     4441 2024-03-18 04:54:03.000000 batchalign-0.7.1b8/batchalign/tests/pipelines/test_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)      555 2024-03-18 04:54:03.000000 batchalign-0.7.1b8/batchalign/tests/pipelines/test_pipeline_models.py
--rw-r--r--   0 houjun     (501) staff       (20)     2472 2024-03-18 04:54:03.000000 batchalign-0.7.1b8/batchalign/tests/test_document.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.571417 batchalign-0.7.1b8/batchalign/utils/
--rw-r--r--   0 houjun     (501) staff       (20)       21 2023-12-16 23:44:38.000000 batchalign-0.7.1b8/batchalign/utils/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3513 2023-12-23 18:18:28.000000 batchalign-0.7.1b8/batchalign/utils/config.py
--rw-r--r--   0 houjun     (501) staff       (20)     7689 2024-01-18 23:05:56.000000 batchalign-0.7.1b8/batchalign/utils/dp.py
--rw-r--r--   0 houjun     (501) staff       (20)     2788 2024-04-01 06:52:40.000000 batchalign-0.7.1b8/batchalign/utils/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)       56 2024-05-23 08:37:41.000000 batchalign-0.7.1b8/batchalign/version
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-23 08:37:55.553709 batchalign-0.7.1b8/batchalign.egg-info/
--rw-r--r--   0 houjun     (501) staff       (20)    11951 2024-05-23 08:37:55.000000 batchalign-0.7.1b8/batchalign.egg-info/PKG-INFO
--rw-r--r--   0 houjun     (501) staff       (20)     3776 2024-05-23 08:37:55.000000 batchalign-0.7.1b8/batchalign.egg-info/SOURCES.txt
--rw-r--r--   0 houjun     (501) staff       (20)        1 2024-05-23 08:37:55.000000 batchalign-0.7.1b8/batchalign.egg-info/dependency_links.txt
--rw-r--r--   0 houjun     (501) staff       (20)       61 2024-05-23 08:37:55.000000 batchalign-0.7.1b8/batchalign.egg-info/entry_points.txt
--rw-r--r--   0 houjun     (501) staff       (20)      902 2024-05-23 08:37:55.000000 batchalign-0.7.1b8/batchalign.egg-info/requires.txt
--rw-r--r--   0 houjun     (501) staff       (20)       11 2024-05-23 08:37:55.000000 batchalign-0.7.1b8/batchalign.egg-info/top_level.txt
--rw-r--r--   0 houjun     (501) staff       (20)       38 2024-05-23 08:37:55.573735 batchalign-0.7.1b8/setup.cfg
--rw-r--r--   0 houjun     (501) staff       (20)     2983 2024-04-01 06:52:43.000000 batchalign-0.7.1b8/setup.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.596790 batchalign-0.7.1b9/
+-rw-r--r--   0 houjun     (501) staff       (20)     1464 2024-01-21 18:39:49.000000 batchalign-0.7.1b9/LICENSE
+-rw-r--r--   0 houjun     (501) staff       (20)      149 2024-04-04 00:32:13.000000 batchalign-0.7.1b9/MANIFEST.in
+-rw-r--r--   0 houjun     (501) staff       (20)    11951 2024-05-24 05:10:54.596536 batchalign-0.7.1b9/PKG-INFO
+-rw-r--r--   0 houjun     (501) staff       (20)     9074 2024-05-12 20:56:18.000000 batchalign-0.7.1b9/README.md
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.574415 batchalign-0.7.1b9/batchalign/
+-rw-r--r--   0 houjun     (501) staff       (20)      497 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)       63 2023-12-17 23:06:14.000000 batchalign-0.7.1b9/batchalign/__main__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.575498 batchalign-0.7.1b9/batchalign/cli/
+-rw-r--r--   0 houjun     (501) staff       (20)       28 2023-12-17 01:12:36.000000 batchalign-0.7.1b9/batchalign/cli/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)    10091 2024-05-24 05:07:57.000000 batchalign-0.7.1b9/batchalign/cli/cli.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7568 2024-04-14 17:16:00.000000 batchalign-0.7.1b9/batchalign/cli/dispatch.py
+-rw-r--r--   0 houjun     (501) staff       (20)      777 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/constants.py
+-rw-r--r--   0 houjun     (501) staff       (20)    14861 2024-05-24 05:03:06.000000 batchalign-0.7.1b9/batchalign/document.py
+-rw-r--r--   0 houjun     (501) staff       (20)      199 2023-12-17 07:10:18.000000 batchalign-0.7.1b9/batchalign/errors.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.575973 batchalign-0.7.1b9/batchalign/formats/
+-rw-r--r--   0 houjun     (501) staff       (20)       62 2024-03-18 04:57:14.000000 batchalign-0.7.1b9/batchalign/formats/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      246 2023-12-18 07:14:44.000000 batchalign-0.7.1b9/batchalign/formats/base.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.576843 batchalign-0.7.1b9/batchalign/formats/chat/
+-rw-r--r--   0 houjun     (501) staff       (20)       27 2024-03-18 04:57:14.000000 batchalign-0.7.1b9/batchalign/formats/chat/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4676 2024-04-05 17:07:15.000000 batchalign-0.7.1b9/batchalign/formats/chat/file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3701 2024-04-05 17:08:43.000000 batchalign-0.7.1b9/batchalign/formats/chat/generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7481 2023-12-28 03:10:19.000000 batchalign-0.7.1b9/batchalign/formats/chat/lexer.py
+-rw-r--r--   0 houjun     (501) staff       (20)    12453 2024-05-24 05:04:54.000000 batchalign-0.7.1b9/batchalign/formats/chat/parser.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5217 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/formats/chat/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.577710 batchalign-0.7.1b9/batchalign/formats/textgrid/
+-rw-r--r--   0 houjun     (501) staff       (20)       31 2023-12-18 07:14:59.000000 batchalign-0.7.1b9/batchalign/formats/textgrid/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3340 2024-03-18 04:57:14.000000 batchalign-0.7.1b9/batchalign/formats/textgrid/file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3485 2023-12-18 07:35:03.000000 batchalign-0.7.1b9/batchalign/formats/textgrid/generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3888 2023-12-18 05:59:42.000000 batchalign-0.7.1b9/batchalign/formats/textgrid/parser.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.578201 batchalign-0.7.1b9/batchalign/models/
+-rw-r--r--   0 houjun     (501) staff       (20)      195 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      454 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/models/resolve.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.579002 batchalign-0.7.1b9/batchalign/models/speaker/
+-rw-r--r--   0 houjun     (501) staff       (20)       36 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/speaker/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5583 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/speaker/config.yaml
+-rw-r--r--   0 houjun     (501) staff       (20)     3246 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/speaker/infer.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1808 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/speaker/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.579425 batchalign-0.7.1b9/batchalign/models/training/
+-rw-r--r--   0 houjun     (501) staff       (20)       22 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/models/training/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      576 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/training/run.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3357 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/models/training/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3081 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/models/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.580183 batchalign-0.7.1b9/batchalign/models/utterance/
+-rw-r--r--   0 houjun     (501) staff       (20)       39 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/utterance/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5447 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/utterance/dataset.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/utterance/execute.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3179 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/utterance/infer.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3057 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/utterance/prep.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4359 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/utterance/train.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.580560 batchalign-0.7.1b9/batchalign/models/whisper/
+-rw-r--r--   0 houjun     (501) staff       (20)       76 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/whisper/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7340 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/models/whisper/infer_asr.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5264 2024-04-08 19:13:44.000000 batchalign-0.7.1b9/batchalign/models/whisper/infer_fa.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.581391 batchalign-0.7.1b9/batchalign/pipelines/
+-rw-r--r--   0 houjun     (501) staff       (20)      449 2024-04-14 00:00:03.000000 batchalign-0.7.1b9/batchalign/pipelines/__init__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.581725 batchalign-0.7.1b9/batchalign/pipelines/analysis/
+-rw-r--r--   0 houjun     (501) staff       (20)       35 2024-02-05 03:35:25.000000 batchalign-0.7.1b9/batchalign/pipelines/analysis/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2557 2024-02-05 03:35:25.000000 batchalign-0.7.1b9/batchalign/pipelines/analysis/eval.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.582809 batchalign-0.7.1b9/batchalign/pipelines/asr/
+-rw-r--r--   0 houjun     (501) staff       (20)       99 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/pipelines/asr/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3723 2024-04-14 05:49:03.000000 batchalign-0.7.1b9/batchalign/pipelines/asr/rev.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7227 2024-04-14 04:23:55.000000 batchalign-0.7.1b9/batchalign/pipelines/asr/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2063 2024-04-14 05:49:03.000000 batchalign-0.7.1b9/batchalign/pipelines/asr/whisper.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4403 2024-04-14 05:49:03.000000 batchalign-0.7.1b9/batchalign/pipelines/asr/whisperx.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1994 2024-02-05 03:35:25.000000 batchalign-0.7.1b9/batchalign/pipelines/base.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.583898 batchalign-0.7.1b9/batchalign/pipelines/cleanup/
+-rw-r--r--   0 houjun     (501) staff       (20)       52 2023-12-16 19:37:43.000000 batchalign-0.7.1b9/batchalign/pipelines/cleanup/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)       93 2023-12-17 00:16:09.000000 batchalign-0.7.1b9/batchalign/pipelines/cleanup/cleanup.py
+-rw-r--r--   0 houjun     (501) staff       (20)      579 2024-02-05 03:35:25.000000 batchalign-0.7.1b9/batchalign/pipelines/cleanup/disfluencies.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2161 2023-12-08 20:58:29.000000 batchalign-0.7.1b9/batchalign/pipelines/cleanup/parse_support.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2624 2024-02-05 03:35:25.000000 batchalign-0.7.1b9/batchalign/pipelines/cleanup/retrace.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.584597 batchalign-0.7.1b9/batchalign/pipelines/cleanup/support/
+-rw-r--r--   0 houjun     (501) staff       (20)      141 2023-12-09 06:23:35.000000 batchalign-0.7.1b9/batchalign/pipelines/cleanup/support/filled_pauses.eng
+-rw-r--r--   0 houjun     (501) staff       (20)      213 2023-12-09 06:23:34.000000 batchalign-0.7.1b9/batchalign/pipelines/cleanup/support/replacements.eng
+-rw-r--r--   0 houjun     (501) staff       (20)      203 2024-03-18 04:54:03.000000 batchalign-0.7.1b9/batchalign/pipelines/cleanup/support/test.test
+-rw-r--r--   0 houjun     (501) staff       (20)     4135 2024-05-17 19:29:50.000000 batchalign-0.7.1b9/batchalign/pipelines/dispatch.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.585089 batchalign-0.7.1b9/batchalign/pipelines/fa/
+-rw-r--r--   0 houjun     (501) staff       (20)       40 2023-12-16 01:03:14.000000 batchalign-0.7.1b9/batchalign/pipelines/fa/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7492 2024-04-20 18:30:40.000000 batchalign-0.7.1b9/batchalign/pipelines/fa/whisper_fa.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.585567 batchalign-0.7.1b9/batchalign/pipelines/morphosyntax/
+-rw-r--r--   0 houjun     (501) staff       (20)       29 2023-12-16 23:54:03.000000 batchalign-0.7.1b9/batchalign/pipelines/morphosyntax/__init__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.585702 batchalign-0.7.1b9/batchalign/pipelines/morphosyntax/fr/
+-rw-r--r--   0 houjun     (501) staff       (20)     1147 2023-12-29 00:44:35.000000 batchalign-0.7.1b9/batchalign/pipelines/morphosyntax/fr/case.py
+-rw-r--r--   0 houjun     (501) staff       (20)    31445 2024-05-23 08:36:28.000000 batchalign-0.7.1b9/batchalign/pipelines/morphosyntax/ud.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7482 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/pipelines/pipeline.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.586034 batchalign-0.7.1b9/batchalign/pipelines/speaker/
+-rw-r--r--   0 houjun     (501) staff       (20)       44 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/pipelines/speaker/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2367 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/batchalign/pipelines/speaker/nemo_speaker.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.588992 batchalign-0.7.1b9/batchalign/pipelines/utr/
+-rw-r--r--   0 houjun     (501) staff       (20)       76 2024-01-03 22:34:21.000000 batchalign-0.7.1b9/batchalign/pipelines/utr/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3525 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/pipelines/utr/rev_utr.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2303 2024-04-19 03:00:06.000000 batchalign-0.7.1b9/batchalign/pipelines/utr/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1559 2024-02-05 03:35:25.000000 batchalign-0.7.1b9/batchalign/pipelines/utr/whisper_utr.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.589416 batchalign-0.7.1b9/batchalign/pipelines/utterance/
+-rw-r--r--   0 houjun     (501) staff       (20)       48 2024-04-13 19:17:01.000000 batchalign-0.7.1b9/batchalign/pipelines/utterance/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)    10922 2024-04-16 21:19:29.000000 batchalign-0.7.1b9/batchalign/pipelines/utterance/ud_utterance.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.589935 batchalign-0.7.1b9/batchalign/tests/
+-rw-r--r--   0 houjun     (501) staff       (20)        0 2023-11-18 22:44:12.000000 batchalign-0.7.1b9/batchalign/tests/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1497 2024-03-18 04:54:03.000000 batchalign-0.7.1b9/batchalign/tests/conftest.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.572445 batchalign-0.7.1b9/batchalign/tests/formats/
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.591890 batchalign-0.7.1b9/batchalign/tests/formats/chat/
+-rw-r--r--   0 houjun     (501) staff       (20)      999 2024-03-18 04:57:14.000000 batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3913 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)      714 2023-12-24 23:29:13.000000 batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_lexer.py
+-rw-r--r--   0 houjun     (501) staff       (20)    10624 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_parser.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1046 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.592032 batchalign-0.7.1b9/batchalign/tests/formats/textgrid/
+-rw-r--r--   0 houjun     (501) staff       (20)     2699 2024-03-18 04:54:03.000000 batchalign-0.7.1b9/batchalign/tests/formats/textgrid/test_textgrid.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.592585 batchalign-0.7.1b9/batchalign/tests/pipelines/
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.592712 batchalign-0.7.1b9/batchalign/tests/pipelines/analysis/
+-rw-r--r--   0 houjun     (501) staff       (20)      604 2024-02-05 03:35:25.000000 batchalign-0.7.1b9/batchalign/tests/pipelines/analysis/test_eval.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.593077 batchalign-0.7.1b9/batchalign/tests/pipelines/asr/
+-rw-r--r--   0 houjun     (501) staff       (20)      938 2024-03-18 04:54:03.000000 batchalign-0.7.1b9/batchalign/tests/pipelines/asr/test_asr_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1570 2024-01-02 20:37:42.000000 batchalign-0.7.1b9/batchalign/tests/pipelines/asr/test_asr_utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.593444 batchalign-0.7.1b9/batchalign/tests/pipelines/cleanup/
+-rw-r--r--   0 houjun     (501) staff       (20)     2716 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/tests/pipelines/cleanup/test_disfluency.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-03-18 04:54:03.000000 batchalign-0.7.1b9/batchalign/tests/pipelines/cleanup/test_parse_support.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.593580 batchalign-0.7.1b9/batchalign/tests/pipelines/fa/
+-rw-r--r--   0 houjun     (501) staff       (20)      261 2024-04-08 19:15:55.000000 batchalign-0.7.1b9/batchalign/tests/pipelines/fa/test_fa_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)      977 2024-03-18 04:54:03.000000 batchalign-0.7.1b9/batchalign/tests/pipelines/fixures.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4441 2024-03-18 04:54:03.000000 batchalign-0.7.1b9/batchalign/tests/pipelines/test_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)      555 2024-03-18 04:54:03.000000 batchalign-0.7.1b9/batchalign/tests/pipelines/test_pipeline_models.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2472 2024-03-18 04:54:03.000000 batchalign-0.7.1b9/batchalign/tests/test_document.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.594426 batchalign-0.7.1b9/batchalign/utils/
+-rw-r--r--   0 houjun     (501) staff       (20)       21 2023-12-16 23:44:38.000000 batchalign-0.7.1b9/batchalign/utils/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3513 2023-12-23 18:18:28.000000 batchalign-0.7.1b9/batchalign/utils/config.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7689 2024-01-18 23:05:56.000000 batchalign-0.7.1b9/batchalign/utils/dp.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2788 2024-04-01 06:52:40.000000 batchalign-0.7.1b9/batchalign/utils/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)       64 2024-05-24 05:10:37.000000 batchalign-0.7.1b9/batchalign/version
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-05-24 05:10:54.575073 batchalign-0.7.1b9/batchalign.egg-info/
+-rw-r--r--   0 houjun     (501) staff       (20)    11951 2024-05-24 05:10:54.000000 batchalign-0.7.1b9/batchalign.egg-info/PKG-INFO
+-rw-r--r--   0 houjun     (501) staff       (20)     3776 2024-05-24 05:10:54.000000 batchalign-0.7.1b9/batchalign.egg-info/SOURCES.txt
+-rw-r--r--   0 houjun     (501) staff       (20)        1 2024-05-24 05:10:54.000000 batchalign-0.7.1b9/batchalign.egg-info/dependency_links.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       61 2024-05-24 05:10:54.000000 batchalign-0.7.1b9/batchalign.egg-info/entry_points.txt
+-rw-r--r--   0 houjun     (501) staff       (20)      902 2024-05-24 05:10:54.000000 batchalign-0.7.1b9/batchalign.egg-info/requires.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       11 2024-05-24 05:10:54.000000 batchalign-0.7.1b9/batchalign.egg-info/top_level.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       38 2024-05-24 05:10:54.596830 batchalign-0.7.1b9/setup.cfg
+-rw-r--r--   0 houjun     (501) staff       (20)     2983 2024-04-01 06:52:43.000000 batchalign-0.7.1b9/setup.py
```

### Comparing `batchalign-0.7.1b8/LICENSE` & `batchalign-0.7.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/PKG-INFO` & `batchalign-0.7.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchalign
-Version: 0.7.1b8
+Version: 0.7.1b9
 Summary: Python Speech Language Sample Analysis
 Author: Brian MacWhinney, Houjun Liu
 Author-email: macw@cmu.edu, houjun@cmu.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `batchalign-0.7.1b8/README.md` & `batchalign-0.7.1b9/README.md`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/cli/cli.py` & `batchalign-0.7.1b9/batchalign/cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,18 +115,18 @@
 @common_options
 @click.option("--whisper/--rev",
               default=False, help="For utterance timing recovery, OpenAI Whisper (ASR) instead of Rev.AI (default).")
 @click.pass_context
 def align(ctx, in_dir, out_dir, lang, num_speakers, whisper, **kwargs):
     """Align transcripts against corresponding media files."""
     def loader(file):
-        return CHATFile(path=os.path.abspath(file), special_mor_=True).doc
+        return CHATFile(path=os.path.abspath(file)).doc
 
     def writer(doc, output):
-        CHATFile(doc=doc, special_mor_=True).write(output)
+        CHATFile(doc=doc).write(output)
 
     _dispatch("align", lang, num_speakers,
               ["cha"], ctx,
               in_dir, out_dir,
               loader, writer, C,
               utr="whisper_utr" if whisper else "rev_utr",
               **kwargs)
@@ -155,19 +155,19 @@
     if kwargs["whisperx"]:
         asr = "whisperx"
 
 
     def writer(doc, output):
         doc.content.insert(0, CustomLine(id="Comment", type=CustomLineType.INDEPENDENT,
                                          content=f"Batchalign {VERSION_NUMBER.strip()}, ASR Engine {asr}"))
-        CHATFile(doc=doc, special_mor_=True).write(output
-                                                   .replace(".wav", ".cha")
-                                                   .replace(".mp4", ".cha")
-                                                   .replace(".mp3", ".cha"),
-                                                   write_wor=kwargs.get("wor", False))
+        CHATFile(doc=doc).write(output
+                                .replace(".wav", ".cha")
+                                .replace(".mp4", ".cha")
+                                .replace(".mp3", ".cha"),
+                                write_wor=kwargs.get("wor", False))
 
     if kwargs.get("diarize"):
         _dispatch("transcribe_s",
                   lang, num_speakers, ["mp3", "mp4", "wav"], ctx,
                   in_dir, out_dir,
                   loader, writer, C,
                   asr=asr, **kwargs)
@@ -188,31 +188,34 @@
               type=click.Path(exists=True,
                               file_okay=True, dir_okay=False),
               help="Comma seperated manual lexicon override")
 @click.pass_context
 def morphotag(ctx, in_dir, out_dir, lang, num_speakers, **kwargs):
     """Perform morphosyntactic analysis on transcripts."""
 
-   
     def loader(file):
         mwt = {}
         if kwargs.get("lexicon") != None and kwargs.get("lexicon", "").strip() != "":
             import csv
             raw = []
             with open(kwargs["lexicon"], 'r') as df:
                 raw = [i for i in csv.reader(df)]
             for i in raw:
                 mwt[i[0]] = tuple(i[1:])
+        cf = CHATFile(path=os.path.abspath(file), special_mor_=True)
+        doc = cf.doc
+        if str(cf).count("%mor") > 0:
+            doc.ba_special_["special_mor_notation"] = True
         return (
-            CHATFile(path=os.path.abspath(file), special_mor_=True).doc,
+            doc,
             {"retokenize": kwargs["retokenize"], "mwt": mwt}
         )
 
     def writer(doc, output):
-        CHATFile(doc=doc, special_mor_=True).write(output)
+        CHATFile(doc=doc, special_mor_=doc.ba_special_.get("special_mor_notation", False)).write(output)
 
     _dispatch("morphotag", lang, num_speakers, ["cha"], ctx,
               in_dir, out_dir,
               loader, writer, C)
 
 
 #################### UTSEG ################################
@@ -220,18 +223,18 @@
 @batchalign.command()
 @common_options
 @click.pass_context
 def utseg(ctx, in_dir, out_dir, lang, num_speakers, **kwargs):
     """Perform morphosyntactic analysis on transcripts."""
 
     def loader(file):
-        return CHATFile(path=os.path.abspath(file), special_mor_=True).doc
+        return CHATFile(path=os.path.abspath(file)).doc
 
     def writer(doc, output):
-        CHATFile(doc=doc, special_mor_=True).write(output)
+        CHATFile(doc=doc).write(output)
 
     _dispatch("utseg", lang, num_speakers, ["cha"], ctx,
               in_dir, out_dir,
               loader, writer, C)
 
 #################### BENCHMARK ################################
```

### Comparing `batchalign-0.7.1b8/batchalign/cli/dispatch.py` & `batchalign-0.7.1b9/batchalign/cli/dispatch.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/constants.py` & `batchalign-0.7.1b9/batchalign/constants.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/document.py` & `batchalign-0.7.1b9/batchalign/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum, IntEnum
-from typing import Optional, List, Tuple, Union
+from typing import Optional, List, Tuple, Union, Any, Dict
 from typing_extensions import Annotated
 
 from pydantic import BaseModel, Field, computed_field
 from pydantic.functional_validators import BeforeValidator
 
 from batchalign.utils import word_tokenize, sent_tokenize, detokenize
 
@@ -327,14 +327,15 @@
 
 class Document(BaseModel):
     content: Paragraph = Field(default=[])
     media: Optional[Media] = Field(default=None)
     langs: List[str] = Field(default=["eng"])
     # persistent digital identifier
     pid: Optional[str] = Field(default=None)
+    ba_special_: Optional[Dict] = Field(default={})
 
     def __repr__(self):
         return "\n".join(self.transcript())
 
     def __str__(self):
         return "\n".join(self.transcript())
```

### Comparing `batchalign-0.7.1b8/batchalign/formats/chat/file.py` & `batchalign-0.7.1b9/batchalign/formats/chat/file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/formats/chat/generator.py` & `batchalign-0.7.1b9/batchalign/formats/chat/generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/formats/chat/lexer.py` & `batchalign-0.7.1b9/batchalign/formats/chat/lexer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/formats/chat/parser.py` & `batchalign-0.7.1b9/batchalign/formats/chat/parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/formats/chat/utils.py` & `batchalign-0.7.1b9/batchalign/formats/chat/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/formats/textgrid/file.py` & `batchalign-0.7.1b9/batchalign/formats/textgrid/file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/formats/textgrid/generator.py` & `batchalign-0.7.1b9/batchalign/formats/textgrid/generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/formats/textgrid/parser.py` & `batchalign-0.7.1b9/batchalign/formats/textgrid/parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/speaker/config.yaml` & `batchalign-0.7.1b9/batchalign/models/speaker/config.yaml`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/speaker/infer.py` & `batchalign-0.7.1b9/batchalign/models/speaker/infer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/speaker/utils.py` & `batchalign-0.7.1b9/batchalign/models/speaker/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/training/run.py` & `batchalign-0.7.1b9/batchalign/models/training/run.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/training/utils.py` & `batchalign-0.7.1b9/batchalign/models/training/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/utils.py` & `batchalign-0.7.1b9/batchalign/models/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/utterance/dataset.py` & `batchalign-0.7.1b9/batchalign/models/utterance/dataset.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/utterance/execute.py` & `batchalign-0.7.1b9/batchalign/models/utterance/execute.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/utterance/infer.py` & `batchalign-0.7.1b9/batchalign/models/utterance/infer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/utterance/prep.py` & `batchalign-0.7.1b9/batchalign/models/utterance/prep.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/utterance/train.py` & `batchalign-0.7.1b9/batchalign/models/utterance/train.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/whisper/infer_asr.py` & `batchalign-0.7.1b9/batchalign/models/whisper/infer_asr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/models/whisper/infer_fa.py` & `batchalign-0.7.1b9/batchalign/models/whisper/infer_fa.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/analysis/eval.py` & `batchalign-0.7.1b9/batchalign/pipelines/analysis/eval.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/asr/rev.py` & `batchalign-0.7.1b9/batchalign/pipelines/asr/rev.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/asr/utils.py` & `batchalign-0.7.1b9/batchalign/pipelines/asr/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/asr/whisper.py` & `batchalign-0.7.1b9/batchalign/pipelines/asr/whisper.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/asr/whisperx.py` & `batchalign-0.7.1b9/batchalign/pipelines/asr/whisperx.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/base.py` & `batchalign-0.7.1b9/batchalign/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/cleanup/disfluencies.py` & `batchalign-0.7.1b9/batchalign/pipelines/cleanup/disfluencies.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/cleanup/parse_support.py` & `batchalign-0.7.1b9/batchalign/pipelines/cleanup/parse_support.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/cleanup/retrace.py` & `batchalign-0.7.1b9/batchalign/pipelines/cleanup/retrace.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/dispatch.py` & `batchalign-0.7.1b9/batchalign/pipelines/dispatch.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/fa/whisper_fa.py` & `batchalign-0.7.1b9/batchalign/pipelines/fa/whisper_fa.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/morphosyntax/fr/case.py` & `batchalign-0.7.1b9/batchalign/pipelines/morphosyntax/fr/case.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/morphosyntax/ud.py` & `batchalign-0.7.1b9/batchalign/pipelines/morphosyntax/ud.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/pipeline.py` & `batchalign-0.7.1b9/batchalign/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/speaker/nemo_speaker.py` & `batchalign-0.7.1b9/batchalign/pipelines/speaker/nemo_speaker.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/utr/rev_utr.py` & `batchalign-0.7.1b9/batchalign/pipelines/utr/rev_utr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/utr/utils.py` & `batchalign-0.7.1b9/batchalign/pipelines/utr/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/utr/whisper_utr.py` & `batchalign-0.7.1b9/batchalign/pipelines/utr/whisper_utr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/pipelines/utterance/ud_utterance.py` & `batchalign-0.7.1b9/batchalign/pipelines/utterance/ud_utterance.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/conftest.py` & `batchalign-0.7.1b9/batchalign/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_file.py` & `batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_generator.py` & `batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_lexer.py` & `batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_lexer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_parser.py` & `batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/formats/chat/test_chat_utils.py` & `batchalign-0.7.1b9/batchalign/tests/formats/chat/test_chat_utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/formats/textgrid/test_textgrid.py` & `batchalign-0.7.1b9/batchalign/tests/formats/textgrid/test_textgrid.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/pipelines/analysis/test_eval.py` & `batchalign-0.7.1b9/batchalign/tests/pipelines/analysis/test_eval.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/pipelines/asr/test_asr_pipeline.py` & `batchalign-0.7.1b9/batchalign/tests/pipelines/asr/test_asr_pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/pipelines/asr/test_asr_utils.py` & `batchalign-0.7.1b9/batchalign/tests/pipelines/asr/test_asr_utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/pipelines/cleanup/test_disfluency.py` & `batchalign-0.7.1b9/batchalign/tests/pipelines/cleanup/test_disfluency.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/pipelines/cleanup/test_parse_support.py` & `batchalign-0.7.1b9/batchalign/tests/pipelines/cleanup/test_parse_support.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/pipelines/fixures.py` & `batchalign-0.7.1b9/batchalign/tests/pipelines/fixures.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/pipelines/test_pipeline.py` & `batchalign-0.7.1b9/batchalign/tests/pipelines/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/pipelines/test_pipeline_models.py` & `batchalign-0.7.1b9/batchalign/tests/pipelines/test_pipeline_models.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/tests/test_document.py` & `batchalign-0.7.1b9/batchalign/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/utils/config.py` & `batchalign-0.7.1b9/batchalign/utils/config.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/utils/dp.py` & `batchalign-0.7.1b9/batchalign/utils/dp.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign/utils/utils.py` & `batchalign-0.7.1b9/batchalign/utils/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign.egg-info/PKG-INFO` & `batchalign-0.7.1b9/batchalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchalign
-Version: 0.7.1b8
+Version: 0.7.1b9
 Summary: Python Speech Language Sample Analysis
 Author: Brian MacWhinney, Houjun Liu
 Author-email: macw@cmu.edu, houjun@cmu.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `batchalign-0.7.1b8/batchalign.egg-info/SOURCES.txt` & `batchalign-0.7.1b9/batchalign.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/batchalign.egg-info/requires.txt` & `batchalign-0.7.1b9/batchalign.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.1b8/setup.py` & `batchalign-0.7.1b9/setup.py`

 * *Files identical despite different names*


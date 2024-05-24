# Comparing `tmp/ochat-3.5.2.tar.gz` & `tmp/ochat-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ochat-3.5.2.tar", last modified: Sat Mar  9 17:38:01 2024, max compression
+gzip compressed data, was "ochat-3.6.0.tar", last modified: Fri May 24 08:52:58 2024, max compression
```

## Comparing `ochat-3.5.2.tar` & `ochat-3.6.0.tar`

### file list

```diff
@@ -1,202 +1,208 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.620326 ochat-3.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.452325 ochat-3.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.456326 ochat-3.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-09 17:37:54.000000 ochat-3.5.2/.github/workflows/pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-09 17:37:54.000000 ochat-3.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-09 17:37:54.000000 ochat-3.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-03-09 17:38:01.620326 ochat-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23527 2024-03-09 17:37:54.000000 ochat-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-09 17:37:54.000000 ochat-3.5.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.460326 ochat-3.5.2/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   568121 2024-03-09 17:37:54.000000 ochat-3.5.2/assets/embeddings.svg
--rw-r--r--   0 runner    (1001) docker     (127)    68349 2024-03-09 17:37:54.000000 ochat-3.5.2/assets/logo_new.png
--rw-r--r--   0 runner    (1001) docker     (127)   464195 2024-03-09 17:37:54.000000 ochat-3.5.2/assets/openchat-bench-0106.png
--rw-r--r--   0 runner    (1001) docker     (127)   238819 2024-03-09 17:37:54.000000 ochat-3.5.2/assets/openchat.png
--rw-r--r--   0 runner    (1001) docker     (127)   208032 2024-03-09 17:37:54.000000 ochat-3.5.2/assets/openchat_grok.png
--rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-03-09 17:37:54.000000 ochat-3.5.2/assets/vicuna_gpt35.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-03-09 17:37:54.000000 ochat-3.5.2/assets/vicuna_gpt4.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.460326 ochat-3.5.2/ochat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.460326 ochat-3.5.2/ochat/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/config/conversation_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/config/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.460326 ochat-3.5.2/ochat/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/data/generate_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.460326 ochat-3.5.2/ochat/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/conv_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/convert_to_evalplus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.456326 ochat-3.5.2/ochat/evaluation/eval_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.452325 ochat-3.5.2/ochat/evaluation/eval_data/coding/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.460326 ochat-3.5.2/ochat/evaluation/eval_data/coding/humaneval/
--rw-r--r--   0 runner    (1001) docker     (127)  7927325 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/coding/humaneval/humaneval.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.452325 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.500326 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/
--rw-r--r--   0 runner    (1001) docker     (127)   491290 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   902939 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   384612 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1013894 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   687182 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1293180 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1341960 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   855574 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   816845 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   863272 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   770081 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   618185 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   638443 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   616281 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   413258 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   441275 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   725193 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   984109 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1870311 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   614065 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   251485 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   942794 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   852090 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   900774 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   807604 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   809832 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   669168 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.500326 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/gsm8k/
--rw-r--r--   0 runner    (1001) docker     (127) 11708109 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.592326 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/
--rw-r--r--   0 runner    (1001) docker     (127)   316921 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/abstract_algebra.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   625753 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/anatomy.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   682238 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/astronomy.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   460360 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/business_ethics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   733122 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/clinical_knowledge.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   712904 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_biology.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   305429 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_chemistry.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   654624 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_computer_science.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   399747 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_mathematics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   779094 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_medicine.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   361549 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_physics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   289993 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/computer_security.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   608886 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/conceptual_physics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   598834 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/econometrics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   388182 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/electrical_engineering.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1212397 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/elementary_mathematics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   608570 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/formal_logic.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   262815 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/global_facts.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1415403 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_biology.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   830314 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_chemistry.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   581758 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_computer_science.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  2491294 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_european_history.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   593280 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_geography.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   684510 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_government_and_politics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1194068 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_macroeconomics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   793994 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_mathematics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   771768 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_microeconomics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   495673 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_physics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  2149295 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_psychology.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1057755 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_statistics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  2458669 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_us_history.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1903525 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_world_history.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   485306 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/human_aging.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   352783 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/human_sexuality.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   552608 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/international_law.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   394984 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/jurisprudence.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   591362 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/logical_fallacies.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   542905 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/machine_learning.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   266364 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/management.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   765602 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/marketing.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   289653 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/medical_genetics.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1688159 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/miscellaneous.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1385332 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/moral_disputes.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  3330079 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/moral_scenarios.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1191226 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/nutrition.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   764153 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/philosophy.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1113452 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/prehistory.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1136228 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_accounting.jsonl
--rw-r--r--   0 runner    (1001) docker     (127) 14678643 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_law.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1694792 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_medicine.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  2468648 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_psychology.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   341069 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/public_relations.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1854554 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/security_studies.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   701727 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/sociology.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   324619 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/us_foreign_policy.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   408827 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/virology.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   351627 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/world_religions.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.456326 ochat-3.5.2/ochat/evaluation/eval_data/zs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.600326 ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/
--rw-r--r--   0 runner    (1001) docker     (127)    92097 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   638524 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   235210 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   626756 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)  1003390 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   103531 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   970033 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   102321 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.608326 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/
--rw-r--r--   0 runner    (1001) docker     (127)    54425 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   227316 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    89913 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   115064 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   182364 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   113342 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    73824 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   201521 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   247838 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   155266 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    84517 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    99515 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    98794 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   161261 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    91553 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   326806 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    62891 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    92422 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   184818 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   227141 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   276090 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)   184755 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    92710 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.608326 ochat-3.5.2/ochat/evaluation/eval_data/zs/math/
--rw-r--r--   0 runner    (1001) docker     (127)  6417549 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/math/MATH.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.612326 ochat-3.5.2/ochat/evaluation/eval_data/zs/truthfulqa_orca/
--rw-r--r--   0 runner    (1001) docker     (127)   265442 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.616326 ochat-3.5.2/ochat/evaluation/grading/
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/grading/math_grader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/grading/math_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/match_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/run_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/evaluation/view_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.616326 ochat-3.5.2/ochat/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/experimental/generate_dataset_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    62488 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/experimental/sharegpt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/experimental/test_multipack_dataloader.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/experimental/text_length.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/experimental/train_alpaca.py
--rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/experimental/verify_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    21113 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/experimental/verify_dataset_orca.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.616326 ochat-3.5.2/ochat/models/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/models/unpadded_gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/models/unpadded_llama.py
--rw-r--r--   0 runner    (1001) docker     (127)    16349 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/models/unpadded_mistral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.616326 ochat-3.5.2/ochat/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/scripts/hf_add_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/scripts/modify_eos_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.616326 ochat-3.5.2/ochat/serving/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/serving/async_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/serving/openai_api_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    14174 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/serving/openai_api_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.616326 ochat-3.5.2/ochat/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12718 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/tests/test_model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.616326 ochat-3.5.2/ochat/training_deepspeed/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/training_deepspeed/deepspeed_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/training_deepspeed/multipack_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/training_deepspeed/openchat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-03-09 17:37:54.000000 ochat-3.5.2/ochat/training_deepspeed/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 17:38:01.616326 ochat-3.5.2/ochat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-03-09 17:38:01.000000 ochat-3.5.2/ochat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-03-09 17:38:01.000000 ochat-3.5.2/ochat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 17:38:01.000000 ochat-3.5.2/ochat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-09 17:38:01.000000 ochat-3.5.2/ochat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-09 17:38:01.000000 ochat-3.5.2/ochat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-09 17:37:54.000000 ochat-3.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-09 17:37:54.000000 ochat-3.5.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 17:38:01.620326 ochat-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.284069 ochat-3.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.096068 ochat-3.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.100068 ochat-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-24 08:52:48.000000 ochat-3.6.0/.github/workflows/pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-24 08:52:48.000000 ochat-3.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-24 08:52:48.000000 ochat-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21382 2024-05-24 08:52:58.284069 ochat-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-05-24 08:52:48.000000 ochat-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-24 08:52:48.000000 ochat-3.6.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.104068 ochat-3.6.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    24053 2024-05-24 08:52:48.000000 ochat-3.6.0/assets/benchmarks-openchat-3.6-20240522.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   568121 2024-05-24 08:52:48.000000 ochat-3.6.0/assets/embeddings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    68349 2024-05-24 08:52:48.000000 ochat-3.6.0/assets/logo_new.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79934 2024-05-24 08:52:48.000000 ochat-3.6.0/assets/openchat-3.6-20240522.png
+-rw-r--r--   0 runner    (1001) docker     (127)   464195 2024-05-24 08:52:48.000000 ochat-3.6.0/assets/openchat-bench-0106.png
+-rw-r--r--   0 runner    (1001) docker     (127)   238819 2024-05-24 08:52:48.000000 ochat-3.6.0/assets/openchat.png
+-rw-r--r--   0 runner    (1001) docker     (127)   208032 2024-05-24 08:52:48.000000 ochat-3.6.0/assets/openchat_grok.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-05-24 08:52:48.000000 ochat-3.6.0/assets/vicuna_gpt35.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-05-24 08:52:48.000000 ochat-3.6.0/assets/vicuna_gpt4.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.104068 ochat-3.6.0/ochat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.104068 ochat-3.6.0/ochat/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/config/conversation_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/config/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.104068 ochat-3.6.0/ochat/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/data/generate_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.104068 ochat-3.6.0/ochat/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/conv_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/convert_to_evalplus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.096068 ochat-3.6.0/ochat/evaluation/eval_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.096068 ochat-3.6.0/ochat/evaluation/eval_data/coding/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.104068 ochat-3.6.0/ochat/evaluation/eval_data/coding/humaneval/
+-rw-r--r--   0 runner    (1001) docker     (127)  7927325 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/coding/humaneval/humaneval.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.096068 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.144068 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/
+-rw-r--r--   0 runner    (1001) docker     (127)   491290 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   902939 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   384612 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1013894 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   687182 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1293180 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1341960 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   855574 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   816845 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   863272 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   770081 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   618185 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   638443 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   616281 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   413258 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   441275 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   725193 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   984109 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1870311 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   614065 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   251485 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   942794 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   852090 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   900774 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   807604 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   809832 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   669168 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.148068 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/gsm8k/
+-rw-r--r--   0 runner    (1001) docker     (127) 11708109 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.256069 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/
+-rw-r--r--   0 runner    (1001) docker     (127)   316921 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/abstract_algebra.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   625753 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/anatomy.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   682238 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/astronomy.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   460360 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/business_ethics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   733122 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/clinical_knowledge.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   712904 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_biology.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   305429 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_chemistry.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   654624 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_computer_science.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   399747 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_mathematics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   779094 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_medicine.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   361549 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_physics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   289993 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/computer_security.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   608886 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/conceptual_physics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   598834 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/econometrics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   388182 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/electrical_engineering.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1212397 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/elementary_mathematics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   608570 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/formal_logic.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   262815 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/global_facts.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1415403 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_biology.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   830314 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_chemistry.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   581758 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_computer_science.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  2491294 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_european_history.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   593280 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_geography.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   684510 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_government_and_politics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1194068 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_macroeconomics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   793994 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_mathematics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   771768 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_microeconomics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   495673 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_physics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  2149295 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_psychology.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1057755 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_statistics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  2458669 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_us_history.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1903525 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_world_history.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   485306 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/human_aging.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   352783 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/human_sexuality.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   552608 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/international_law.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   394984 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/jurisprudence.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   591362 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/logical_fallacies.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   542905 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/machine_learning.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   266364 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/management.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   765602 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/marketing.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   289653 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/medical_genetics.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1688159 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/miscellaneous.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1385332 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/moral_disputes.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  3330079 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/moral_scenarios.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1191226 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/nutrition.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   764153 2024-05-24 08:52:48.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/philosophy.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1113452 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/prehistory.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1136228 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_accounting.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127) 14678643 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_law.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1694792 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_medicine.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  2468648 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_psychology.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   341069 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/public_relations.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1854554 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/security_studies.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   701727 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/sociology.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   324619 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/us_foreign_policy.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   408827 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/virology.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   351627 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/world_religions.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.096068 ochat-3.6.0/ochat/evaluation/eval_data/zs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.264069 ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/
+-rw-r--r--   0 runner    (1001) docker     (127)    92097 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   638524 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   235210 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   626756 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)  1003390 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   103531 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   970033 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   102321 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.272069 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/
+-rw-r--r--   0 runner    (1001) docker     (127)    54425 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   227316 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    89913 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   115064 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   182364 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   113342 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    73824 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   201521 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   247838 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   155266 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    84517 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    99515 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    98794 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   161261 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    91553 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   326806 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    62891 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    92422 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   184818 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   227141 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   276090 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)   184755 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    92710 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.272069 ochat-3.6.0/ochat/evaluation/eval_data/zs/gpqa/
+-rw-r--r--   0 runner    (1001) docker     (127)   166487 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/gpqa/diamond.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.272069 ochat-3.6.0/ochat/evaluation/eval_data/zs/math/
+-rw-r--r--   0 runner    (1001) docker     (127)  6417549 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/math/MATH.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.280069 ochat-3.6.0/ochat/evaluation/eval_data/zs/truthfulqa_orca/
+-rw-r--r--   0 runner    (1001) docker     (127)   265442 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.280069 ochat-3.6.0/ochat/evaluation/grading/
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/grading/math_grader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/grading/math_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/match_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/run_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/evaluation/view_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.284069 ochat-3.6.0/ochat/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/experimental/generate_dataset_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62488 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/experimental/sharegpt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/experimental/test_multipack_dataloader.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/experimental/text_length.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/experimental/train_alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/experimental/verify_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21113 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/experimental/verify_dataset_orca.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.284069 ochat-3.6.0/ochat/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/models/unpadded_gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/models/unpadded_llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16349 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/models/unpadded_mistral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.284069 ochat-3.6.0/ochat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/scripts/hf_add_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/scripts/init_special_embedding_llama3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/scripts/modify_eos_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.284069 ochat-3.6.0/ochat/serving/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/serving/async_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/serving/openai_api_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14174 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/serving/openai_api_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.284069 ochat-3.6.0/ochat/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20012 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/tests/test_model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.284069 ochat-3.6.0/ochat/training_deepspeed/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/training_deepspeed/deepspeed_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/training_deepspeed/hf_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/training_deepspeed/multipack_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/training_deepspeed/openchat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-05-24 08:52:49.000000 ochat-3.6.0/ochat/training_deepspeed/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:52:58.284069 ochat-3.6.0/ochat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21382 2024-05-24 08:52:57.000000 ochat-3.6.0/ochat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-24 08:52:58.000000 ochat-3.6.0/ochat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:52:57.000000 ochat-3.6.0/ochat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-24 08:52:57.000000 ochat-3.6.0/ochat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 08:52:57.000000 ochat-3.6.0/ochat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-24 08:52:49.000000 ochat-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 08:52:49.000000 ochat-3.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:52:58.284069 ochat-3.6.0/setup.cfg
```

### Comparing `ochat-3.5.2/.gitignore` & `ochat-3.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/LICENSE` & `ochat-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/PKG-INFO` & `ochat-3.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 Metadata-Version: 2.1
 Name: ochat
-Version: 3.5.2
+Version: 3.6.0
 Summary: An efficient framework for training and serving top-tier, open-source conversational LLMs.
 Project-URL: Homepage, https://github.com/imoneoi/openchat
 Project-URL: Bug Tracker, https://github.com/imoneoi/openchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4
 Requires-Dist: markdownify
-Requires-Dist: openai
+Requires-Dist: pylatexenc
+Requires-Dist: openai>=1
 Requires-Dist: tenacity
 Requires-Dist: tiktoken
 Requires-Dist: tqdm
 Requires-Dist: wandb
 Requires-Dist: numba
 Requires-Dist: datasets
 Requires-Dist: orjson
 Requires-Dist: torch
+Requires-Dist: packaging
+Requires-Dist: ninja
+Requires-Dist: flash-attn
 Requires-Dist: ray
 Requires-Dist: sentencepiece
-Requires-Dist: transformers>=4.38.2
+Requires-Dist: transformers>=4.40.1
 Requires-Dist: accelerate
 Requires-Dist: protobuf
 Requires-Dist: fastapi
 Requires-Dist: pydantic
 Requires-Dist: shortuuid
 Requires-Dist: uvicorn
-Requires-Dist: vllm>=0.3.3
+Requires-Dist: vllm>=0.4.0
 Requires-Dist: pytest
 
 # OpenChat: Advancing Open-source Language Models with Mixed-Quality Data
 
 <div align="center">
   <img src="assets/logo_new.png" style="width: 65%">
 </div>
 
 <p align="center">
   <a href="https://openchat.team">💻Online Demo</a> |
   <a href="https://huggingface.co/openchat">🤗Huggingface</a> |
   <a href="https://arxiv.org/pdf/2309.11235.pdf">📃Paper</a> |
   <a href="https://discord.gg/pQjnXvNKHY">💭Discord</a> 
-  <br><br>
-  <strong>🏆 The Overall Best Performing Open Source 7B Model 🏆</strong>
-  <br>
-  <strong>🤖 Outperforms ChatGPT (March) and Grok-1 🤖</strong>
-  <br>
 </p>
 
-<div align="center">
-  <img src="https://raw.githubusercontent.com/imoneoi/openchat/master/assets/openchat-bench-0106.png" style="width: 95%;">
-</div>
-
 - OpenChat is an innovative library of **open-source language models**, fine-tuned with [**C-RLFT**](https://arxiv.org/pdf/2309.11235.pdf) - a strategy inspired by offline reinforcement learning.
 - Our models learn from mixed-quality data without preference labels, delivering exceptional performance on par with `ChatGPT`, even with a `7B` model which can be run on a **consumer GPU (e.g. RTX 3090)**.
 - Despite our simple approach, we are committed to developing a high-performance, commercially viable, open-source large language model, and we continue to make significant strides toward this vision.
 
 [![DOI](https://zenodo.org/badge/645397533.svg)](https://zenodo.org/badge/latestdoi/645397533)
 
 # ✨ News
 
+ - [2024/05/22] We released the Llama-3 based version [OpenChat 3.6 20240522](https://huggingface.co/openchat/openchat-3.6-8b-20240522), outperforming official Llama 3 8B Instruct and open-source finetunes/merges.
+
 - [2024/01/06] We released the second update, [OpenChat 3.5 0106](openchat/openchat-3.5-0106), further improved coding and overall performance 🏆.
 
 - [2023/12/10] We released the first update, [OpenChat 3.5 1210](openchat/openchat-3.5-1210), improved coding by 15 points 🚀.
 
 - [2023/11/01] We released the [OpenChat-3.5-7B](https://huggingface.co/openchat/openchat_3.5) model, surpassing ChatGPT on various benchmarks 🔥.
 
 - [2023/09/21] We released our paper [OpenChat: Advancing Open-source Language Models with Mixed-Quality Data](https://arxiv.org/pdf/2309.11235.pdf).
@@ -80,21 +77,39 @@
 - [2023/07/30] We are thrilled to introduce the [OpenChat V3 model series](#models), based on Llama 2, and now available for free for commercial use!
 
 - [2023/07/07] We released the [OpenChat V2 model series](#legacy-models).
 
 - [2023/07/01] We released the [OpenChat V1 model series](#legacy-models).
 </details>
 
-# 🏷️ Benchmarks
+# 🏷️ Benchmarks - OpenChat 3.6
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/imoneoi/openchat/master/assets/benchmarks-openchat-3.6-20240522.svg" style="width: 95%;">
+</div>
+
+
+<details>
+  <summary>Reproducing benchmarks</summary>
+
+Note: Please run the following commands at the base directory of this repository.
+
+```bash
+python -m ochat.evaluation.run_eval --condition "GPT4 Correct" --model openchat/openchat-3.6-8b-20240522 --eval_sets fs_cothub/mmlu fs_cothub/gsm8k fs_cothub/math
+python -m ochat.evaluation.run_eval --condition "GPT4" --model openchat/openchat-3.6-8b-20240522 --eval_sets zs/gpqa
+```
+
+HumanEval is run using the official [EvalPlus repository](https://github.com/evalplus/evalplus).
+</details>
+
+# 🏷️ Benchmarks - OpenChat 3.5
 
 | Model                 | # Params | Average  | MT-Bench     | HumanEval       | BBH MC   | AGIEval  | TruthfulQA    | MMLU         | GSM8K        | BBH CoT     |
 |-----------------------|----------|----------|--------------|-----------------|----------|----------|---------------|--------------|--------------|-------------|
 | **OpenChat-3.5-0106** | **7B**   | **64.5** | 7.8          | **71.3**        | **51.5** | **49.1** | 61.0          | 65.8         | **77.4**     | 62.2        |
-| OpenChat-3.5-1210     | **7B**   | 63.8     | 7.76         | 68.9            | 49.5     | 48.0     | **61.8**      | 65.3         | 77.3         | 61.8        |
-| OpenChat-3.5          | **7B**   | 61.6     | 7.81         | 55.5            | 47.6     | 47.4     | 59.1          | 64.3         | 77.3         | 63.5        |
 | ChatGPT (March)*      | ???B     | 61.5     | **7.94**     | 48.1            | 47.6     | 47.1     | 57.7          | **67.3**     | 74.9         | **70.1**    |
 |                       |          |          |              |                 |          |          |               |              |              |             |
 | OpenHermes 2.5        | 7B       | 59.3     | 7.54         | 48.2            | 49.4     | 46.5     | 57.5          | 63.8         | 73.5         | 59.9        |
 | OpenOrca Mistral      | 7B       | 52.7     | 6.86         | 38.4            | 49.4     | 42.9     | 45.9          | 59.3         | 59.1         | 58.1        |
 | Zephyr-β^             | 7B       | 34.6     | 7.34         | 22.0            | 40.6     | 39.0     | 40.8          | 39.8         | 5.1          | 16.0        |
 | Mistral               | 7B       | -        | 6.84         | 30.5            | 39.0     | 38.0     | -             | 60.1         | 52.2         | -           |
 | Open-source SOTA**    | 13B-70B  | 61.4     | 7.71         | 73.2            | 49.7     | 41.7     | 62.3          | 63.7         | 82.3         | 41.4        |
@@ -156,16 +171,14 @@
 ## 🎇 Comparison with [X.AI Grok](https://x.ai/)
 
 🔥 OpenChat-3.5-0106 (7B) now outperforms Grok-0 (33B) on **all 4 benchmarks** and Grok-1 (???B) on average and **3/4 benchmarks**.
 
 |                       | License     | # Param | Average  | MMLU   | HumanEval | MATH     | GSM8k    |
 |-----------------------|-------------|---------|----------|--------|-----------|----------|----------|
 | **OpenChat-3.5-0106** | Apache-2.0  | **7B**  | **61.0** | 65.8   | **71.3**  | **29.3** | **77.4** |
-| OpenChat-3.5-1210     | Apache-2.0  | **7B**  | 60.1     | 65.3   | 68.9      | 28.9     | 77.3     |
-| OpenChat-3.5          | Apache-2.0  | **7B**  | 56.4     | 64.3   | 55.5      | 28.6     | 77.3     |
 | Grok-0                | Proprietary | 33B     | 44.5     | 65.7   | 39.7      | 15.7     | 56.8     |
 | Grok-1                | Proprietary | ???B    | 55.8     | **73** | 63.2      | 23.9     | 62.9     |
 
 # ⬇️ Installation
 > [!NOTE]
 > Need [`pytorch`](https://pytorch.org/get-started/locally/#start-locally) to run OpenChat
 
@@ -303,23 +316,22 @@
 
 # <a id="training"></a> 🛠️ Training
 
 The OpenChat training system utilizes padding-free training and the [Multipack Sampler](https://github.com/imoneoi/multipack_sampler), achieving a **3~10x** speedup compared to the conventional padded training.
 
 ## Choose a base model
 
-OpenChat supports Llama 2 and Mistral models. Please first choose a base model to fit your needs. Each base model has a corresponding weight repo, model type, and recommended batch size as listed below, they should be filled into `BASE_REPO`, `MODEL_TYPE`, and `BATCH_SIZE` in the following instructions.
+OpenChat supports Llama 3 and Mistral models. Please first choose a base model to fit your needs. Each base model has a corresponding weight repo, model type, and recommended batch size as listed below, they should be filled into `BASE_REPO`, `MODEL_TYPE`, and `BATCH_SIZE` in the following instructions.
 
-| Base Model | Size | Weights (with EOT token)          | Model Type              | Recommended Batch Size per GPU (8xA100 80GB) |
-|------------|------|-----------------------------------|-------------------------|--------------------------------------|
-| Mistral    | 7B   | `imone/Mistral_7B_with_EOT_token` | `openchat_v3.2_mistral` | 77824                                |
-| Llama 2    | 7B   | `imone/LLaMA2_7B_with_EOT_token`  | `openchat_v3.2`         | 77824                                |
-| Llama 2    | 13B  | `imone/Llama2_13B_with_EOT_token` | `openchat_v3.2`         | 36864                                |
+| Base Model | Size | Weights (with EOT token)                   | Model Type              | Recommended Batch Size per GPU (8xA100 80GB) |
+|------------|------|--------------------------------------------|-------------------------|----------------------------------------------|
+| Llama 3    | 8B   | `imone/Llama-3-8B-fixed-special-embedding` | `openchat_3.6`          | 40960                                        |
+| Mistral    | 7B   | `imone/Mistral_7B_with_EOT_token`          | `openchat_v3.2_mistral` | 77824                                        |
 
-Note: The OpenChat conversation template requires an `<|end_of_turn|>` special token. The base model specified must include this token. Our provided weights are the original base weights with this token added. If you want to add them manually, use the `convert_llama_weights_to_hf_add_tokens.py` or `mistral_add_tokens.py` in the `scripts` directory.
+Note: The OpenChat conversation template requires `<|eot_id|>, <|start_header_id|>, <|end_header_id|>` (Llama 3) `<|end_of_turn|>` (Mistral) special tokens. The base model specified must include these tokens with initialized embeddings. Our provided weights are the original base weights with this token added and embeddings initialized. If you want to add them manually, use the `init_special_embedding_llama3.py` or `mistral_add_tokens.py` in the `scripts` directory.
 
 ## Installing DeepSpeed and Flash Attention
 
 First, ensure that the CUDA `nvcc` compiler is available in your environment. If it is not, install the CUDA toolkit that matches the version used by PyTorch.
 
 Next, install building dependencies:
 
@@ -420,57 +432,47 @@
 OpenChat may sometimes generate information that does not exist or is not accurate, also known as "hallucination". Users should be aware of this possibility and verify any critical information obtained the model.
 
 ## Safety
 OpenChat may sometimes generate harmful, hate speech, biased responses, or answer unsafe questions. It's crucial to apply additional AI safety measures in use cases that require safe and moderated responses.
 
 # License
 
-Our OpenChat 3.5 `code` and `models` are distributed under the **Apache License 2.0**.
-
-# <a id="models"></a> Models
-
-| Model        | Size | Context | Weights                                                     | Serving                                                                                                     |
-|--------------|------|---------|-------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
-| OpenChat 3.5 0106 | 7B   | 8192    | [Huggingface](https://huggingface.co/openchat/openchat-3.5-0106) | `python -m ochat.serving.openai_api_server --model openchat/openchat-3.5-0106 --engine-use-ray --worker-use-ray` |
-| OpenChat 3.5 1210 | 7B   | 8192    | [Huggingface](https://huggingface.co/openchat/openchat-3.5-1210) | `python -m ochat.serving.openai_api_server --model openchat/openchat-3.5-1210 --engine-use-ray --worker-use-ray` |
-| OpenChat 3.5 | 7B   | 8192    | [Huggingface](https://huggingface.co/openchat/openchat_3.5) | `python -m ochat.serving.openai_api_server --model openchat/openchat_3.5 --engine-use-ray --worker-use-ray` |
-
-## <a id="legacy-models"></a> Legacy Models
-
-The following models are older versions of OpenChat and have inferior performance compared to the latest version. They will be deprecated in the next release. Please note that OpenChat V1 and V2 series are now deprecated, [please install 3.1.x for using V1 and V2 models](https://github.com/imoneoi/openchat/tree/83a683c775c77867cc45937fafdf48e8dcb68daa)
-
-To run the models on multiple GPUs with smaller VRAM, you can enable tensor parallelization, for example, using the `--tensor-parallel-size 2` flag.
-
-| Model        | Size | Context | Weights                                                      | Serving                                                                                                      |
-|--------------|------|---------|--------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|
-| OpenChat 3.2 SUPER | 13B  | 4096    | [Huggingface](https://huggingface.co/openchat/openchat_v3.2_super) | `python -m ochat.serving.openai_api_server --model openchat/openchat_v3.2_super --engine-use-ray --worker-use-ray` |
+Code is distributed under the **Apache License 2.0**.
 
 # Citation
 
 ```
 @article{wang2023openchat,
   title={OpenChat: Advancing Open-source Language Models with Mixed-Quality Data},
   author={Wang, Guan and Cheng, Sijie and Zhan, Xianyuan and Li, Xiangang and Song, Sen and Liu, Yang},
   journal={arXiv preprint arXiv:2309.11235},
   year={2023}
 }
 ```
 
 # 💌Contact
 
-We are a student team at Tsinghua University, working on OpenChat, a project that requires additional computing power or LLMs API keys for further development. If you are interested in our project and would like to offer support, please feel free to reach out to us:
-
-**Project Leader:**
+**Project Lead:**
 - Guan Wang [imonenext at gmail dot com]
-- [Sijie Cheng](https://adacheng.github.io/) [csj23 at mails dot tsinghua dot edu dot cn]
+- [Alpay Ariyak](https://github.com/alpayariyak) [aariyak at wpi dot edu]
 
 **Main Contributors:**
-- [Xianyuan Zhan](https://scholar.google.com.hk/citations?user=pDMnGloAAAAJ&hl=zh-CN) (Tsinghua University): Provided invaluable advice on paper writing.
-- [Alpay Ariyak](https://github.com/alpayariyak): Responsible for data collection, documentation, model cards and PR for `openchat-3.5-1210`, `openchat-3.5-0106`.
-- LDJ: Tasked with partial data collection for `openchat-3.5`.
+- [Xianyuan Zhan](https://scholar.google.com.hk/citations?user=pDMnGloAAAAJ) (Tsinghua University)
+- Qiying Yu (Tsinghua University)
+- Changling Liu (GPT Desk Pte. Ltd.)
+- LDJ
+- AutoMeta (Alignment Lab AI)
 
 **Sponsors:**
-- [Sen Song](https://scholar.google.com/citations?user=cYgtRP4AAAAJ&hl=en) (Tsinghua University), [Yang Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University), [01.AI Company](https://www.lingyiwanwu.com/en), [RunPod](https://www.runpod.io/), Changling Liu (GPT Desk Pte. Ltd.), Qiying Yu (Tsinghua University), AutoMeta (Alignment Lab AI).
+- [Sen Song](https://scholar.google.com/citations?user=cYgtRP4AAAAJ) (Tsinghua University)
+- [Yang Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University)
+- [01.AI Company](https://www.lingyiwanwu.com/en)
+- [RunPod](https://www.runpod.io/)
 
 **Special Thanks:**
-- We express our profound gratitude to Alignment Lab AI, Nous Research, and Pygmalion AI for their significant contributions to data collection and model training. We also extend our special thanks to Xiangang Li, Baochang Ma, and Hao Wan from 01.AI company for their generous provision of resources. We also thank Jianxiong Li and Peng Li at Tsinghua University for their insightful discussions that have enriched our work.
-- We acknowledge and thank the developers behind these projects: [Mistral](https://mistral.ai/), [Chain-of-Thought Hub](https://github.com/FranxYao/chain-of-thought-hub), [Llama 2](https://ai.meta.com/llama/), [Self-Instruct](https://arxiv.org/abs/2212.10560), [FastChat (Vicuna)](https://github.com/lm-sys/FastChat), [Alpaca](https://github.com/tatsu-lab/stanford_alpaca.git), and [StarCoder](https://github.com/bigcode-project/starcoder). Their work has been instrumental in driving our research forward.
+ - [Mistral](https://mistral.ai/)
+ - [Chain-of-Thought Hub](https://github.com/FranxYao/chain-of-thought-hub)
+ - [Llama 2](https://ai.meta.com/llama/)
+ - [Self-Instruct](https://arxiv.org/abs/2212.10560)
+ - [FastChat (Vicuna)](https://github.com/lm-sys/FastChat)
+ - [Alpaca](https://github.com/tatsu-lab/stanford_alpaca.git)
+ - [StarCoder](https://github.com/bigcode-project/starcoder)
```

#### html2text {}

```diff
@@ -1,125 +1,129 @@
-Metadata-Version: 2.1 Name: ochat Version: 3.5.2 Summary: An efficient
+Metadata-Version: 2.1 Name: ochat Version: 3.6.0 Summary: An efficient
 framework for training and serving top-tier, open-source conversational LLMs.
 Project-URL: Homepage, https://github.com/imoneoi/openchat Project-URL: Bug
 Tracker, https://github.com/imoneoi/openchat/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
-Requires-Dist: openai Requires-Dist: tenacity Requires-Dist: tiktoken Requires-
-Dist: tqdm Requires-Dist: wandb Requires-Dist: numba Requires-Dist: datasets
-Requires-Dist: orjson Requires-Dist: torch Requires-Dist: ray Requires-Dist:
-sentencepiece Requires-Dist: transformers>=4.38.2 Requires-Dist: accelerate
-Requires-Dist: protobuf Requires-Dist: fastapi Requires-Dist: pydantic
-Requires-Dist: shortuuid Requires-Dist: uvicorn Requires-Dist: vllm>=0.3.3
-Requires-Dist: pytest # OpenChat: Advancing Open-source Language Models with
-Mixed-Quality Data
+Requires-Dist: pylatexenc Requires-Dist: openai>=1 Requires-Dist: tenacity
+Requires-Dist: tiktoken Requires-Dist: tqdm Requires-Dist: wandb Requires-Dist:
+numba Requires-Dist: datasets Requires-Dist: orjson Requires-Dist: torch
+Requires-Dist: packaging Requires-Dist: ninja Requires-Dist: flash-attn
+Requires-Dist: ray Requires-Dist: sentencepiece Requires-Dist:
+transformers>=4.40.1 Requires-Dist: accelerate Requires-Dist: protobuf
+Requires-Dist: fastapi Requires-Dist: pydantic Requires-Dist: shortuuid
+Requires-Dist: uvicorn Requires-Dist: vllm>=0.4.0 Requires-Dist: pytest #
+OpenChat: Advancing Open-source Language Models with Mixed-Quality Data
                              [assets/logo_new.png]
-         _ð___»_O_n_l_i_n_e_ _D_e_m_o | _ð__¤__H_u_g_g_i_n_g_f_a_c_e | _ð____P_a_p_e_r | _ð___­_D_i_s_c_o_r_d
-
-          ?ð??? TThhee OOvveerraallll BBeesstt PPeerrffoorrmmiinngg OOppeenn SSoouurrccee 77BB MMooddeell ?ð???
-               ?ð??¤? OOuuttppeerrffoorrmmss CChhaattGGPPTT ((MMaarrcchh)) aanndd GGrrookk--11 ?ð??¤?
-  [https://raw.githubusercontent.com/imoneoi/openchat/master/assets/openchat-
-                                bench-0106.png]
+          _ð___»_O_n_l_i_n_e_ _D_e_m_o | _ð__¤__H_u_g_g_i_n_g_f_a_c_e | _ð____P_a_p_e_r | _ð___­_D_i_s_c_o_r_d
 - OpenChat is an innovative library of **open-source language models**, fine-
 tuned with [**C-RLFT**](https://arxiv.org/pdf/2309.11235.pdf) - a strategy
 inspired by offline reinforcement learning. - Our models learn from mixed-
 quality data without preference labels, delivering exceptional performance on
 par with `ChatGPT`, even with a `7B` model which can be run on a **consumer GPU
 (e.g. RTX 3090)**. - Despite our simple approach, we are committed to
 developing a high-performance, commercially viable, open-source large language
 model, and we continue to make significant strides toward this vision. [![DOI]
 (https://zenodo.org/badge/645397533.svg)](https://zenodo.org/badge/latestdoi/
-645397533) # â¨ News - [2024/01/06] We released the second update, [OpenChat
-3.5 0106](openchat/openchat-3.5-0106), further improved coding and overall
+645397533) # â¨ News - [2024/05/22] We released the Llama-3 based version
+[OpenChat 3.6 20240522](https://huggingface.co/openchat/openchat-3.6-8b-
+20240522), outperforming official Llama 3 8B Instruct and open-source
+finetunes/merges. - [2024/01/06] We released the second update, [OpenChat 3.5
+0106](openchat/openchat-3.5-0106), further improved coding and overall
 performance ð. - [2023/12/10] We released the first update, [OpenChat 3.5
 1210](openchat/openchat-3.5-1210), improved coding by 15 points ð. - [2023/
 11/01] We released the [OpenChat-3.5-7B](https://huggingface.co/openchat/
 openchat_3.5) model, surpassing ChatGPT on various benchmarks ð¥. - [2023/09/
 21] We released our paper [OpenChat: Advancing Open-source Language Models with
 Mixed-Quality Data](https://arxiv.org/pdf/2309.11235.pdf). Read more - [2023/
 09/03] We released the [OpenChat V3.2 SUPER]([#models](https://huggingface.co/
 openchat/openchat_v3.2_super)) model. - [2023/08/04] We have launched an
 [Online Demo](https://openchat.team) featuring the latest version, OpenChat
 3.2. - [2023/07/30] We are thrilled to introduce the [OpenChat V3 model series]
 (#models), based on Llama 2, and now available for free for commercial use! -
 [2023/07/07] We released the [OpenChat V2 model series](#legacy-models). -
 [2023/07/01] We released the [OpenChat V1 model series](#legacy-models). #
-ð·ï¸ Benchmarks | Model | # Params | Average | MT-Bench | HumanEval | BBH MC
-| AGIEval | TruthfulQA | MMLU | GSM8K | BBH CoT | |-----------------------|----
-------|----------|--------------|-----------------|----------|----------|------
----------|--------------|--------------|-------------| | **OpenChat-3.5-0106**
-| **7B** | **64.5** | 7.8 | **71.3** | **51.5** | **49.1** | 61.0 | 65.8 |
-**77.4** | 62.2 | | OpenChat-3.5-1210 | **7B** | 63.8 | 7.76 | 68.9 | 49.5 |
-48.0 | **61.8** | 65.3 | 77.3 | 61.8 | | OpenChat-3.5 | **7B** | 61.6 | 7.81 |
-55.5 | 47.6 | 47.4 | 59.1 | 64.3 | 77.3 | 63.5 | | ChatGPT (March)* | ???B |
-61.5 | **7.94** | 48.1 | 47.6 | 47.1 | 57.7 | **67.3** | 74.9 | **70.1** | | |
-| | | | | | | | | | | OpenHermes 2.5 | 7B | 59.3 | 7.54 | 48.2 | 49.4 | 46.5 |
-57.5 | 63.8 | 73.5 | 59.9 | | OpenOrca Mistral | 7B | 52.7 | 6.86 | 38.4 | 49.4
-| 42.9 | 45.9 | 59.3 | 59.1 | 58.1 | | Zephyr-Î²^ | 7B | 34.6 | 7.34 | 22.0 |
-40.6 | 39.0 | 40.8 | 39.8 | 5.1 | 16.0 | | Mistral | 7B | - | 6.84 | 30.5 |
-39.0 | 38.0 | - | 60.1 | 52.2 | - | | Open-source SOTA** | 13B-70B | 61.4 |
-7.71 | 73.2 | 49.7 | 41.7 | 62.3 | 63.7 | 82.3 | 41.4 | | | | | WizardLM 70B |
-WizardCoder 34B | Orca 13B | Orca 13B | Platypus2 70B | WizardLM 70B | MetaMath
-70B | Flan-T5 11B | Evaluation details *: ChatGPT (March) results are from GPT-
-4 Technical Report, Chain-of-Thought Hub, and our evaluation. ^: Zephyr-Î²
-often fails to follow few-shot CoT instructions, likely because it was aligned
-with only chat data but not trained on few-shot data. **: Mistral and Open-
-source SOTA results are taken from reported results in instruction-tuned model
-papers and official repositories. All models are evaluated in chat mode (e.g.
-with the respective conversation template applied). All zero-shot benchmarks
-follow the same setting as in the AGIEval paper and Orca paper. CoT tasks use
-the same configuration as Chain-of-Thought Hub, HumanEval is evaluated with
-EvalPlus, and MT-bench is run using FastChat. To reproduce our results, follow
-the instructions below. Reproducing benchmarks Reasoning and Coding: Note:
-Please run the following commands at the base directory of this repository.
-```bash python -m ochat.evaluation.run_eval --condition "GPT4 Correct" --model
-openchat/openchat-3.5-0106 --eval_sets coding fs_cothub/bbh fs_cothub/mmlu zs/
-agieval zs/bbh_mc_orca zs/truthfulqa_orca python ochat/evaluation/
-view_results.py python ochat/evaluation/convert_to_evalplus.py ``` Then all
-humaneval code samples are placed in `ochat/evaluation/evalplus_codegen`. Use
-the following command to evaluate an individual code sample named
-`samples.jsonl` using Docker as a sandbox. ```bash docker run -v $(pwd):/app
-ganler/evalplus:latest --dataset humaneval --samples samples.jsonl ```
-Mathematical Reasoning: Note: Please run the following commands at the base
+ð·ï¸ Benchmarks - OpenChat 3.6
+ [https://raw.githubusercontent.com/imoneoi/openchat/master/assets/benchmarks-
+                          openchat-3.6-20240522.svg]
+Reproducing benchmarks Note: Please run the following commands at the base
 directory of this repository. ```bash python -m ochat.evaluation.run_eval --
-condition "Math Correct" --model openchat/openchat-3.5-0106 --eval_sets
-fs_cothub/gsm8k zs/math python ochat/evaluation/view_results.py ``` MT-Bench:
-Please first launch a local API server, then download FastChat and run the
-following commands. Note: Due to non-zero temperature and GPT-4 API changes
-over time, there might be variations in the results. ```bash cd fastchat/
-llm_judge python gen_api_answer.py --model openchat-3.5-0106 --max-tokens 4096
---parallel 128 --openai-api-base http://localhost:18888/v1 python
-gen_judgment.py --model-list openchat-3.5-0106 --parallel 8 --mode single ```
-## ð Comparison with [X.AI Grok](https://x.ai/) ð¥ OpenChat-3.5-0106 (7B)
-now outperforms Grok-0 (33B) on **all 4 benchmarks** and Grok-1 (???B) on
-average and **3/4 benchmarks**. | | License | # Param | Average | MMLU |
-HumanEval | MATH | GSM8k | |-----------------------|-------------|---------|---
--------|--------|-----------|----------|----------| | **OpenChat-3.5-0106** |
-Apache-2.0 | **7B** | **61.0** | 65.8 | **71.3** | **29.3** | **77.4** | |
-OpenChat-3.5-1210 | Apache-2.0 | **7B** | 60.1 | 65.3 | 68.9 | 28.9 | 77.3 | |
-OpenChat-3.5 | Apache-2.0 | **7B** | 56.4 | 64.3 | 55.5 | 28.6 | 77.3 | | Grok-
-0 | Proprietary | 33B | 44.5 | 65.7 | 39.7 | 15.7 | 56.8 | | Grok-1 |
-Proprietary | ???B | 55.8 | **73** | 63.2 | 23.9 | 62.9 | # â¬ï¸ Installation
-> [!NOTE] > Need [`pytorch`](https://pytorch.org/get-started/locally/#start-
-locally) to run OpenChat ## pip ```bash pip3 install ochat ``` > [!IMPORTANT] >
-If you are facing package compatibility issues with pip, try the conda method
-below or check [this issue](https://github.com/imoneoi/openchat/issues/41) ##
-conda ```bash conda create -y --name openchat python=3.11 conda activate
-openchat pip3 install ochat ``` ## Windows (WSL 1.x, Ubuntu-22.04) ```bash sudo
-apt update sudo apt install build-essential sudo apt install -y curl curl -
-o miniconda.sh https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-
-x86_64.sh bash miniconda.sh # Restart WSL terminal if the following conda
-command does not work conda create -y --name openchat python=3.11 conda
-activate openchat pip3 install ochat ``` ## From source Clone this repo and
-install openchat from source in editable mode ```bash git clone https://
-github.com/imoneoi/openchat cd openchat pip3 install --upgrade pip # enable PEP
-660 support pip3 install -e . # Editable mode, you can make changes in this
-cloned repo ``` # ð Deploying API server â¡ Our API server is ready for
-production use and compatible with the OpenAI API protocol. It is highly
+condition "GPT4 Correct" --model openchat/openchat-3.6-8b-20240522 --eval_sets
+fs_cothub/mmlu fs_cothub/gsm8k fs_cothub/math python -
+m ochat.evaluation.run_eval --condition "GPT4" --model openchat/openchat-3.6-
+8b-20240522 --eval_sets zs/gpqa ``` HumanEval is run using the official
+[EvalPlus repository](https://github.com/evalplus/evalplus). # ð·ï¸
+Benchmarks - OpenChat 3.5 | Model | # Params | Average | MT-Bench | HumanEval |
+BBH MC | AGIEval | TruthfulQA | MMLU | GSM8K | BBH CoT | |---------------------
+--|----------|----------|--------------|-----------------|----------|----------
+|---------------|--------------|--------------|-------------| | **OpenChat-3.5-
+0106** | **7B** | **64.5** | 7.8 | **71.3** | **51.5** | **49.1** | 61.0 | 65.8
+| **77.4** | 62.2 | | ChatGPT (March)* | ???B | 61.5 | **7.94** | 48.1 | 47.6 |
+47.1 | 57.7 | **67.3** | 74.9 | **70.1** | | | | | | | | | | | | | | OpenHermes
+2.5 | 7B | 59.3 | 7.54 | 48.2 | 49.4 | 46.5 | 57.5 | 63.8 | 73.5 | 59.9 | |
+OpenOrca Mistral | 7B | 52.7 | 6.86 | 38.4 | 49.4 | 42.9 | 45.9 | 59.3 | 59.1 |
+58.1 | | Zephyr-Î²^ | 7B | 34.6 | 7.34 | 22.0 | 40.6 | 39.0 | 40.8 | 39.8 | 5.1
+| 16.0 | | Mistral | 7B | - | 6.84 | 30.5 | 39.0 | 38.0 | - | 60.1 | 52.2 | - |
+| Open-source SOTA** | 13B-70B | 61.4 | 7.71 | 73.2 | 49.7 | 41.7 | 62.3 | 63.7
+| 82.3 | 41.4 | | | | | WizardLM 70B | WizardCoder 34B | Orca 13B | Orca 13B |
+Platypus2 70B | WizardLM 70B | MetaMath 70B | Flan-T5 11B | Evaluation details
+*: ChatGPT (March) results are from GPT-4 Technical Report, Chain-of-Thought
+Hub, and our evaluation. ^: Zephyr-Î² often fails to follow few-shot CoT
+instructions, likely because it was aligned with only chat data but not trained
+on few-shot data. **: Mistral and Open-source SOTA results are taken from
+reported results in instruction-tuned model papers and official repositories.
+All models are evaluated in chat mode (e.g. with the respective conversation
+template applied). All zero-shot benchmarks follow the same setting as in the
+AGIEval paper and Orca paper. CoT tasks use the same configuration as Chain-of-
+Thought Hub, HumanEval is evaluated with EvalPlus, and MT-bench is run using
+FastChat. To reproduce our results, follow the instructions below. Reproducing
+benchmarks Reasoning and Coding: Note: Please run the following commands at the
+base directory of this repository. ```bash python -m ochat.evaluation.run_eval
+--condition "GPT4 Correct" --model openchat/openchat-3.5-0106 --eval_sets
+coding fs_cothub/bbh fs_cothub/mmlu zs/agieval zs/bbh_mc_orca zs/
+truthfulqa_orca python ochat/evaluation/view_results.py python ochat/
+evaluation/convert_to_evalplus.py ``` Then all humaneval code samples are
+placed in `ochat/evaluation/evalplus_codegen`. Use the following command to
+evaluate an individual code sample named `samples.jsonl` using Docker as a
+sandbox. ```bash docker run -v $(pwd):/app ganler/evalplus:latest --dataset
+humaneval --samples samples.jsonl ``` Mathematical Reasoning: Note: Please run
+the following commands at the base directory of this repository. ```bash python
+-m ochat.evaluation.run_eval --condition "Math Correct" --model openchat/
+openchat-3.5-0106 --eval_sets fs_cothub/gsm8k zs/math python ochat/evaluation/
+view_results.py ``` MT-Bench: Please first launch a local API server, then
+download FastChat and run the following commands. Note: Due to non-zero
+temperature and GPT-4 API changes over time, there might be variations in the
+results. ```bash cd fastchat/llm_judge python gen_api_answer.py --model
+openchat-3.5-0106 --max-tokens 4096 --parallel 128 --openai-api-base http://
+localhost:18888/v1 python gen_judgment.py --model-list openchat-3.5-0106 --
+parallel 8 --mode single ``` ## ð Comparison with [X.AI Grok](https://x.ai/
+) ð¥ OpenChat-3.5-0106 (7B) now outperforms Grok-0 (33B) on **all 4
+benchmarks** and Grok-1 (???B) on average and **3/4 benchmarks**. | | License |
+# Param | Average | MMLU | HumanEval | MATH | GSM8k | |-----------------------
+|-------------|---------|----------|--------|-----------|----------|----------
+| | **OpenChat-3.5-0106** | Apache-2.0 | **7B** | **61.0** | 65.8 | **71.3** |
+**29.3** | **77.4** | | Grok-0 | Proprietary | 33B | 44.5 | 65.7 | 39.7 | 15.7
+| 56.8 | | Grok-1 | Proprietary | ???B | 55.8 | **73** | 63.2 | 23.9 | 62.9 | #
+â¬ï¸ Installation > [!NOTE] > Need [`pytorch`](https://pytorch.org/get-
+started/locally/#start-locally) to run OpenChat ## pip ```bash pip3 install
+ochat ``` > [!IMPORTANT] > If you are facing package compatibility issues with
+pip, try the conda method below or check [this issue](https://github.com/
+imoneoi/openchat/issues/41) ## conda ```bash conda create -y --name openchat
+python=3.11 conda activate openchat pip3 install ochat ``` ## Windows (WSL 1.x,
+Ubuntu-22.04) ```bash sudo apt update sudo apt install build-essential sudo apt
+install -y curl curl -o miniconda.sh https://repo.anaconda.com/miniconda/
+Miniconda3-latest-Linux-x86_64.sh bash miniconda.sh # Restart WSL terminal if
+the following conda command does not work conda create -y --name openchat
+python=3.11 conda activate openchat pip3 install ochat ``` ## From source Clone
+this repo and install openchat from source in editable mode ```bash git clone
+https://github.com/imoneoi/openchat cd openchat pip3 install --upgrade pip #
+enable PEP 660 support pip3 install -e . # Editable mode, you can make changes
+in this cloned repo ``` # ð Deploying API server â¡ Our API server is ready
+for production use and compatible with the OpenAI API protocol. It is highly
 optimized with vLLM and can dynamically batch requests. ð Note: For 20
 series or older GPUs that do not support `bfloat16`, add `--dtype float16` to
 the server args. ### For a single GPU (e.g. RTX 3090, 4090) ```bash python -
 m ochat.serving.openai_api_server --model openchat/openchat-3.5-0106 ``` ###
 For multiple GPUs (tensor parallel) ```bash # N is the number of tensor
 parallel GPUs python -m ochat.serving.openai_api_server --model openchat/
 openchat-3.5-0106 --engine-use-ray --worker-use-ray --tensor-parallel-size N
@@ -154,141 +158,102 @@
 Correct User: 10.3 â 7988.8133=<|end_of_turn|>Math Correct Assistant: ```
 â ï¸ **Notice:** Remember to set `<|end_of_turn|>` as end of generation
 token. The default (GPT4 Correct) template is also available as the integrated
 `tokenizer.chat_template`, which can be used instead of manually specifying the
 template. # ð ï¸ Training The OpenChat training system utilizes padding-free
 training and the [Multipack Sampler](https://github.com/imoneoi/
 multipack_sampler), achieving a **3~10x** speedup compared to the conventional
-padded training. ## Choose a base model OpenChat supports Llama 2 and Mistral
+padded training. ## Choose a base model OpenChat supports Llama 3 and Mistral
 models. Please first choose a base model to fit your needs. Each base model has
 a corresponding weight repo, model type, and recommended batch size as listed
 below, they should be filled into `BASE_REPO`, `MODEL_TYPE`, and `BATCH_SIZE`
 in the following instructions. | Base Model | Size | Weights (with EOT token) |
 Model Type | Recommended Batch Size per GPU (8xA100 80GB) | |------------|-----
--|-----------------------------------|-------------------------|---------------
------------------------| | Mistral | 7B | `imone/Mistral_7B_with_EOT_token` |
-`openchat_v3.2_mistral` | 77824 | | Llama 2 | 7B | `imone/
-LLaMA2_7B_with_EOT_token` | `openchat_v3.2` | 77824 | | Llama 2 | 13B | `imone/
-Llama2_13B_with_EOT_token` | `openchat_v3.2` | 36864 | Note: The OpenChat
-conversation template requires an `<|end_of_turn|>` special token. The base
-model specified must include this token. Our provided weights are the original
-base weights with this token added. If you want to add them manually, use the
-`convert_llama_weights_to_hf_add_tokens.py` or `mistral_add_tokens.py` in the
-`scripts` directory. ## Installing DeepSpeed and Flash Attention First, ensure
-that the CUDA `nvcc` compiler is available in your environment. If it is not,
-install the CUDA toolkit that matches the version used by PyTorch. Next,
-install building dependencies: ```bash pip install packaging ninja ``` Finally,
-install the packages: ```bash pip install deepspeed flash-attn ``` ###
-Preparing Your Data To utilize the OpenChat trainer, prepare your SFT data into
-a JSON Lines format where each line corresponds to a `Conversation` object:
-```python class Message(BaseModel): role: str # Must be "user" or "assistant"
-content: str # Message content weight: Optional[float] = None # Loss weight for
-this message. Typically 0 for user and 1 for assistant to supervise assistant's
-responses only class Conversation(BaseModel): items: List[Message] # All
-messages within the conversation condition: str = "" # C-RLFT condition, can be
-any string or empty. system: str = "" # System message for this conversation
-``` For basic SFT, assign `weight` as `0` for human messages and `1` for
-assistant responses. SFT example: ```json {"items":[{"role":"user","content":
-"Hello","weight":0.0},{"role":"assistant","content":"Hi","weight":1.0},{"role":
-"user","content":"How are you today?","weight":0.0},{"role":
-"assistant","content":"I'm fine.","weight":1.0}],"system":""} {"items":[
-{"role":"user","content":"Who are you?","weight":0.0},{"role":
-"assistant","content":"I'm OpenChat.","weight":1.0}],"system":"You are a
-helpful assistant named OpenChat."} ``` For C-RLFT, `condition` should be set
-as the class the conversation belongs to (e.g. `GPT3` or `GPT4`). The `weight`
-is assigned as `0` for human messages and `w` for assistant responses, where
-`w` is the weight of the class (e.g. `0.1` for `GPT3` and `1` for `GPT4`, as
-found in our C-RLFT paper). C-RLFT example: ```json {"items":[{"role":
-"user","content":"What is C-RLFT?","weight":0.0},{"role":"assistant","content":
-"C-RLFT is a method for improving open-source LLMs with mixed-quality
-data.","weight":1.0}],"condition":"GPT4","system":""} {"items":[{"role":
-"user","content":"What is C-RLFT?","weight":0.0},{"role":"assistant","content":
-"I don't know.","weight":0.1}],"condition":"GPT3","system":""} ``` ### Pre-
-tokenizing the Dataset You'll then need to pre-tokenize the dataset using the
-command (please specify a filename as `PRETOKENIZED_DATA_OUTPUT_PATH` to store
-the pretokenized dataset): ```bash python -m ochat.data.generate_dataset --
-model-type MODEL_TYPE --model-path BASE_REPO --in-files data.jsonl --out-prefix
-PRETOKENIZED_DATA_OUTPUT_PATH ``` ### Launching the OpenChat Trainer You can
-now launch the OpenChat trainer using the command below. - 13B model requires
-eight `A/H100s` with 80GB VRAM - 7B model can be trained with four `A/H100s`
-with 80GB VRAM or eight `A/H100s` with 40GB VRAM. For hyperparameters, we
-recommend first setting the batch size to the recommended batch size. If OOM
-occurs, try setting it to the exact maximum that VRAM can hold and as a
-multiple of `2048`. Other hyperparameters have been carefully selected as the
-default. Furthermore, the learning rate is automatically determined based on
-the [inverse square-root rule](https://arxiv.org/abs/2006.09092). Training
-Commands (click to expand) ```bash NUM_GPUS=8 deepspeed --num_gpus=$NUM_GPUS --
-module ochat.training_deepspeed.train \ --model_path BASE_REPO \ --data_prefix
+-|--------------------------------------------|-------------------------|------
+----------------------------------------| | Llama 3 | 8B | `imone/Llama-3-8B-
+fixed-special-embedding` | `openchat_3.6` | 40960 | | Mistral | 7B | `imone/
+Mistral_7B_with_EOT_token` | `openchat_v3.2_mistral` | 77824 | Note: The
+OpenChat conversation template requires `<|eot_id|>, <|start_header_id|>,
+<|end_header_id|>` (Llama 3) `<|end_of_turn|>` (Mistral) special tokens. The
+base model specified must include these tokens with initialized embeddings. Our
+provided weights are the original base weights with this token added and
+embeddings initialized. If you want to add them manually, use the
+`init_special_embedding_llama3.py` or `mistral_add_tokens.py` in the `scripts`
+directory. ## Installing DeepSpeed and Flash Attention First, ensure that the
+CUDA `nvcc` compiler is available in your environment. If it is not, install
+the CUDA toolkit that matches the version used by PyTorch. Next, install
+building dependencies: ```bash pip install packaging ninja ``` Finally, install
+the packages: ```bash pip install deepspeed flash-attn ``` ### Preparing Your
+Data To utilize the OpenChat trainer, prepare your SFT data into a JSON Lines
+format where each line corresponds to a `Conversation` object: ```python class
+Message(BaseModel): role: str # Must be "user" or "assistant" content: str #
+Message content weight: Optional[float] = None # Loss weight for this message.
+Typically 0 for user and 1 for assistant to supervise assistant's responses
+only class Conversation(BaseModel): items: List[Message] # All messages within
+the conversation condition: str = "" # C-RLFT condition, can be any string or
+empty. system: str = "" # System message for this conversation ``` For basic
+SFT, assign `weight` as `0` for human messages and `1` for assistant responses.
+SFT example: ```json {"items":[{"role":"user","content":"Hello","weight":0.0},
+{"role":"assistant","content":"Hi","weight":1.0},{"role":"user","content":"How
+are you today?","weight":0.0},{"role":"assistant","content":"I'm
+fine.","weight":1.0}],"system":""} {"items":[{"role":"user","content":"Who are
+you?","weight":0.0},{"role":"assistant","content":"I'm OpenChat.","weight":
+1.0}],"system":"You are a helpful assistant named OpenChat."} ``` For C-RLFT,
+`condition` should be set as the class the conversation belongs to (e.g. `GPT3`
+or `GPT4`). The `weight` is assigned as `0` for human messages and `w` for
+assistant responses, where `w` is the weight of the class (e.g. `0.1` for
+`GPT3` and `1` for `GPT4`, as found in our C-RLFT paper). C-RLFT example:
+```json {"items":[{"role":"user","content":"What is C-RLFT?","weight":0.0},
+{"role":"assistant","content":"C-RLFT is a method for improving open-source
+LLMs with mixed-quality data.","weight":1.0}],"condition":"GPT4","system":""}
+{"items":[{"role":"user","content":"What is C-RLFT?","weight":0.0},{"role":
+"assistant","content":"I don't know.","weight":0.1}],"condition":
+"GPT3","system":""} ``` ### Pre-tokenizing the Dataset You'll then need to pre-
+tokenize the dataset using the command (please specify a filename as
+`PRETOKENIZED_DATA_OUTPUT_PATH` to store the pretokenized dataset): ```bash
+python -m ochat.data.generate_dataset --model-type MODEL_TYPE --model-path
+BASE_REPO --in-files data.jsonl --out-prefix PRETOKENIZED_DATA_OUTPUT_PATH ```
+### Launching the OpenChat Trainer You can now launch the OpenChat trainer
+using the command below. - 13B model requires eight `A/H100s` with 80GB VRAM -
+7B model can be trained with four `A/H100s` with 80GB VRAM or eight `A/H100s`
+with 40GB VRAM. For hyperparameters, we recommend first setting the batch size
+to the recommended batch size. If OOM occurs, try setting it to the exact
+maximum that VRAM can hold and as a multiple of `2048`. Other hyperparameters
+have been carefully selected as the default. Furthermore, the learning rate is
+automatically determined based on the [inverse square-root rule](https://
+arxiv.org/abs/2006.09092). Training Commands (click to expand) ```bash
+NUM_GPUS=8 deepspeed --num_gpus=$NUM_GPUS --module
+ochat.training_deepspeed.train \ --model_path BASE_REPO \ --data_prefix
 PRETOKENIZED_DATA_OUTPUT_PATH \ --save_path PATH_TO_SAVE_MODEL \ --
 batch_max_len BATCH_SIZE \ --epochs 5 \ --save_every 1 \ --deepspeed \ --
 deepspeed_config ochat/training_deepspeed/deepspeed_config.json ``` You can
 find checkpoints of all epochs in `PATH_TO_SAVE_MODEL`. Then you may evaluate
 each epoch and choose the best one. # Limitations ## Foundation Model
 Limitations Despite its advanced capabilities, OpenChat is still bound by the
 limitations inherent in its foundation models. These limitations may impact the
 model's performance in areas such as: - Complex reasoning - Mathematical and
 arithmetic tasks - Programming and coding challenges ## Hallucination of Non-
 existent Information OpenChat may sometimes generate information that does not
 exist or is not accurate, also known as "hallucination". Users should be aware
 of this possibility and verify any critical information obtained the model. ##
 Safety OpenChat may sometimes generate harmful, hate speech, biased responses,
 or answer unsafe questions. It's crucial to apply additional AI safety measures
-in use cases that require safe and moderated responses. # License Our OpenChat
-3.5 `code` and `models` are distributed under the **Apache License 2.0**. #
-Models | Model | Size | Context | Weights | Serving | |--------------|------|--
--------|-------------------------------------------------------------|---------
--------------------------------------------------------------------------------
----------------------| | OpenChat 3.5 0106 | 7B | 8192 | [Huggingface](https://
-huggingface.co/openchat/openchat-3.5-0106) | `python -
-m ochat.serving.openai_api_server --model openchat/openchat-3.5-0106 --engine-
-use-ray --worker-use-ray` | | OpenChat 3.5 1210 | 7B | 8192 | [Huggingface]
-(https://huggingface.co/openchat/openchat-3.5-1210) | `python -
-m ochat.serving.openai_api_server --model openchat/openchat-3.5-1210 --engine-
-use-ray --worker-use-ray` | | OpenChat 3.5 | 7B | 8192 | [Huggingface](https://
-huggingface.co/openchat/openchat_3.5) | `python -
-m ochat.serving.openai_api_server --model openchat/openchat_3.5 --engine-use-
-ray --worker-use-ray` | ## Legacy Models The following models are older
-versions of OpenChat and have inferior performance compared to the latest
-version. They will be deprecated in the next release. Please note that OpenChat
-V1 and V2 series are now deprecated, [please install 3.1.x for using V1 and V2
-models](https://github.com/imoneoi/openchat/tree/
-83a683c775c77867cc45937fafdf48e8dcb68daa) To run the models on multiple GPUs
-with smaller VRAM, you can enable tensor parallelization, for example, using
-the `--tensor-parallel-size 2` flag. | Model | Size | Context | Weights |
-Serving | |--------------|------|---------|------------------------------------
---------------------------|----------------------------------------------------
-----------------------------------------------------------| | OpenChat 3.2
-SUPER | 13B | 4096 | [Huggingface](https://huggingface.co/openchat/
-openchat_v3.2_super) | `python -m ochat.serving.openai_api_server --model
-openchat/openchat_v3.2_super --engine-use-ray --worker-use-ray` | # Citation
-``` @article{wang2023openchat, title={OpenChat: Advancing Open-source Language
-Models with Mixed-Quality Data}, author={Wang, Guan and Cheng, Sijie and Zhan,
-Xianyuan and Li, Xiangang and Song, Sen and Liu, Yang}, journal={arXiv preprint
-arXiv:2309.11235}, year={2023} } ``` # ðContact We are a student team at
-Tsinghua University, working on OpenChat, a project that requires additional
-computing power or LLMs API keys for further development. If you are interested
-in our project and would like to offer support, please feel free to reach out
-to us: **Project Leader:** - Guan Wang [imonenext at gmail dot com] - [Sijie
-Cheng](https://adacheng.github.io/) [csj23 at mails dot tsinghua dot edu dot
-cn] **Main Contributors:** - [Xianyuan Zhan](https://scholar.google.com.hk/
-citations?user=pDMnGloAAAAJ&hl=zh-CN) (Tsinghua University): Provided
-invaluable advice on paper writing. - [Alpay Ariyak](https://github.com/
-alpayariyak): Responsible for data collection, documentation, model cards and
-PR for `openchat-3.5-1210`, `openchat-3.5-0106`. - LDJ: Tasked with partial
-data collection for `openchat-3.5`. **Sponsors:** - [Sen Song](https://
-scholar.google.com/citations?user=cYgtRP4AAAAJ&hl=en) (Tsinghua University),
-[Yang Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University), [01.AI
-Company](https://www.lingyiwanwu.com/en), [RunPod](https://www.runpod.io/),
-Changling Liu (GPT Desk Pte. Ltd.), Qiying Yu (Tsinghua University), AutoMeta
-(Alignment Lab AI). **Special Thanks:** - We express our profound gratitude to
-Alignment Lab AI, Nous Research, and Pygmalion AI for their significant
-contributions to data collection and model training. We also extend our special
-thanks to Xiangang Li, Baochang Ma, and Hao Wan from 01.AI company for their
-generous provision of resources. We also thank Jianxiong Li and Peng Li at
-Tsinghua University for their insightful discussions that have enriched our
-work. - We acknowledge and thank the developers behind these projects:
-[Mistral](https://mistral.ai/), [Chain-of-Thought Hub](https://github.com/
-FranxYao/chain-of-thought-hub), [Llama 2](https://ai.meta.com/llama/), [Self-
-Instruct](https://arxiv.org/abs/2212.10560), [FastChat (Vicuna)](https://
-github.com/lm-sys/FastChat), [Alpaca](https://github.com/tatsu-lab/
-stanford_alpaca.git), and [StarCoder](https://github.com/bigcode-project/
-starcoder). Their work has been instrumental in driving our research forward.
+in use cases that require safe and moderated responses. # License Code is
+distributed under the **Apache License 2.0**. # Citation ``` @article
+{wang2023openchat, title={OpenChat: Advancing Open-source Language Models with
+Mixed-Quality Data}, author={Wang, Guan and Cheng, Sijie and Zhan, Xianyuan and
+Li, Xiangang and Song, Sen and Liu, Yang}, journal={arXiv preprint arXiv:
+2309.11235}, year={2023} } ``` # ðContact **Project Lead:** - Guan Wang
+[imonenext at gmail dot com] - [Alpay Ariyak](https://github.com/alpayariyak)
+[aariyak at wpi dot edu] **Main Contributors:** - [Xianyuan Zhan](https://
+scholar.google.com.hk/citations?user=pDMnGloAAAAJ) (Tsinghua University) -
+Qiying Yu (Tsinghua University) - Changling Liu (GPT Desk Pte. Ltd.) - LDJ -
+AutoMeta (Alignment Lab AI) **Sponsors:** - [Sen Song](https://
+scholar.google.com/citations?user=cYgtRP4AAAAJ) (Tsinghua University) - [Yang
+Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University) - [01.AI
+Company](https://www.lingyiwanwu.com/en) - [RunPod](https://www.runpod.io/
+) **Special Thanks:** - [Mistral](https://mistral.ai/) - [Chain-of-Thought Hub]
+(https://github.com/FranxYao/chain-of-thought-hub) - [Llama 2](https://
+ai.meta.com/llama/) - [Self-Instruct](https://arxiv.org/abs/2212.10560) -
+[FastChat (Vicuna)](https://github.com/lm-sys/FastChat) - [Alpaca](https://
+github.com/tatsu-lab/stanford_alpaca.git) - [StarCoder](https://github.com/
+bigcode-project/starcoder)
```

### Comparing `ochat-3.5.2/README.md` & `ochat-3.6.0/ochat.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,68 @@
+Metadata-Version: 2.1
+Name: ochat
+Version: 3.6.0
+Summary: An efficient framework for training and serving top-tier, open-source conversational LLMs.
+Project-URL: Homepage, https://github.com/imoneoi/openchat
+Project-URL: Bug Tracker, https://github.com/imoneoi/openchat/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify
+Requires-Dist: pylatexenc
+Requires-Dist: openai>=1
+Requires-Dist: tenacity
+Requires-Dist: tiktoken
+Requires-Dist: tqdm
+Requires-Dist: wandb
+Requires-Dist: numba
+Requires-Dist: datasets
+Requires-Dist: orjson
+Requires-Dist: torch
+Requires-Dist: packaging
+Requires-Dist: ninja
+Requires-Dist: flash-attn
+Requires-Dist: ray
+Requires-Dist: sentencepiece
+Requires-Dist: transformers>=4.40.1
+Requires-Dist: accelerate
+Requires-Dist: protobuf
+Requires-Dist: fastapi
+Requires-Dist: pydantic
+Requires-Dist: shortuuid
+Requires-Dist: uvicorn
+Requires-Dist: vllm>=0.4.0
+Requires-Dist: pytest
+
 # OpenChat: Advancing Open-source Language Models with Mixed-Quality Data
 
 <div align="center">
   <img src="assets/logo_new.png" style="width: 65%">
 </div>
 
 <p align="center">
   <a href="https://openchat.team">💻Online Demo</a> |
   <a href="https://huggingface.co/openchat">🤗Huggingface</a> |
   <a href="https://arxiv.org/pdf/2309.11235.pdf">📃Paper</a> |
   <a href="https://discord.gg/pQjnXvNKHY">💭Discord</a> 
-  <br><br>
-  <strong>🏆 The Overall Best Performing Open Source 7B Model 🏆</strong>
-  <br>
-  <strong>🤖 Outperforms ChatGPT (March) and Grok-1 🤖</strong>
-  <br>
 </p>
 
-<div align="center">
-  <img src="https://raw.githubusercontent.com/imoneoi/openchat/master/assets/openchat-bench-0106.png" style="width: 95%;">
-</div>
-
 - OpenChat is an innovative library of **open-source language models**, fine-tuned with [**C-RLFT**](https://arxiv.org/pdf/2309.11235.pdf) - a strategy inspired by offline reinforcement learning.
 - Our models learn from mixed-quality data without preference labels, delivering exceptional performance on par with `ChatGPT`, even with a `7B` model which can be run on a **consumer GPU (e.g. RTX 3090)**.
 - Despite our simple approach, we are committed to developing a high-performance, commercially viable, open-source large language model, and we continue to make significant strides toward this vision.
 
 [![DOI](https://zenodo.org/badge/645397533.svg)](https://zenodo.org/badge/latestdoi/645397533)
 
 # ✨ News
 
+ - [2024/05/22] We released the Llama-3 based version [OpenChat 3.6 20240522](https://huggingface.co/openchat/openchat-3.6-8b-20240522), outperforming official Llama 3 8B Instruct and open-source finetunes/merges.
+
 - [2024/01/06] We released the second update, [OpenChat 3.5 0106](openchat/openchat-3.5-0106), further improved coding and overall performance 🏆.
 
 - [2023/12/10] We released the first update, [OpenChat 3.5 1210](openchat/openchat-3.5-1210), improved coding by 15 points 🚀.
 
 - [2023/11/01] We released the [OpenChat-3.5-7B](https://huggingface.co/openchat/openchat_3.5) model, surpassing ChatGPT on various benchmarks 🔥.
 
 - [2023/09/21] We released our paper [OpenChat: Advancing Open-source Language Models with Mixed-Quality Data](https://arxiv.org/pdf/2309.11235.pdf).
@@ -46,21 +77,39 @@
 - [2023/07/30] We are thrilled to introduce the [OpenChat V3 model series](#models), based on Llama 2, and now available for free for commercial use!
 
 - [2023/07/07] We released the [OpenChat V2 model series](#legacy-models).
 
 - [2023/07/01] We released the [OpenChat V1 model series](#legacy-models).
 </details>
 
-# 🏷️ Benchmarks
+# 🏷️ Benchmarks - OpenChat 3.6
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/imoneoi/openchat/master/assets/benchmarks-openchat-3.6-20240522.svg" style="width: 95%;">
+</div>
+
+
+<details>
+  <summary>Reproducing benchmarks</summary>
+
+Note: Please run the following commands at the base directory of this repository.
+
+```bash
+python -m ochat.evaluation.run_eval --condition "GPT4 Correct" --model openchat/openchat-3.6-8b-20240522 --eval_sets fs_cothub/mmlu fs_cothub/gsm8k fs_cothub/math
+python -m ochat.evaluation.run_eval --condition "GPT4" --model openchat/openchat-3.6-8b-20240522 --eval_sets zs/gpqa
+```
+
+HumanEval is run using the official [EvalPlus repository](https://github.com/evalplus/evalplus).
+</details>
+
+# 🏷️ Benchmarks - OpenChat 3.5
 
 | Model                 | # Params | Average  | MT-Bench     | HumanEval       | BBH MC   | AGIEval  | TruthfulQA    | MMLU         | GSM8K        | BBH CoT     |
 |-----------------------|----------|----------|--------------|-----------------|----------|----------|---------------|--------------|--------------|-------------|
 | **OpenChat-3.5-0106** | **7B**   | **64.5** | 7.8          | **71.3**        | **51.5** | **49.1** | 61.0          | 65.8         | **77.4**     | 62.2        |
-| OpenChat-3.5-1210     | **7B**   | 63.8     | 7.76         | 68.9            | 49.5     | 48.0     | **61.8**      | 65.3         | 77.3         | 61.8        |
-| OpenChat-3.5          | **7B**   | 61.6     | 7.81         | 55.5            | 47.6     | 47.4     | 59.1          | 64.3         | 77.3         | 63.5        |
 | ChatGPT (March)*      | ???B     | 61.5     | **7.94**     | 48.1            | 47.6     | 47.1     | 57.7          | **67.3**     | 74.9         | **70.1**    |
 |                       |          |          |              |                 |          |          |               |              |              |             |
 | OpenHermes 2.5        | 7B       | 59.3     | 7.54         | 48.2            | 49.4     | 46.5     | 57.5          | 63.8         | 73.5         | 59.9        |
 | OpenOrca Mistral      | 7B       | 52.7     | 6.86         | 38.4            | 49.4     | 42.9     | 45.9          | 59.3         | 59.1         | 58.1        |
 | Zephyr-β^             | 7B       | 34.6     | 7.34         | 22.0            | 40.6     | 39.0     | 40.8          | 39.8         | 5.1          | 16.0        |
 | Mistral               | 7B       | -        | 6.84         | 30.5            | 39.0     | 38.0     | -             | 60.1         | 52.2         | -           |
 | Open-source SOTA**    | 13B-70B  | 61.4     | 7.71         | 73.2            | 49.7     | 41.7     | 62.3          | 63.7         | 82.3         | 41.4        |
@@ -122,16 +171,14 @@
 ## 🎇 Comparison with [X.AI Grok](https://x.ai/)
 
 🔥 OpenChat-3.5-0106 (7B) now outperforms Grok-0 (33B) on **all 4 benchmarks** and Grok-1 (???B) on average and **3/4 benchmarks**.
 
 |                       | License     | # Param | Average  | MMLU   | HumanEval | MATH     | GSM8k    |
 |-----------------------|-------------|---------|----------|--------|-----------|----------|----------|
 | **OpenChat-3.5-0106** | Apache-2.0  | **7B**  | **61.0** | 65.8   | **71.3**  | **29.3** | **77.4** |
-| OpenChat-3.5-1210     | Apache-2.0  | **7B**  | 60.1     | 65.3   | 68.9      | 28.9     | 77.3     |
-| OpenChat-3.5          | Apache-2.0  | **7B**  | 56.4     | 64.3   | 55.5      | 28.6     | 77.3     |
 | Grok-0                | Proprietary | 33B     | 44.5     | 65.7   | 39.7      | 15.7     | 56.8     |
 | Grok-1                | Proprietary | ???B    | 55.8     | **73** | 63.2      | 23.9     | 62.9     |
 
 # ⬇️ Installation
 > [!NOTE]
 > Need [`pytorch`](https://pytorch.org/get-started/locally/#start-locally) to run OpenChat
 
@@ -269,23 +316,22 @@
 
 # <a id="training"></a> 🛠️ Training
 
 The OpenChat training system utilizes padding-free training and the [Multipack Sampler](https://github.com/imoneoi/multipack_sampler), achieving a **3~10x** speedup compared to the conventional padded training.
 
 ## Choose a base model
 
-OpenChat supports Llama 2 and Mistral models. Please first choose a base model to fit your needs. Each base model has a corresponding weight repo, model type, and recommended batch size as listed below, they should be filled into `BASE_REPO`, `MODEL_TYPE`, and `BATCH_SIZE` in the following instructions.
+OpenChat supports Llama 3 and Mistral models. Please first choose a base model to fit your needs. Each base model has a corresponding weight repo, model type, and recommended batch size as listed below, they should be filled into `BASE_REPO`, `MODEL_TYPE`, and `BATCH_SIZE` in the following instructions.
 
-| Base Model | Size | Weights (with EOT token)          | Model Type              | Recommended Batch Size per GPU (8xA100 80GB) |
-|------------|------|-----------------------------------|-------------------------|--------------------------------------|
-| Mistral    | 7B   | `imone/Mistral_7B_with_EOT_token` | `openchat_v3.2_mistral` | 77824                                |
-| Llama 2    | 7B   | `imone/LLaMA2_7B_with_EOT_token`  | `openchat_v3.2`         | 77824                                |
-| Llama 2    | 13B  | `imone/Llama2_13B_with_EOT_token` | `openchat_v3.2`         | 36864                                |
+| Base Model | Size | Weights (with EOT token)                   | Model Type              | Recommended Batch Size per GPU (8xA100 80GB) |
+|------------|------|--------------------------------------------|-------------------------|----------------------------------------------|
+| Llama 3    | 8B   | `imone/Llama-3-8B-fixed-special-embedding` | `openchat_3.6`          | 40960                                        |
+| Mistral    | 7B   | `imone/Mistral_7B_with_EOT_token`          | `openchat_v3.2_mistral` | 77824                                        |
 
-Note: The OpenChat conversation template requires an `<|end_of_turn|>` special token. The base model specified must include this token. Our provided weights are the original base weights with this token added. If you want to add them manually, use the `convert_llama_weights_to_hf_add_tokens.py` or `mistral_add_tokens.py` in the `scripts` directory.
+Note: The OpenChat conversation template requires `<|eot_id|>, <|start_header_id|>, <|end_header_id|>` (Llama 3) `<|end_of_turn|>` (Mistral) special tokens. The base model specified must include these tokens with initialized embeddings. Our provided weights are the original base weights with this token added and embeddings initialized. If you want to add them manually, use the `init_special_embedding_llama3.py` or `mistral_add_tokens.py` in the `scripts` directory.
 
 ## Installing DeepSpeed and Flash Attention
 
 First, ensure that the CUDA `nvcc` compiler is available in your environment. If it is not, install the CUDA toolkit that matches the version used by PyTorch.
 
 Next, install building dependencies:
 
@@ -386,57 +432,47 @@
 OpenChat may sometimes generate information that does not exist or is not accurate, also known as "hallucination". Users should be aware of this possibility and verify any critical information obtained the model.
 
 ## Safety
 OpenChat may sometimes generate harmful, hate speech, biased responses, or answer unsafe questions. It's crucial to apply additional AI safety measures in use cases that require safe and moderated responses.
 
 # License
 
-Our OpenChat 3.5 `code` and `models` are distributed under the **Apache License 2.0**.
-
-# <a id="models"></a> Models
-
-| Model        | Size | Context | Weights                                                     | Serving                                                                                                     |
-|--------------|------|---------|-------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
-| OpenChat 3.5 0106 | 7B   | 8192    | [Huggingface](https://huggingface.co/openchat/openchat-3.5-0106) | `python -m ochat.serving.openai_api_server --model openchat/openchat-3.5-0106 --engine-use-ray --worker-use-ray` |
-| OpenChat 3.5 1210 | 7B   | 8192    | [Huggingface](https://huggingface.co/openchat/openchat-3.5-1210) | `python -m ochat.serving.openai_api_server --model openchat/openchat-3.5-1210 --engine-use-ray --worker-use-ray` |
-| OpenChat 3.5 | 7B   | 8192    | [Huggingface](https://huggingface.co/openchat/openchat_3.5) | `python -m ochat.serving.openai_api_server --model openchat/openchat_3.5 --engine-use-ray --worker-use-ray` |
-
-## <a id="legacy-models"></a> Legacy Models
-
-The following models are older versions of OpenChat and have inferior performance compared to the latest version. They will be deprecated in the next release. Please note that OpenChat V1 and V2 series are now deprecated, [please install 3.1.x for using V1 and V2 models](https://github.com/imoneoi/openchat/tree/83a683c775c77867cc45937fafdf48e8dcb68daa)
-
-To run the models on multiple GPUs with smaller VRAM, you can enable tensor parallelization, for example, using the `--tensor-parallel-size 2` flag.
-
-| Model        | Size | Context | Weights                                                      | Serving                                                                                                      |
-|--------------|------|---------|--------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|
-| OpenChat 3.2 SUPER | 13B  | 4096    | [Huggingface](https://huggingface.co/openchat/openchat_v3.2_super) | `python -m ochat.serving.openai_api_server --model openchat/openchat_v3.2_super --engine-use-ray --worker-use-ray` |
+Code is distributed under the **Apache License 2.0**.
 
 # Citation
 
 ```
 @article{wang2023openchat,
   title={OpenChat: Advancing Open-source Language Models with Mixed-Quality Data},
   author={Wang, Guan and Cheng, Sijie and Zhan, Xianyuan and Li, Xiangang and Song, Sen and Liu, Yang},
   journal={arXiv preprint arXiv:2309.11235},
   year={2023}
 }
 ```
 
 # 💌Contact
 
-We are a student team at Tsinghua University, working on OpenChat, a project that requires additional computing power or LLMs API keys for further development. If you are interested in our project and would like to offer support, please feel free to reach out to us:
-
-**Project Leader:**
+**Project Lead:**
 - Guan Wang [imonenext at gmail dot com]
-- [Sijie Cheng](https://adacheng.github.io/) [csj23 at mails dot tsinghua dot edu dot cn]
+- [Alpay Ariyak](https://github.com/alpayariyak) [aariyak at wpi dot edu]
 
 **Main Contributors:**
-- [Xianyuan Zhan](https://scholar.google.com.hk/citations?user=pDMnGloAAAAJ&hl=zh-CN) (Tsinghua University): Provided invaluable advice on paper writing.
-- [Alpay Ariyak](https://github.com/alpayariyak): Responsible for data collection, documentation, model cards and PR for `openchat-3.5-1210`, `openchat-3.5-0106`.
-- LDJ: Tasked with partial data collection for `openchat-3.5`.
+- [Xianyuan Zhan](https://scholar.google.com.hk/citations?user=pDMnGloAAAAJ) (Tsinghua University)
+- Qiying Yu (Tsinghua University)
+- Changling Liu (GPT Desk Pte. Ltd.)
+- LDJ
+- AutoMeta (Alignment Lab AI)
 
 **Sponsors:**
-- [Sen Song](https://scholar.google.com/citations?user=cYgtRP4AAAAJ&hl=en) (Tsinghua University), [Yang Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University), [01.AI Company](https://www.lingyiwanwu.com/en), [RunPod](https://www.runpod.io/), Changling Liu (GPT Desk Pte. Ltd.), Qiying Yu (Tsinghua University), AutoMeta (Alignment Lab AI).
+- [Sen Song](https://scholar.google.com/citations?user=cYgtRP4AAAAJ) (Tsinghua University)
+- [Yang Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University)
+- [01.AI Company](https://www.lingyiwanwu.com/en)
+- [RunPod](https://www.runpod.io/)
 
 **Special Thanks:**
-- We express our profound gratitude to Alignment Lab AI, Nous Research, and Pygmalion AI for their significant contributions to data collection and model training. We also extend our special thanks to Xiangang Li, Baochang Ma, and Hao Wan from 01.AI company for their generous provision of resources. We also thank Jianxiong Li and Peng Li at Tsinghua University for their insightful discussions that have enriched our work.
-- We acknowledge and thank the developers behind these projects: [Mistral](https://mistral.ai/), [Chain-of-Thought Hub](https://github.com/FranxYao/chain-of-thought-hub), [Llama 2](https://ai.meta.com/llama/), [Self-Instruct](https://arxiv.org/abs/2212.10560), [FastChat (Vicuna)](https://github.com/lm-sys/FastChat), [Alpaca](https://github.com/tatsu-lab/stanford_alpaca.git), and [StarCoder](https://github.com/bigcode-project/starcoder). Their work has been instrumental in driving our research forward.
+ - [Mistral](https://mistral.ai/)
+ - [Chain-of-Thought Hub](https://github.com/FranxYao/chain-of-thought-hub)
+ - [Llama 2](https://ai.meta.com/llama/)
+ - [Self-Instruct](https://arxiv.org/abs/2212.10560)
+ - [FastChat (Vicuna)](https://github.com/lm-sys/FastChat)
+ - [Alpaca](https://github.com/tatsu-lab/stanford_alpaca.git)
+ - [StarCoder](https://github.com/bigcode-project/starcoder)
```

#### html2text {}

```diff
@@ -1,111 +1,129 @@
-# OpenChat: Advancing Open-source Language Models with Mixed-Quality Data
+Metadata-Version: 2.1 Name: ochat Version: 3.6.0 Summary: An efficient
+framework for training and serving top-tier, open-source conversational LLMs.
+Project-URL: Homepage, https://github.com/imoneoi/openchat Project-URL: Bug
+Tracker, https://github.com/imoneoi/openchat/issues Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
+License Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
+Requires-Dist: pylatexenc Requires-Dist: openai>=1 Requires-Dist: tenacity
+Requires-Dist: tiktoken Requires-Dist: tqdm Requires-Dist: wandb Requires-Dist:
+numba Requires-Dist: datasets Requires-Dist: orjson Requires-Dist: torch
+Requires-Dist: packaging Requires-Dist: ninja Requires-Dist: flash-attn
+Requires-Dist: ray Requires-Dist: sentencepiece Requires-Dist:
+transformers>=4.40.1 Requires-Dist: accelerate Requires-Dist: protobuf
+Requires-Dist: fastapi Requires-Dist: pydantic Requires-Dist: shortuuid
+Requires-Dist: uvicorn Requires-Dist: vllm>=0.4.0 Requires-Dist: pytest #
+OpenChat: Advancing Open-source Language Models with Mixed-Quality Data
                              [assets/logo_new.png]
-         _ð___»_O_n_l_i_n_e_ _D_e_m_o | _ð__¤__H_u_g_g_i_n_g_f_a_c_e | _ð____P_a_p_e_r | _ð___­_D_i_s_c_o_r_d
-
-          ?ð??? TThhee OOvveerraallll BBeesstt PPeerrffoorrmmiinngg OOppeenn SSoouurrccee 77BB MMooddeell ?ð???
-               ?ð??¤? OOuuttppeerrffoorrmmss CChhaattGGPPTT ((MMaarrcchh)) aanndd GGrrookk--11 ?ð??¤?
-  [https://raw.githubusercontent.com/imoneoi/openchat/master/assets/openchat-
-                                bench-0106.png]
+          _ð___»_O_n_l_i_n_e_ _D_e_m_o | _ð__¤__H_u_g_g_i_n_g_f_a_c_e | _ð____P_a_p_e_r | _ð___­_D_i_s_c_o_r_d
 - OpenChat is an innovative library of **open-source language models**, fine-
 tuned with [**C-RLFT**](https://arxiv.org/pdf/2309.11235.pdf) - a strategy
 inspired by offline reinforcement learning. - Our models learn from mixed-
 quality data without preference labels, delivering exceptional performance on
 par with `ChatGPT`, even with a `7B` model which can be run on a **consumer GPU
 (e.g. RTX 3090)**. - Despite our simple approach, we are committed to
 developing a high-performance, commercially viable, open-source large language
 model, and we continue to make significant strides toward this vision. [![DOI]
 (https://zenodo.org/badge/645397533.svg)](https://zenodo.org/badge/latestdoi/
-645397533) # â¨ News - [2024/01/06] We released the second update, [OpenChat
-3.5 0106](openchat/openchat-3.5-0106), further improved coding and overall
+645397533) # â¨ News - [2024/05/22] We released the Llama-3 based version
+[OpenChat 3.6 20240522](https://huggingface.co/openchat/openchat-3.6-8b-
+20240522), outperforming official Llama 3 8B Instruct and open-source
+finetunes/merges. - [2024/01/06] We released the second update, [OpenChat 3.5
+0106](openchat/openchat-3.5-0106), further improved coding and overall
 performance ð. - [2023/12/10] We released the first update, [OpenChat 3.5
 1210](openchat/openchat-3.5-1210), improved coding by 15 points ð. - [2023/
 11/01] We released the [OpenChat-3.5-7B](https://huggingface.co/openchat/
 openchat_3.5) model, surpassing ChatGPT on various benchmarks ð¥. - [2023/09/
 21] We released our paper [OpenChat: Advancing Open-source Language Models with
 Mixed-Quality Data](https://arxiv.org/pdf/2309.11235.pdf). Read more - [2023/
 09/03] We released the [OpenChat V3.2 SUPER]([#models](https://huggingface.co/
 openchat/openchat_v3.2_super)) model. - [2023/08/04] We have launched an
 [Online Demo](https://openchat.team) featuring the latest version, OpenChat
 3.2. - [2023/07/30] We are thrilled to introduce the [OpenChat V3 model series]
 (#models), based on Llama 2, and now available for free for commercial use! -
 [2023/07/07] We released the [OpenChat V2 model series](#legacy-models). -
 [2023/07/01] We released the [OpenChat V1 model series](#legacy-models). #
-ð·ï¸ Benchmarks | Model | # Params | Average | MT-Bench | HumanEval | BBH MC
-| AGIEval | TruthfulQA | MMLU | GSM8K | BBH CoT | |-----------------------|----
-------|----------|--------------|-----------------|----------|----------|------
----------|--------------|--------------|-------------| | **OpenChat-3.5-0106**
-| **7B** | **64.5** | 7.8 | **71.3** | **51.5** | **49.1** | 61.0 | 65.8 |
-**77.4** | 62.2 | | OpenChat-3.5-1210 | **7B** | 63.8 | 7.76 | 68.9 | 49.5 |
-48.0 | **61.8** | 65.3 | 77.3 | 61.8 | | OpenChat-3.5 | **7B** | 61.6 | 7.81 |
-55.5 | 47.6 | 47.4 | 59.1 | 64.3 | 77.3 | 63.5 | | ChatGPT (March)* | ???B |
-61.5 | **7.94** | 48.1 | 47.6 | 47.1 | 57.7 | **67.3** | 74.9 | **70.1** | | |
-| | | | | | | | | | | OpenHermes 2.5 | 7B | 59.3 | 7.54 | 48.2 | 49.4 | 46.5 |
-57.5 | 63.8 | 73.5 | 59.9 | | OpenOrca Mistral | 7B | 52.7 | 6.86 | 38.4 | 49.4
-| 42.9 | 45.9 | 59.3 | 59.1 | 58.1 | | Zephyr-Î²^ | 7B | 34.6 | 7.34 | 22.0 |
-40.6 | 39.0 | 40.8 | 39.8 | 5.1 | 16.0 | | Mistral | 7B | - | 6.84 | 30.5 |
-39.0 | 38.0 | - | 60.1 | 52.2 | - | | Open-source SOTA** | 13B-70B | 61.4 |
-7.71 | 73.2 | 49.7 | 41.7 | 62.3 | 63.7 | 82.3 | 41.4 | | | | | WizardLM 70B |
-WizardCoder 34B | Orca 13B | Orca 13B | Platypus2 70B | WizardLM 70B | MetaMath
-70B | Flan-T5 11B | Evaluation details *: ChatGPT (March) results are from GPT-
-4 Technical Report, Chain-of-Thought Hub, and our evaluation. ^: Zephyr-Î²
-often fails to follow few-shot CoT instructions, likely because it was aligned
-with only chat data but not trained on few-shot data. **: Mistral and Open-
-source SOTA results are taken from reported results in instruction-tuned model
-papers and official repositories. All models are evaluated in chat mode (e.g.
-with the respective conversation template applied). All zero-shot benchmarks
-follow the same setting as in the AGIEval paper and Orca paper. CoT tasks use
-the same configuration as Chain-of-Thought Hub, HumanEval is evaluated with
-EvalPlus, and MT-bench is run using FastChat. To reproduce our results, follow
-the instructions below. Reproducing benchmarks Reasoning and Coding: Note:
-Please run the following commands at the base directory of this repository.
-```bash python -m ochat.evaluation.run_eval --condition "GPT4 Correct" --model
-openchat/openchat-3.5-0106 --eval_sets coding fs_cothub/bbh fs_cothub/mmlu zs/
-agieval zs/bbh_mc_orca zs/truthfulqa_orca python ochat/evaluation/
-view_results.py python ochat/evaluation/convert_to_evalplus.py ``` Then all
-humaneval code samples are placed in `ochat/evaluation/evalplus_codegen`. Use
-the following command to evaluate an individual code sample named
-`samples.jsonl` using Docker as a sandbox. ```bash docker run -v $(pwd):/app
-ganler/evalplus:latest --dataset humaneval --samples samples.jsonl ```
-Mathematical Reasoning: Note: Please run the following commands at the base
+ð·ï¸ Benchmarks - OpenChat 3.6
+ [https://raw.githubusercontent.com/imoneoi/openchat/master/assets/benchmarks-
+                          openchat-3.6-20240522.svg]
+Reproducing benchmarks Note: Please run the following commands at the base
 directory of this repository. ```bash python -m ochat.evaluation.run_eval --
-condition "Math Correct" --model openchat/openchat-3.5-0106 --eval_sets
-fs_cothub/gsm8k zs/math python ochat/evaluation/view_results.py ``` MT-Bench:
-Please first launch a local API server, then download FastChat and run the
-following commands. Note: Due to non-zero temperature and GPT-4 API changes
-over time, there might be variations in the results. ```bash cd fastchat/
-llm_judge python gen_api_answer.py --model openchat-3.5-0106 --max-tokens 4096
---parallel 128 --openai-api-base http://localhost:18888/v1 python
-gen_judgment.py --model-list openchat-3.5-0106 --parallel 8 --mode single ```
-## ð Comparison with [X.AI Grok](https://x.ai/) ð¥ OpenChat-3.5-0106 (7B)
-now outperforms Grok-0 (33B) on **all 4 benchmarks** and Grok-1 (???B) on
-average and **3/4 benchmarks**. | | License | # Param | Average | MMLU |
-HumanEval | MATH | GSM8k | |-----------------------|-------------|---------|---
--------|--------|-----------|----------|----------| | **OpenChat-3.5-0106** |
-Apache-2.0 | **7B** | **61.0** | 65.8 | **71.3** | **29.3** | **77.4** | |
-OpenChat-3.5-1210 | Apache-2.0 | **7B** | 60.1 | 65.3 | 68.9 | 28.9 | 77.3 | |
-OpenChat-3.5 | Apache-2.0 | **7B** | 56.4 | 64.3 | 55.5 | 28.6 | 77.3 | | Grok-
-0 | Proprietary | 33B | 44.5 | 65.7 | 39.7 | 15.7 | 56.8 | | Grok-1 |
-Proprietary | ???B | 55.8 | **73** | 63.2 | 23.9 | 62.9 | # â¬ï¸ Installation
-> [!NOTE] > Need [`pytorch`](https://pytorch.org/get-started/locally/#start-
-locally) to run OpenChat ## pip ```bash pip3 install ochat ``` > [!IMPORTANT] >
-If you are facing package compatibility issues with pip, try the conda method
-below or check [this issue](https://github.com/imoneoi/openchat/issues/41) ##
-conda ```bash conda create -y --name openchat python=3.11 conda activate
-openchat pip3 install ochat ``` ## Windows (WSL 1.x, Ubuntu-22.04) ```bash sudo
-apt update sudo apt install build-essential sudo apt install -y curl curl -
-o miniconda.sh https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-
-x86_64.sh bash miniconda.sh # Restart WSL terminal if the following conda
-command does not work conda create -y --name openchat python=3.11 conda
-activate openchat pip3 install ochat ``` ## From source Clone this repo and
-install openchat from source in editable mode ```bash git clone https://
-github.com/imoneoi/openchat cd openchat pip3 install --upgrade pip # enable PEP
-660 support pip3 install -e . # Editable mode, you can make changes in this
-cloned repo ``` # ð Deploying API server â¡ Our API server is ready for
-production use and compatible with the OpenAI API protocol. It is highly
+condition "GPT4 Correct" --model openchat/openchat-3.6-8b-20240522 --eval_sets
+fs_cothub/mmlu fs_cothub/gsm8k fs_cothub/math python -
+m ochat.evaluation.run_eval --condition "GPT4" --model openchat/openchat-3.6-
+8b-20240522 --eval_sets zs/gpqa ``` HumanEval is run using the official
+[EvalPlus repository](https://github.com/evalplus/evalplus). # ð·ï¸
+Benchmarks - OpenChat 3.5 | Model | # Params | Average | MT-Bench | HumanEval |
+BBH MC | AGIEval | TruthfulQA | MMLU | GSM8K | BBH CoT | |---------------------
+--|----------|----------|--------------|-----------------|----------|----------
+|---------------|--------------|--------------|-------------| | **OpenChat-3.5-
+0106** | **7B** | **64.5** | 7.8 | **71.3** | **51.5** | **49.1** | 61.0 | 65.8
+| **77.4** | 62.2 | | ChatGPT (March)* | ???B | 61.5 | **7.94** | 48.1 | 47.6 |
+47.1 | 57.7 | **67.3** | 74.9 | **70.1** | | | | | | | | | | | | | | OpenHermes
+2.5 | 7B | 59.3 | 7.54 | 48.2 | 49.4 | 46.5 | 57.5 | 63.8 | 73.5 | 59.9 | |
+OpenOrca Mistral | 7B | 52.7 | 6.86 | 38.4 | 49.4 | 42.9 | 45.9 | 59.3 | 59.1 |
+58.1 | | Zephyr-Î²^ | 7B | 34.6 | 7.34 | 22.0 | 40.6 | 39.0 | 40.8 | 39.8 | 5.1
+| 16.0 | | Mistral | 7B | - | 6.84 | 30.5 | 39.0 | 38.0 | - | 60.1 | 52.2 | - |
+| Open-source SOTA** | 13B-70B | 61.4 | 7.71 | 73.2 | 49.7 | 41.7 | 62.3 | 63.7
+| 82.3 | 41.4 | | | | | WizardLM 70B | WizardCoder 34B | Orca 13B | Orca 13B |
+Platypus2 70B | WizardLM 70B | MetaMath 70B | Flan-T5 11B | Evaluation details
+*: ChatGPT (March) results are from GPT-4 Technical Report, Chain-of-Thought
+Hub, and our evaluation. ^: Zephyr-Î² often fails to follow few-shot CoT
+instructions, likely because it was aligned with only chat data but not trained
+on few-shot data. **: Mistral and Open-source SOTA results are taken from
+reported results in instruction-tuned model papers and official repositories.
+All models are evaluated in chat mode (e.g. with the respective conversation
+template applied). All zero-shot benchmarks follow the same setting as in the
+AGIEval paper and Orca paper. CoT tasks use the same configuration as Chain-of-
+Thought Hub, HumanEval is evaluated with EvalPlus, and MT-bench is run using
+FastChat. To reproduce our results, follow the instructions below. Reproducing
+benchmarks Reasoning and Coding: Note: Please run the following commands at the
+base directory of this repository. ```bash python -m ochat.evaluation.run_eval
+--condition "GPT4 Correct" --model openchat/openchat-3.5-0106 --eval_sets
+coding fs_cothub/bbh fs_cothub/mmlu zs/agieval zs/bbh_mc_orca zs/
+truthfulqa_orca python ochat/evaluation/view_results.py python ochat/
+evaluation/convert_to_evalplus.py ``` Then all humaneval code samples are
+placed in `ochat/evaluation/evalplus_codegen`. Use the following command to
+evaluate an individual code sample named `samples.jsonl` using Docker as a
+sandbox. ```bash docker run -v $(pwd):/app ganler/evalplus:latest --dataset
+humaneval --samples samples.jsonl ``` Mathematical Reasoning: Note: Please run
+the following commands at the base directory of this repository. ```bash python
+-m ochat.evaluation.run_eval --condition "Math Correct" --model openchat/
+openchat-3.5-0106 --eval_sets fs_cothub/gsm8k zs/math python ochat/evaluation/
+view_results.py ``` MT-Bench: Please first launch a local API server, then
+download FastChat and run the following commands. Note: Due to non-zero
+temperature and GPT-4 API changes over time, there might be variations in the
+results. ```bash cd fastchat/llm_judge python gen_api_answer.py --model
+openchat-3.5-0106 --max-tokens 4096 --parallel 128 --openai-api-base http://
+localhost:18888/v1 python gen_judgment.py --model-list openchat-3.5-0106 --
+parallel 8 --mode single ``` ## ð Comparison with [X.AI Grok](https://x.ai/
+) ð¥ OpenChat-3.5-0106 (7B) now outperforms Grok-0 (33B) on **all 4
+benchmarks** and Grok-1 (???B) on average and **3/4 benchmarks**. | | License |
+# Param | Average | MMLU | HumanEval | MATH | GSM8k | |-----------------------
+|-------------|---------|----------|--------|-----------|----------|----------
+| | **OpenChat-3.5-0106** | Apache-2.0 | **7B** | **61.0** | 65.8 | **71.3** |
+**29.3** | **77.4** | | Grok-0 | Proprietary | 33B | 44.5 | 65.7 | 39.7 | 15.7
+| 56.8 | | Grok-1 | Proprietary | ???B | 55.8 | **73** | 63.2 | 23.9 | 62.9 | #
+â¬ï¸ Installation > [!NOTE] > Need [`pytorch`](https://pytorch.org/get-
+started/locally/#start-locally) to run OpenChat ## pip ```bash pip3 install
+ochat ``` > [!IMPORTANT] > If you are facing package compatibility issues with
+pip, try the conda method below or check [this issue](https://github.com/
+imoneoi/openchat/issues/41) ## conda ```bash conda create -y --name openchat
+python=3.11 conda activate openchat pip3 install ochat ``` ## Windows (WSL 1.x,
+Ubuntu-22.04) ```bash sudo apt update sudo apt install build-essential sudo apt
+install -y curl curl -o miniconda.sh https://repo.anaconda.com/miniconda/
+Miniconda3-latest-Linux-x86_64.sh bash miniconda.sh # Restart WSL terminal if
+the following conda command does not work conda create -y --name openchat
+python=3.11 conda activate openchat pip3 install ochat ``` ## From source Clone
+this repo and install openchat from source in editable mode ```bash git clone
+https://github.com/imoneoi/openchat cd openchat pip3 install --upgrade pip #
+enable PEP 660 support pip3 install -e . # Editable mode, you can make changes
+in this cloned repo ``` # ð Deploying API server â¡ Our API server is ready
+for production use and compatible with the OpenAI API protocol. It is highly
 optimized with vLLM and can dynamically batch requests. ð Note: For 20
 series or older GPUs that do not support `bfloat16`, add `--dtype float16` to
 the server args. ### For a single GPU (e.g. RTX 3090, 4090) ```bash python -
 m ochat.serving.openai_api_server --model openchat/openchat-3.5-0106 ``` ###
 For multiple GPUs (tensor parallel) ```bash # N is the number of tensor
 parallel GPUs python -m ochat.serving.openai_api_server --model openchat/
 openchat-3.5-0106 --engine-use-ray --worker-use-ray --tensor-parallel-size N
@@ -140,141 +158,102 @@
 Correct User: 10.3 â 7988.8133=<|end_of_turn|>Math Correct Assistant: ```
 â ï¸ **Notice:** Remember to set `<|end_of_turn|>` as end of generation
 token. The default (GPT4 Correct) template is also available as the integrated
 `tokenizer.chat_template`, which can be used instead of manually specifying the
 template. # ð ï¸ Training The OpenChat training system utilizes padding-free
 training and the [Multipack Sampler](https://github.com/imoneoi/
 multipack_sampler), achieving a **3~10x** speedup compared to the conventional
-padded training. ## Choose a base model OpenChat supports Llama 2 and Mistral
+padded training. ## Choose a base model OpenChat supports Llama 3 and Mistral
 models. Please first choose a base model to fit your needs. Each base model has
 a corresponding weight repo, model type, and recommended batch size as listed
 below, they should be filled into `BASE_REPO`, `MODEL_TYPE`, and `BATCH_SIZE`
 in the following instructions. | Base Model | Size | Weights (with EOT token) |
 Model Type | Recommended Batch Size per GPU (8xA100 80GB) | |------------|-----
--|-----------------------------------|-------------------------|---------------
------------------------| | Mistral | 7B | `imone/Mistral_7B_with_EOT_token` |
-`openchat_v3.2_mistral` | 77824 | | Llama 2 | 7B | `imone/
-LLaMA2_7B_with_EOT_token` | `openchat_v3.2` | 77824 | | Llama 2 | 13B | `imone/
-Llama2_13B_with_EOT_token` | `openchat_v3.2` | 36864 | Note: The OpenChat
-conversation template requires an `<|end_of_turn|>` special token. The base
-model specified must include this token. Our provided weights are the original
-base weights with this token added. If you want to add them manually, use the
-`convert_llama_weights_to_hf_add_tokens.py` or `mistral_add_tokens.py` in the
-`scripts` directory. ## Installing DeepSpeed and Flash Attention First, ensure
-that the CUDA `nvcc` compiler is available in your environment. If it is not,
-install the CUDA toolkit that matches the version used by PyTorch. Next,
-install building dependencies: ```bash pip install packaging ninja ``` Finally,
-install the packages: ```bash pip install deepspeed flash-attn ``` ###
-Preparing Your Data To utilize the OpenChat trainer, prepare your SFT data into
-a JSON Lines format where each line corresponds to a `Conversation` object:
-```python class Message(BaseModel): role: str # Must be "user" or "assistant"
-content: str # Message content weight: Optional[float] = None # Loss weight for
-this message. Typically 0 for user and 1 for assistant to supervise assistant's
-responses only class Conversation(BaseModel): items: List[Message] # All
-messages within the conversation condition: str = "" # C-RLFT condition, can be
-any string or empty. system: str = "" # System message for this conversation
-``` For basic SFT, assign `weight` as `0` for human messages and `1` for
-assistant responses. SFT example: ```json {"items":[{"role":"user","content":
-"Hello","weight":0.0},{"role":"assistant","content":"Hi","weight":1.0},{"role":
-"user","content":"How are you today?","weight":0.0},{"role":
-"assistant","content":"I'm fine.","weight":1.0}],"system":""} {"items":[
-{"role":"user","content":"Who are you?","weight":0.0},{"role":
-"assistant","content":"I'm OpenChat.","weight":1.0}],"system":"You are a
-helpful assistant named OpenChat."} ``` For C-RLFT, `condition` should be set
-as the class the conversation belongs to (e.g. `GPT3` or `GPT4`). The `weight`
-is assigned as `0` for human messages and `w` for assistant responses, where
-`w` is the weight of the class (e.g. `0.1` for `GPT3` and `1` for `GPT4`, as
-found in our C-RLFT paper). C-RLFT example: ```json {"items":[{"role":
-"user","content":"What is C-RLFT?","weight":0.0},{"role":"assistant","content":
-"C-RLFT is a method for improving open-source LLMs with mixed-quality
-data.","weight":1.0}],"condition":"GPT4","system":""} {"items":[{"role":
-"user","content":"What is C-RLFT?","weight":0.0},{"role":"assistant","content":
-"I don't know.","weight":0.1}],"condition":"GPT3","system":""} ``` ### Pre-
-tokenizing the Dataset You'll then need to pre-tokenize the dataset using the
-command (please specify a filename as `PRETOKENIZED_DATA_OUTPUT_PATH` to store
-the pretokenized dataset): ```bash python -m ochat.data.generate_dataset --
-model-type MODEL_TYPE --model-path BASE_REPO --in-files data.jsonl --out-prefix
-PRETOKENIZED_DATA_OUTPUT_PATH ``` ### Launching the OpenChat Trainer You can
-now launch the OpenChat trainer using the command below. - 13B model requires
-eight `A/H100s` with 80GB VRAM - 7B model can be trained with four `A/H100s`
-with 80GB VRAM or eight `A/H100s` with 40GB VRAM. For hyperparameters, we
-recommend first setting the batch size to the recommended batch size. If OOM
-occurs, try setting it to the exact maximum that VRAM can hold and as a
-multiple of `2048`. Other hyperparameters have been carefully selected as the
-default. Furthermore, the learning rate is automatically determined based on
-the [inverse square-root rule](https://arxiv.org/abs/2006.09092). Training
-Commands (click to expand) ```bash NUM_GPUS=8 deepspeed --num_gpus=$NUM_GPUS --
-module ochat.training_deepspeed.train \ --model_path BASE_REPO \ --data_prefix
+-|--------------------------------------------|-------------------------|------
+----------------------------------------| | Llama 3 | 8B | `imone/Llama-3-8B-
+fixed-special-embedding` | `openchat_3.6` | 40960 | | Mistral | 7B | `imone/
+Mistral_7B_with_EOT_token` | `openchat_v3.2_mistral` | 77824 | Note: The
+OpenChat conversation template requires `<|eot_id|>, <|start_header_id|>,
+<|end_header_id|>` (Llama 3) `<|end_of_turn|>` (Mistral) special tokens. The
+base model specified must include these tokens with initialized embeddings. Our
+provided weights are the original base weights with this token added and
+embeddings initialized. If you want to add them manually, use the
+`init_special_embedding_llama3.py` or `mistral_add_tokens.py` in the `scripts`
+directory. ## Installing DeepSpeed and Flash Attention First, ensure that the
+CUDA `nvcc` compiler is available in your environment. If it is not, install
+the CUDA toolkit that matches the version used by PyTorch. Next, install
+building dependencies: ```bash pip install packaging ninja ``` Finally, install
+the packages: ```bash pip install deepspeed flash-attn ``` ### Preparing Your
+Data To utilize the OpenChat trainer, prepare your SFT data into a JSON Lines
+format where each line corresponds to a `Conversation` object: ```python class
+Message(BaseModel): role: str # Must be "user" or "assistant" content: str #
+Message content weight: Optional[float] = None # Loss weight for this message.
+Typically 0 for user and 1 for assistant to supervise assistant's responses
+only class Conversation(BaseModel): items: List[Message] # All messages within
+the conversation condition: str = "" # C-RLFT condition, can be any string or
+empty. system: str = "" # System message for this conversation ``` For basic
+SFT, assign `weight` as `0` for human messages and `1` for assistant responses.
+SFT example: ```json {"items":[{"role":"user","content":"Hello","weight":0.0},
+{"role":"assistant","content":"Hi","weight":1.0},{"role":"user","content":"How
+are you today?","weight":0.0},{"role":"assistant","content":"I'm
+fine.","weight":1.0}],"system":""} {"items":[{"role":"user","content":"Who are
+you?","weight":0.0},{"role":"assistant","content":"I'm OpenChat.","weight":
+1.0}],"system":"You are a helpful assistant named OpenChat."} ``` For C-RLFT,
+`condition` should be set as the class the conversation belongs to (e.g. `GPT3`
+or `GPT4`). The `weight` is assigned as `0` for human messages and `w` for
+assistant responses, where `w` is the weight of the class (e.g. `0.1` for
+`GPT3` and `1` for `GPT4`, as found in our C-RLFT paper). C-RLFT example:
+```json {"items":[{"role":"user","content":"What is C-RLFT?","weight":0.0},
+{"role":"assistant","content":"C-RLFT is a method for improving open-source
+LLMs with mixed-quality data.","weight":1.0}],"condition":"GPT4","system":""}
+{"items":[{"role":"user","content":"What is C-RLFT?","weight":0.0},{"role":
+"assistant","content":"I don't know.","weight":0.1}],"condition":
+"GPT3","system":""} ``` ### Pre-tokenizing the Dataset You'll then need to pre-
+tokenize the dataset using the command (please specify a filename as
+`PRETOKENIZED_DATA_OUTPUT_PATH` to store the pretokenized dataset): ```bash
+python -m ochat.data.generate_dataset --model-type MODEL_TYPE --model-path
+BASE_REPO --in-files data.jsonl --out-prefix PRETOKENIZED_DATA_OUTPUT_PATH ```
+### Launching the OpenChat Trainer You can now launch the OpenChat trainer
+using the command below. - 13B model requires eight `A/H100s` with 80GB VRAM -
+7B model can be trained with four `A/H100s` with 80GB VRAM or eight `A/H100s`
+with 40GB VRAM. For hyperparameters, we recommend first setting the batch size
+to the recommended batch size. If OOM occurs, try setting it to the exact
+maximum that VRAM can hold and as a multiple of `2048`. Other hyperparameters
+have been carefully selected as the default. Furthermore, the learning rate is
+automatically determined based on the [inverse square-root rule](https://
+arxiv.org/abs/2006.09092). Training Commands (click to expand) ```bash
+NUM_GPUS=8 deepspeed --num_gpus=$NUM_GPUS --module
+ochat.training_deepspeed.train \ --model_path BASE_REPO \ --data_prefix
 PRETOKENIZED_DATA_OUTPUT_PATH \ --save_path PATH_TO_SAVE_MODEL \ --
 batch_max_len BATCH_SIZE \ --epochs 5 \ --save_every 1 \ --deepspeed \ --
 deepspeed_config ochat/training_deepspeed/deepspeed_config.json ``` You can
 find checkpoints of all epochs in `PATH_TO_SAVE_MODEL`. Then you may evaluate
 each epoch and choose the best one. # Limitations ## Foundation Model
 Limitations Despite its advanced capabilities, OpenChat is still bound by the
 limitations inherent in its foundation models. These limitations may impact the
 model's performance in areas such as: - Complex reasoning - Mathematical and
 arithmetic tasks - Programming and coding challenges ## Hallucination of Non-
 existent Information OpenChat may sometimes generate information that does not
 exist or is not accurate, also known as "hallucination". Users should be aware
 of this possibility and verify any critical information obtained the model. ##
 Safety OpenChat may sometimes generate harmful, hate speech, biased responses,
 or answer unsafe questions. It's crucial to apply additional AI safety measures
-in use cases that require safe and moderated responses. # License Our OpenChat
-3.5 `code` and `models` are distributed under the **Apache License 2.0**. #
-Models | Model | Size | Context | Weights | Serving | |--------------|------|--
--------|-------------------------------------------------------------|---------
--------------------------------------------------------------------------------
----------------------| | OpenChat 3.5 0106 | 7B | 8192 | [Huggingface](https://
-huggingface.co/openchat/openchat-3.5-0106) | `python -
-m ochat.serving.openai_api_server --model openchat/openchat-3.5-0106 --engine-
-use-ray --worker-use-ray` | | OpenChat 3.5 1210 | 7B | 8192 | [Huggingface]
-(https://huggingface.co/openchat/openchat-3.5-1210) | `python -
-m ochat.serving.openai_api_server --model openchat/openchat-3.5-1210 --engine-
-use-ray --worker-use-ray` | | OpenChat 3.5 | 7B | 8192 | [Huggingface](https://
-huggingface.co/openchat/openchat_3.5) | `python -
-m ochat.serving.openai_api_server --model openchat/openchat_3.5 --engine-use-
-ray --worker-use-ray` | ## Legacy Models The following models are older
-versions of OpenChat and have inferior performance compared to the latest
-version. They will be deprecated in the next release. Please note that OpenChat
-V1 and V2 series are now deprecated, [please install 3.1.x for using V1 and V2
-models](https://github.com/imoneoi/openchat/tree/
-83a683c775c77867cc45937fafdf48e8dcb68daa) To run the models on multiple GPUs
-with smaller VRAM, you can enable tensor parallelization, for example, using
-the `--tensor-parallel-size 2` flag. | Model | Size | Context | Weights |
-Serving | |--------------|------|---------|------------------------------------
---------------------------|----------------------------------------------------
-----------------------------------------------------------| | OpenChat 3.2
-SUPER | 13B | 4096 | [Huggingface](https://huggingface.co/openchat/
-openchat_v3.2_super) | `python -m ochat.serving.openai_api_server --model
-openchat/openchat_v3.2_super --engine-use-ray --worker-use-ray` | # Citation
-``` @article{wang2023openchat, title={OpenChat: Advancing Open-source Language
-Models with Mixed-Quality Data}, author={Wang, Guan and Cheng, Sijie and Zhan,
-Xianyuan and Li, Xiangang and Song, Sen and Liu, Yang}, journal={arXiv preprint
-arXiv:2309.11235}, year={2023} } ``` # ðContact We are a student team at
-Tsinghua University, working on OpenChat, a project that requires additional
-computing power or LLMs API keys for further development. If you are interested
-in our project and would like to offer support, please feel free to reach out
-to us: **Project Leader:** - Guan Wang [imonenext at gmail dot com] - [Sijie
-Cheng](https://adacheng.github.io/) [csj23 at mails dot tsinghua dot edu dot
-cn] **Main Contributors:** - [Xianyuan Zhan](https://scholar.google.com.hk/
-citations?user=pDMnGloAAAAJ&hl=zh-CN) (Tsinghua University): Provided
-invaluable advice on paper writing. - [Alpay Ariyak](https://github.com/
-alpayariyak): Responsible for data collection, documentation, model cards and
-PR for `openchat-3.5-1210`, `openchat-3.5-0106`. - LDJ: Tasked with partial
-data collection for `openchat-3.5`. **Sponsors:** - [Sen Song](https://
-scholar.google.com/citations?user=cYgtRP4AAAAJ&hl=en) (Tsinghua University),
-[Yang Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University), [01.AI
-Company](https://www.lingyiwanwu.com/en), [RunPod](https://www.runpod.io/),
-Changling Liu (GPT Desk Pte. Ltd.), Qiying Yu (Tsinghua University), AutoMeta
-(Alignment Lab AI). **Special Thanks:** - We express our profound gratitude to
-Alignment Lab AI, Nous Research, and Pygmalion AI for their significant
-contributions to data collection and model training. We also extend our special
-thanks to Xiangang Li, Baochang Ma, and Hao Wan from 01.AI company for their
-generous provision of resources. We also thank Jianxiong Li and Peng Li at
-Tsinghua University for their insightful discussions that have enriched our
-work. - We acknowledge and thank the developers behind these projects:
-[Mistral](https://mistral.ai/), [Chain-of-Thought Hub](https://github.com/
-FranxYao/chain-of-thought-hub), [Llama 2](https://ai.meta.com/llama/), [Self-
-Instruct](https://arxiv.org/abs/2212.10560), [FastChat (Vicuna)](https://
-github.com/lm-sys/FastChat), [Alpaca](https://github.com/tatsu-lab/
-stanford_alpaca.git), and [StarCoder](https://github.com/bigcode-project/
-starcoder). Their work has been instrumental in driving our research forward.
+in use cases that require safe and moderated responses. # License Code is
+distributed under the **Apache License 2.0**. # Citation ``` @article
+{wang2023openchat, title={OpenChat: Advancing Open-source Language Models with
+Mixed-Quality Data}, author={Wang, Guan and Cheng, Sijie and Zhan, Xianyuan and
+Li, Xiangang and Song, Sen and Liu, Yang}, journal={arXiv preprint arXiv:
+2309.11235}, year={2023} } ``` # ðContact **Project Lead:** - Guan Wang
+[imonenext at gmail dot com] - [Alpay Ariyak](https://github.com/alpayariyak)
+[aariyak at wpi dot edu] **Main Contributors:** - [Xianyuan Zhan](https://
+scholar.google.com.hk/citations?user=pDMnGloAAAAJ) (Tsinghua University) -
+Qiying Yu (Tsinghua University) - Changling Liu (GPT Desk Pte. Ltd.) - LDJ -
+AutoMeta (Alignment Lab AI) **Sponsors:** - [Sen Song](https://
+scholar.google.com/citations?user=cYgtRP4AAAAJ) (Tsinghua University) - [Yang
+Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University) - [01.AI
+Company](https://www.lingyiwanwu.com/en) - [RunPod](https://www.runpod.io/
+) **Special Thanks:** - [Mistral](https://mistral.ai/) - [Chain-of-Thought Hub]
+(https://github.com/FranxYao/chain-of-thought-hub) - [Llama 2](https://
+ai.meta.com/llama/) - [Self-Instruct](https://arxiv.org/abs/2212.10560) -
+[FastChat (Vicuna)](https://github.com/lm-sys/FastChat) - [Alpaca](https://
+github.com/tatsu-lab/stanford_alpaca.git) - [StarCoder](https://github.com/
+bigcode-project/starcoder)
```

### Comparing `ochat-3.5.2/SECURITY.md` & `ochat-3.6.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/assets/embeddings.svg` & `ochat-3.6.0/assets/embeddings.svg`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/assets/logo_new.png` & `ochat-3.6.0/assets/logo_new.png`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/assets/openchat-bench-0106.png` & `ochat-3.6.0/assets/openchat-bench-0106.png`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/assets/openchat.png` & `ochat-3.6.0/assets/openchat.png`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/assets/openchat_grok.png` & `ochat-3.6.0/assets/openchat_grok.png`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/assets/vicuna_gpt35.svg` & `ochat-3.6.0/assets/vicuna_gpt35.svg`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/assets/vicuna_gpt4.svg` & `ochat-3.6.0/assets/vicuna_gpt4.svg`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/config/conversation_template.py` & `ochat-3.6.0/ochat/config/conversation_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Callable, Iterable, List, Dict
+from typing import Optional, Callable, Iterable, List
 
 from pydantic import BaseModel
 
 
 class Message(BaseModel):
     role: str
     content: str
@@ -18,50 +18,62 @@
 
 
 class ConversationTemplate(BaseModel):
     tokenizer: Callable
 
     # Prompt
     role_prefix: Callable
+    system_as_role: Optional[bool] = False
     eot: str
 
     inference_condition: Optional[str] = None
 
     # Private
     bos_tokens_: List[int]
     eot_tokens_: List[int]
 
     def __init__(self, **data):
         tokenizer = data["tokenizer"]
         eot = data["eot"]
         bos_tokens_ = tokenizer("").input_ids
         eot_tokens_ = tokenizer(eot, add_special_tokens=False).input_ids
-
         super().__init__(**data, bos_tokens_=bos_tokens_, eot_tokens_=eot_tokens_)
 
     def _tokenize(self, strings: Iterable[str], ignore_special: bool = True) -> List[List[int]]:
-        return self.tokenizer(strings, split_special_tokens=ignore_special, return_attention_mask=False, add_special_tokens=False).input_ids
+        if self.tokenizer.is_fast:
+            # Support for fast tokenizer
+            # https://github.com/huggingface/tokenizers/pull/1419
+            self.tokenizer._tokenizer.encode_special_tokens = ignore_special
+            result = self.tokenizer(strings, return_attention_mask=False, add_special_tokens=False).input_ids
+            self.tokenizer._tokenizer.encode_special_tokens = False
+        else:
+            result = self.tokenizer(strings, split_special_tokens=ignore_special, return_attention_mask=False, add_special_tokens=False).input_ids
+
+        return result
 
     def tokenize_conversations(self, conversations: Iterable[Conversation], inference: bool = False, seq_level_weight: bool = False):
         # Pre-tokenize all conversations
         default_condition = self.inference_condition if inference else ""
 
         sys_mappings = set()
         role_mappings = set()
         all_text = []
         for conv in conversations:
             sys_mappings.add(conv.system)
             for msg in conv.items:
                 role_mappings.add((msg.role, conv.condition or default_condition))
                 all_text.append(msg.content)
 
+        system_role_tokens = []
+        if self.system_as_role:
+            system_role_tokens = self._tokenize(self.role_prefix("system", ""), ignore_special=False)
+        
         sys_mappings = list(sys_mappings)
         role_mappings = list(role_mappings)
 
-        # Tokenize
         sys_mappings = dict(zip(sys_mappings, self._tokenize(sys_mappings)))
         role_mappings = dict(zip(role_mappings, self._tokenize([self.role_prefix(*args) for args in role_mappings], ignore_special=False)))
         all_text = self._tokenize(all_text)
 
         # Convert
         result_tokens = []
         result_weights = []
@@ -72,29 +84,32 @@
 
             # bos tokens
             tokens.extend(self.bos_tokens_)
             weights.extend([0.] * len(self.bos_tokens_))
 
             # System
             if conv.system:
+                tokens.extend(system_role_tokens)
+                weights.extend([0.] * len(system_role_tokens)) 
+                
                 system = sys_mappings[conv.system]
                 tokens.extend(system)
                 weights.extend([0.] * len(system))
 
                 tokens.extend(self.eot_tokens_)
                 weights.extend([0.] * len(self.eot_tokens_))
 
             # Messages
             last_idx = len(conv.items) - 1
             for idx, msg in enumerate(conv.items):
-                # Prefix
+                # Role Prefix
                 role = role_mappings[(msg.role, conv.condition or default_condition)]
                 tokens.extend(role)
                 weights.extend([0.] * len(role))
-
+                
                 # Message
                 text = all_text[all_text_idx]
                 all_text_idx += 1
 
                 # weight
                 w = None
                 if not inference:
```

### Comparing `ochat-3.5.2/ochat/data/generate_dataset.py` & `ochat-3.6.0/ochat/data/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/conv_eval.py` & `ochat-3.6.0/ochat/evaluation/conv_eval.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/convert_to_evalplus.py` & `ochat-3.6.0/ochat/evaluation/convert_to_evalplus.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/coding/humaneval/humaneval.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/coding/humaneval/humaneval.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/abstract_algebra.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/abstract_algebra.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/anatomy.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/anatomy.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/astronomy.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/astronomy.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/business_ethics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/business_ethics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/clinical_knowledge.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/clinical_knowledge.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_biology.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_biology.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_chemistry.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_chemistry.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_computer_science.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_computer_science.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_mathematics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_mathematics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_medicine.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_medicine.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/college_physics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/college_physics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/computer_security.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/computer_security.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/conceptual_physics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/conceptual_physics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/econometrics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/econometrics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/electrical_engineering.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/electrical_engineering.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/elementary_mathematics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/elementary_mathematics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/formal_logic.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/formal_logic.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/global_facts.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/global_facts.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_biology.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_biology.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_chemistry.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_chemistry.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_computer_science.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_computer_science.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_european_history.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_european_history.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_geography.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_geography.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_government_and_politics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_government_and_politics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_macroeconomics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_macroeconomics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_mathematics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_mathematics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_microeconomics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_microeconomics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_physics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_physics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_psychology.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_psychology.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_statistics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_statistics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_us_history.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_us_history.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_world_history.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/high_school_world_history.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/human_aging.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/human_aging.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/human_sexuality.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/human_sexuality.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/international_law.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/international_law.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/jurisprudence.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/jurisprudence.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/logical_fallacies.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/logical_fallacies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/machine_learning.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/machine_learning.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/management.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/management.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/marketing.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/marketing.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/medical_genetics.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/medical_genetics.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/miscellaneous.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/miscellaneous.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/moral_disputes.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/moral_disputes.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/moral_scenarios.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/moral_scenarios.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/nutrition.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/nutrition.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/philosophy.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/philosophy.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/prehistory.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/prehistory.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_accounting.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_accounting.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_law.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_law.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_medicine.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_medicine.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_psychology.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/professional_psychology.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/public_relations.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/public_relations.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/security_studies.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/security_studies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/sociology.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/sociology.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/us_foreign_policy.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/us_foreign_policy.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/virology.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/virology.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/fs_cothub/mmlu/world_religions.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/fs_cothub/mmlu/world_religions.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/math/MATH.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/math/MATH.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl` & `ochat-3.6.0/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/grading/math_grader.py` & `ochat-3.6.0/ochat/evaluation/grading/math_grader.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/grading/math_normalize.py` & `ochat-3.6.0/ochat/evaluation/grading/math_normalize.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/evaluation/match_answer.py` & `ochat-3.6.0/ochat/evaluation/match_answer.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     for c in response:
         if c in task_data["options"]:
             return True, c
 
     return False, ""
 
 
-def zs_math_match_answer(task_data, response):
+def zs_math_match_answer(task_data, response, max_length=256):
     def _last_boxed_only_string(string):
         idx = string.rfind("\\boxed")
         if idx < 0:
             idx = string.rfind("\\fbox")
             if idx < 0:
                 return None
 
@@ -79,17 +79,35 @@
     # Find boxed
     ans_boxed = _last_boxed_only_string(response)
     if ans_boxed:
         is_matched = True
         response = ans_boxed
 
     # Grade
+    response = response[:max_length]  # To avoid sympy taking too long
     return is_matched, grade_answer(response, ground_truth_answer)
 
 
+def zs_gpqa_match_answer(task_data, response):
+    # Expected to see answer field, otherwise return C.
+    ans = response.split("The correct answer is")
+
+    if len(ans) == 1:
+        return False, "C"
+
+    ans = ans[1]
+
+    letter_set = {"A", "B", "C", "D"} 
+    for c in ans:
+        if c in letter_set:
+            return True, c
+
+    return False, "C"
+
+
 def fs_cothub_bbh_match_answer(task_data, response):
     # CoT hub match answer for BBH
     # https://github.com/FranxYao/chain-of-thought-hub/blob/main/BBH/run_bbh_gpt_3.5_turbo.py
 
     ans_line = response.split('answer is ')
 
     # Expect to see 'answer is'. If not return whole string
@@ -185,14 +203,15 @@
 
 
 MATCH_ANSWER_FUNCTION = {
     "zs/agieval": zs_agieval_match_answer,
     "zs/bbh_mc_orca": zs_bbh_mc_orca_truthfulqa_orca_match_answer,
     "zs/truthfulqa_orca": zs_bbh_mc_orca_truthfulqa_orca_match_answer,
     "zs/math": zs_math_match_answer,
+    "zs/gpqa": zs_gpqa_match_answer,
 
     "fs_cothub/bbh": fs_cothub_bbh_match_answer,
     "fs_cothub/gsm8k": fs_cothub_gsm8k_match_answer,
     "fs_cothub/mmlu": fs_cothub_mmlu_match_answer,
 
     "coding/humaneval": coding_humaneval_match_answer
 }
```

### Comparing `ochat-3.5.2/ochat/evaluation/run_eval.py` & `ochat-3.6.0/ochat/evaluation/run_eval.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import asyncio
 from glob import glob
 
 import orjson
 import openai
 from tqdm import tqdm
-from openai.error import RateLimitError, ServiceUnavailableError
+from openai import RateLimitError, InternalServerError, APIConnectionError
 from tenacity import retry, stop_after_attempt, wait_random_exponential, retry_if_exception_type
 from vllm import LLM, SamplingParams
 
 from transformers.utils.hub import cached_file
 
 from ochat.evaluation.match_answer import MATCH_ANSWER_FUNCTION
 from ochat.config import MODEL_CONFIG_MAP
@@ -19,36 +19,39 @@
 
 def _strip_first_space(s: str):
     if len(s) and s[0] == " ":
         return s[1:]
     return s
 
 
-@retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(20), retry=retry_if_exception_type((RateLimitError, ServiceUnavailableError, )))
-async def _chat_completion_with_backoff(**kwargs):
-    return await openai.ChatCompletion.acreate(**kwargs)
+@retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(20), retry=retry_if_exception_type((RateLimitError, InternalServerError, APIConnectionError, )))
+async def _chat_completion_with_backoff(client, **kwargs):
+    return await client.chat.completions.create(**kwargs)
 
 
 async def chat_completion_thread(model, progress_bar, queue):
+    client = openai.AsyncOpenAI()
+
     while True:
         # Fetch task
         try:
             task = queue.get_nowait()
         except asyncio.QueueEmpty:
             break
 
         # Completion
         try:
             response = await _chat_completion_with_backoff(
+                client,
                 model=model,
                 messages=[{"role": "user", "content": task["question"]}],
 
                 temperature=0
             )
-            task["response"] = response["choices"][0]["message"]["content"]  # type: ignore
+            task["response"] = response.choices[0].message.content  # type: ignore
         except Exception as e:
             if hasattr(e, "last_attempt"):
                 e = e.last_attempt
             if hasattr(e, "_exception"):
                 e = e._exception
 
             print(type(e), str(e))
@@ -233,19 +236,19 @@
 
     # Input / output
     parser.add_argument("--model", type=str, default=None)
     parser.add_argument("--condition", type=str, default="")
     parser.add_argument("--system-msg", type=str, default="")
     parser.add_argument("--model-type", type=str, default=None)
 
-    parser.add_argument("--data_path", type=str, default="ochat/evaluation/eval_data")
-    parser.add_argument("--eval_sets", type=str, nargs="+", default=[])
+    parser.add_argument("--data-path", type=str, default="ochat/evaluation/eval_data")
+    parser.add_argument("--eval-sets", type=str, nargs="+", default=[])
 
-    parser.add_argument("--continue_from", type=str, default=None)
-    parser.add_argument("--output_file",   type=str, default=None)
+    parser.add_argument("--continue-from", type=str, default=None)
+    parser.add_argument("--output-file",   type=str, default=None)
     parser.add_argument("--parallel",      type=int, default=16)
     parser.add_argument("--tensor-parallel-size", type=int, default=1)
 
     args = parser.parse_args()
 
     await run_eval(**vars(args))
```

### Comparing `ochat-3.5.2/ochat/evaluation/view_results.py` & `ochat-3.6.0/ochat/evaluation/view_results.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,50 +2,58 @@
 import os
 from pathlib import Path
 
 import orjson
 import pandas as pd
 from glob import glob
 
-
+def save_results(dfs, save_path: str):
+    os.makedirs(os.path.dirname(save_path), exist_ok=True)
+    with pd.ExcelWriter(save_path) as writer:
+        for task_type, df_task in dfs.items():
+            df_task.to_excel(writer, sheet_name=task_type)
+                
 def view_results(result_path: str):
     # Read results
     eval_results = []
     for filename in glob(os.path.join(result_path, "*.json")):
         with open(filename, "rb") as f:
             questions = orjson.loads(f.read())
 
             eval_results.extend([{
                 "model": Path(filename).stem,
                 "task_type": q["task_type"],
                 "task_name": os.path.relpath(q["task_name"], q["task_type"]),
                 "accuracy": q["is_correct"],
                 "unmatched": not q["is_matched"],
             } for q in questions])
-
     df = pd.DataFrame.from_records(eval_results)
-
+    all_tables = dict()    
     # Overall metrics table
     df_overall = df.pivot_table(index=["model"], columns=["task_type"], values=["accuracy", "unmatched"], aggfunc="mean")
+    all_tables["overall"] = df_overall
     print(df_overall.to_string(float_format=lambda x: f"{x * 100:.1f}", na_rep="-"))
-
     # Print tables for each task
     for task_type in df["task_type"].unique():
         df_task = df[df["task_type"] == task_type].pivot_table(index=["task_name"], columns=["model"], values=["accuracy", "unmatched"], aggfunc="mean")
-
+        all_tables[task_type.replace("/", "_")] = df_task
         print(f"\n### {task_type}\n")
         print(df_task.to_string(float_format=lambda x: f"{x * 100:.1f}", na_rep="-"))
+    return all_tables
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     # Input / output
     parser.add_argument("--result_path", type=str, default="ochat/evaluation/eval_results")
-
+    parser.add_argument("--save_path", type=str, default="ochat/evaluation/eval_results/summary.xlsx")
+    parser.add_argument("--save", "-s", action="store_true", help="Save the results to a file")
     args = parser.parse_args()
-
-    view_results(**vars(args))
+    
+    all_tables = view_results(args.result_path)
+    if args.save:
+        save_results(all_tables, args.save_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ochat-3.5.2/ochat/experimental/generate_dataset_old.py` & `ochat-3.6.0/ochat/experimental/generate_dataset_old.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/experimental/sharegpt.ipynb` & `ochat-3.6.0/ochat/experimental/sharegpt.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/experimental/test_multipack_dataloader.ipynb` & `ochat-3.6.0/ochat/experimental/test_multipack_dataloader.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/experimental/text_length.ipynb` & `ochat-3.6.0/ochat/experimental/text_length.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/experimental/train_alpaca.py` & `ochat-3.6.0/ochat/experimental/train_alpaca.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/experimental/verify_dataset.ipynb` & `ochat-3.6.0/ochat/experimental/verify_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/experimental/verify_dataset_orca.ipynb` & `ochat-3.6.0/ochat/experimental/verify_dataset_orca.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/models/unpadded_gemma.py` & `ochat-3.6.0/ochat/models/unpadded_gemma.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/models/unpadded_llama.py` & `ochat-3.6.0/ochat/models/unpadded_mistral.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" PyTorch Unpadded & Fused LLaMA model. Compatible with HF. """
+""" PyTorch Unpadded & Fused Mistral model. Compatible with HF. """
 
 from typing import Optional, Tuple
 
 import torch
 import torch.utils.checkpoint
 from torch import nn
 
 from transformers.activations import ACT2FN
 from transformers.modeling_outputs import CausalLMOutputWithPast
 from transformers.modeling_utils import PreTrainedModel
 from transformers.utils import logging
-from transformers.models.llama.configuration_llama import LlamaConfig
+from transformers.models.mistral.configuration_mistral import MistralConfig
 
 try:
     from flash_attn.flash_attn_interface import flash_attn_varlen_func
     from flash_attn.bert_padding import pad_input
 except ImportError:
     print ("FlashAttention not found. Install it if you need to train models.")
 
@@ -65,30 +65,31 @@
     cos = cos[position_ids].unsqueeze(-2)  # [nnz, 1, head_dim]
     sin = sin[position_ids].unsqueeze(-2)  # [nnz, 1, head_dim]
     q_embed = (q * cos) + (rotate_half(q) * sin)
     k_embed = (k * cos) + (rotate_half(k) * sin)
     return q_embed, k_embed
 
 
+# Copied from transformers.models.llama.modeling_llama.LlamaRMSNorm with Llama->Mistral
 RMS_NORM_TRACED = None
 
 
 def rms_norm(hidden_states: torch.Tensor, weight: torch.Tensor, variance_epsilon: torch.Tensor):
     input_dtype = hidden_states.dtype
     hidden_states = hidden_states.to(torch.float32)
 
     variance = (hidden_states * hidden_states).mean(-1, keepdim=True)
     hidden_states = hidden_states * torch.rsqrt(variance + variance_epsilon)
     return weight * hidden_states.to(input_dtype)
 
 
-class UnpaddedLlamaRMSNorm(nn.Module):
+class UnpaddedMistralRMSNorm(nn.Module):
     def __init__(self, hidden_size, eps):
         """
-        UnpaddedLlamaRMSNorm is equivalent to T5LayerNorm
+        UnpaddedMistralRMSNorm is equivalent to T5LayerNorm
         """
         super().__init__()
 
         self.weight = nn.Parameter(torch.ones(hidden_size))
         self.variance_epsilon = torch.tensor(eps, dtype=torch.get_default_dtype())
 
         global RMS_NORM_TRACED
@@ -96,15 +97,16 @@
             RMS_NORM_TRACED = torch.jit.trace(rms_norm, (torch.ones(hidden_size), torch.ones(hidden_size), self.variance_epsilon))
 
     def forward(self, hidden_states):
         global RMS_NORM_TRACED
         return RMS_NORM_TRACED(hidden_states, self.weight, self.variance_epsilon)
 
 
-class UnpaddedLlamaRotaryEmbedding(torch.nn.Module):
+# Copied from transformers.models.llama.modeling_llama.LlamaRotaryEmbedding with Llama->Mistral
+class UnpaddedMistralRotaryEmbedding(torch.nn.Module):
     def __init__(self, dim, max_position_embeddings, base, device=None):
         super().__init__()
 
         # RoPE
         inv_freq = 1.0 / (base ** (torch.arange(0, dim, 2, dtype=torch.float32, device=device) / dim))
         t = torch.arange(max_position_embeddings, dtype=torch.float32, device=device)
         freqs = torch.outer(t, inv_freq)
@@ -115,41 +117,41 @@
         self.register_buffer("cos_cached", emb.cos().to(dtype), persistent=False)
         self.register_buffer("sin_cached", emb.sin().to(dtype), persistent=False)
 
     def forward(self):
         return self.cos_cached, self.sin_cached
 
 
-class UnpaddedLlamaMLP(nn.Module):
-    def __init__(
-        self,
-        hidden_size: int,
-        intermediate_size: int,
-        hidden_act: str,
-    ):
+class UnpaddedMistralMLP(nn.Module):
+    def __init__(self, config: MistralConfig):
         super().__init__()
-        self.gate_proj = nn.Linear(hidden_size, intermediate_size, bias=False)
-        self.down_proj = nn.Linear(intermediate_size, hidden_size, bias=False)
-        self.up_proj = nn.Linear(hidden_size, intermediate_size, bias=False)
-        self.act_fn = ACT2FN[hidden_act]
+
+        self.hidden_size = config.hidden_size
+        self.intermediate_size = config.intermediate_size
+
+        self.gate_proj = nn.Linear(self.hidden_size, self.intermediate_size, bias=False)
+        self.up_proj = nn.Linear(self.hidden_size, self.intermediate_size, bias=False)
+        self.down_proj = nn.Linear(self.intermediate_size, self.hidden_size, bias=False)
+        self.act_fn = ACT2FN[config.hidden_act]
 
     def forward(self, x):
         return self.down_proj(self.act_fn(self.gate_proj(x)) * self.up_proj(x))
 
 
-class UnpaddedLlamaAttention(nn.Module):
+class UnpaddedMistralAttention(nn.Module):
     """Multi-headed attention from 'Attention Is All You Need' paper"""
 
-    def __init__(self, config: LlamaConfig):
+    def __init__(self, config: MistralConfig):
         super().__init__()
 
         self.hidden_size = config.hidden_size
         self.num_heads = config.num_attention_heads
         self.head_dim = self.hidden_size // self.num_heads
         self.num_key_value_heads = config.num_key_value_heads
+        self.sliding_window = config.sliding_window
 
         if (self.head_dim * self.num_heads) != self.hidden_size:
             raise ValueError(
                 f"hidden_size must be divisible by num_heads (got `hidden_size`: {self.hidden_size}"
                 f" and `num_heads`: {self.num_heads})."
             )
 
@@ -180,34 +182,32 @@
         query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, nz_position_ids)
 
         # flash attn
         attn_output = flash_attn_varlen_func(
             q=query_states, k=key_states, v=value_states,
             cu_seqlens_q=cu_seqlens, cu_seqlens_k=cu_seqlens,
             max_seqlen_q=max_seqlen, max_seqlen_k=max_seqlen,
-            dropout_p=0.0, causal=True)
+
+            dropout_p=0.0, causal=True,
+            window_size=(self.sliding_window, self.sliding_window))
 
         # attn_output: [total_nnz, num_heads, head_dim]
         attn_output = attn_output.view(-1, self.hidden_size)  # type: ignore
         return self.o_proj(attn_output)
 
 
-class UnpaddedLlamaDecoderLayer(nn.Module):
-    def __init__(self, config: LlamaConfig):
+class UnpaddedMistralDecoderLayer(nn.Module):
+    def __init__(self, config: MistralConfig):
         super().__init__()
 
         self.hidden_size = config.hidden_size
-        self.self_attn = UnpaddedLlamaAttention(config=config)
-        self.mlp = UnpaddedLlamaMLP(
-            hidden_size=self.hidden_size,
-            intermediate_size=config.intermediate_size,
-            hidden_act=config.hidden_act,
-        )
-        self.input_layernorm = UnpaddedLlamaRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
-        self.post_attention_layernorm = UnpaddedLlamaRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
+        self.self_attn = UnpaddedMistralAttention(config=config)
+        self.mlp = UnpaddedMistralMLP(config=config)
+        self.input_layernorm = UnpaddedMistralRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
+        self.post_attention_layernorm = UnpaddedMistralRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
     def forward(
         self,
         cos_sin: Tuple[torch.Tensor, torch.Tensor],
         # Unpadded inputs
         nz_hidden_states: torch.Tensor,
         nz_position_ids: torch.Tensor,
@@ -234,52 +234,52 @@
         nz_hidden_states = self.post_attention_layernorm(nz_hidden_states)
         nz_hidden_states = self.mlp(nz_hidden_states)
         nz_hidden_states = residual + nz_hidden_states
 
         return nz_hidden_states
 
 
-class UnpaddedLlamaPreTrainedModel(PreTrainedModel):
-    config_class = LlamaConfig
+class UnpaddedMistralPreTrainedModel(PreTrainedModel):
+    config_class = MistralConfig
     base_model_prefix = "model"
     supports_gradient_checkpointing = True
-    _no_split_modules = ["UnpaddedLlamaDecoderLayer"]
+    _no_split_modules = ["UnpaddedMistralDecoderLayer"]
 
     def _init_weights(self, module):
         std = self.config.initializer_range
         if isinstance(module, nn.Linear):
             module.weight.data.normal_(mean=0.0, std=std)
             if module.bias is not None:
                 module.bias.data.zero_()
         elif isinstance(module, nn.Embedding):
             module.weight.data.normal_(mean=0.0, std=std)
             if module.padding_idx is not None:
                 module.weight.data[module.padding_idx].zero_()
 
 
-class UnpaddedLlamaModel(UnpaddedLlamaPreTrainedModel):
+class UnpaddedMistralModel(UnpaddedMistralPreTrainedModel):
     """
-    Transformer decoder consisting of *config.num_hidden_layers* layers. Each layer is a [`UnpaddedLlamaDecoderLayer`]
+    Transformer decoder consisting of *config.num_hidden_layers* layers. Each layer is a [`UnpaddedMistralDecoderLayer`]
 
     Args:
-        config: LlamaConfig
+        config: MistralConfig
     """
 
-    def __init__(self, config: LlamaConfig):
+    def __init__(self, config: MistralConfig):
         super().__init__(config)
         self.padding_idx = config.pad_token_id
         self.vocab_size = config.vocab_size
 
         self.embed_tokens = nn.Embedding(config.vocab_size, config.hidden_size, self.padding_idx)
-        self.rotary_emb   = UnpaddedLlamaRotaryEmbedding(config.hidden_size // config.num_attention_heads,
+        self.rotary_emb   = UnpaddedMistralRotaryEmbedding(config.hidden_size // config.num_attention_heads,
                                                          max_position_embeddings=config.max_position_embeddings,
                                                          base=config.rope_theta)
 
-        self.layers = nn.ModuleList([UnpaddedLlamaDecoderLayer(config) for _ in range(config.num_hidden_layers)])
-        self.norm = UnpaddedLlamaRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
+        self.layers = nn.ModuleList([UnpaddedMistralDecoderLayer(config) for _ in range(config.num_hidden_layers)])
+        self.norm = UnpaddedMistralRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
         self.gradient_checkpointing = False
         # Initialize weights and apply final processing
         self.post_init()
 
     def get_input_embeddings(self):
         return self.embed_tokens
@@ -321,21 +321,18 @@
                 )
 
         nz_hidden_states = self.norm(nz_hidden_states)
 
         return nz_hidden_states
 
 
-class LlamaForCausalLM(UnpaddedLlamaPreTrainedModel):
-    # Ignore rotary emb inv_freq on load, as they will be calculated on creation
-    _keys_to_ignore_on_load_unexpected = [r"model\.layers\.\d+\.self_attn\.rotary_emb\.inv_freq"]
-
+class MistralForCausalLM(UnpaddedMistralPreTrainedModel):
     def __init__(self, config):
         super().__init__(config)
-        self.model = UnpaddedLlamaModel(config)
+        self.model = UnpaddedMistralModel(config)
 
         self.lm_head = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def get_input_embeddings(self):
@@ -385,15 +382,15 @@
 
         return CausalLMOutputWithPast(
             loss=loss,  # type: ignore
             logits=logits
         )
 
 
-class PaddedLlamaForCausalLM(LlamaForCausalLM):
+class PaddedMistralForCausalLM(MistralForCausalLM):
     """Compat layer for padded inputs"""
 
     def forward(
         self,
         input_ids: torch.Tensor,
         attention_mask: torch.Tensor,
         position_ids: Optional[torch.Tensor] = None,
```

### Comparing `ochat-3.5.2/ochat/models/unpadded_mistral.py` & `ochat-3.6.0/ochat/models/unpadded_llama.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,46 +13,43 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" PyTorch Unpadded & Fused Mistral model. Compatible with HF. """
+""" PyTorch Unpadded & Fused LLaMA model. Compatible with HF. """
 
 from typing import Optional, Tuple
 
 import torch
 import torch.utils.checkpoint
+import torch.nn.functional as F
 from torch import nn
 
 from transformers.activations import ACT2FN
 from transformers.modeling_outputs import CausalLMOutputWithPast
 from transformers.modeling_utils import PreTrainedModel
 from transformers.utils import logging
-from transformers.models.mistral.configuration_mistral import MistralConfig
+from transformers.models.llama.configuration_llama import LlamaConfig
 
 try:
     from flash_attn.flash_attn_interface import flash_attn_varlen_func
     from flash_attn.bert_padding import pad_input
 except ImportError:
     print ("FlashAttention not found. Install it if you need to train models.")
 
 
-logger = logging.get_logger(__name__)
-
-
-@torch.jit.script  # type: ignore
-def weighted_token_accuracy(logits: torch.Tensor, labels: torch.Tensor, weights: torch.Tensor):
-    return (weights * (torch.argmax(logits, dim=-1) == labels)).sum()
-
-
-@torch.jit.script  # type: ignore
-def weighted_cross_entropy(logits: torch.Tensor, labels: torch.Tensor, weights: torch.Tensor):
-    return (weights * torch.nn.functional.cross_entropy(logits, labels, reduction="none")).sum()
+@torch.jit.script
+def lm_head_with_loss(embed_weights: torch.Tensor, hidden_states: torch.Tensor, nz_shifted_label_ids: torch.Tensor, nz_shifted_loss_weights: torch.Tensor):
+    logits = F.linear(hidden_states, embed_weights)
+
+    loss = (nz_shifted_loss_weights * torch.nn.functional.cross_entropy(logits, nz_shifted_label_ids, reduction="none")).sum()
+    token_accuracy = (nz_shifted_loss_weights * (torch.argmax(logits.detach(), dim=-1) == nz_shifted_label_ids)).sum()
+    return loss, token_accuracy
 
 
 def rotate_half(x: torch.Tensor):
     """Rotates half the hidden dims of the input."""
     x1 = x[..., : x.shape[-1] // 2]
     x2 = x[..., x.shape[-1] // 2 :]
     return torch.cat((-x2, x1), dim=-1)
@@ -65,31 +62,30 @@
     cos = cos[position_ids].unsqueeze(-2)  # [nnz, 1, head_dim]
     sin = sin[position_ids].unsqueeze(-2)  # [nnz, 1, head_dim]
     q_embed = (q * cos) + (rotate_half(q) * sin)
     k_embed = (k * cos) + (rotate_half(k) * sin)
     return q_embed, k_embed
 
 
-# Copied from transformers.models.llama.modeling_llama.LlamaRMSNorm with Llama->Mistral
 RMS_NORM_TRACED = None
 
 
 def rms_norm(hidden_states: torch.Tensor, weight: torch.Tensor, variance_epsilon: torch.Tensor):
     input_dtype = hidden_states.dtype
     hidden_states = hidden_states.to(torch.float32)
 
     variance = (hidden_states * hidden_states).mean(-1, keepdim=True)
     hidden_states = hidden_states * torch.rsqrt(variance + variance_epsilon)
     return weight * hidden_states.to(input_dtype)
 
 
-class UnpaddedMistralRMSNorm(nn.Module):
+class UnpaddedLlamaRMSNorm(nn.Module):
     def __init__(self, hidden_size, eps):
         """
-        UnpaddedMistralRMSNorm is equivalent to T5LayerNorm
+        UnpaddedLlamaRMSNorm is equivalent to T5LayerNorm
         """
         super().__init__()
 
         self.weight = nn.Parameter(torch.ones(hidden_size))
         self.variance_epsilon = torch.tensor(eps, dtype=torch.get_default_dtype())
 
         global RMS_NORM_TRACED
@@ -97,16 +93,15 @@
             RMS_NORM_TRACED = torch.jit.trace(rms_norm, (torch.ones(hidden_size), torch.ones(hidden_size), self.variance_epsilon))
 
     def forward(self, hidden_states):
         global RMS_NORM_TRACED
         return RMS_NORM_TRACED(hidden_states, self.weight, self.variance_epsilon)
 
 
-# Copied from transformers.models.llama.modeling_llama.LlamaRotaryEmbedding with Llama->Mistral
-class UnpaddedMistralRotaryEmbedding(torch.nn.Module):
+class UnpaddedLlamaRotaryEmbedding(torch.nn.Module):
     def __init__(self, dim, max_position_embeddings, base, device=None):
         super().__init__()
 
         # RoPE
         inv_freq = 1.0 / (base ** (torch.arange(0, dim, 2, dtype=torch.float32, device=device) / dim))
         t = torch.arange(max_position_embeddings, dtype=torch.float32, device=device)
         freqs = torch.outer(t, inv_freq)
@@ -117,41 +112,41 @@
         self.register_buffer("cos_cached", emb.cos().to(dtype), persistent=False)
         self.register_buffer("sin_cached", emb.sin().to(dtype), persistent=False)
 
     def forward(self):
         return self.cos_cached, self.sin_cached
 
 
-class UnpaddedMistralMLP(nn.Module):
-    def __init__(self, config: MistralConfig):
+class UnpaddedLlamaMLP(nn.Module):
+    def __init__(
+        self,
+        hidden_size: int,
+        intermediate_size: int,
+        hidden_act: str,
+    ):
         super().__init__()
-
-        self.hidden_size = config.hidden_size
-        self.intermediate_size = config.intermediate_size
-
-        self.gate_proj = nn.Linear(self.hidden_size, self.intermediate_size, bias=False)
-        self.up_proj = nn.Linear(self.hidden_size, self.intermediate_size, bias=False)
-        self.down_proj = nn.Linear(self.intermediate_size, self.hidden_size, bias=False)
-        self.act_fn = ACT2FN[config.hidden_act]
+        self.gate_proj = nn.Linear(hidden_size, intermediate_size, bias=False)
+        self.down_proj = nn.Linear(intermediate_size, hidden_size, bias=False)
+        self.up_proj = nn.Linear(hidden_size, intermediate_size, bias=False)
+        self.act_fn = ACT2FN[hidden_act]
 
     def forward(self, x):
         return self.down_proj(self.act_fn(self.gate_proj(x)) * self.up_proj(x))
 
 
-class UnpaddedMistralAttention(nn.Module):
+class UnpaddedLlamaAttention(nn.Module):
     """Multi-headed attention from 'Attention Is All You Need' paper"""
 
-    def __init__(self, config: MistralConfig):
+    def __init__(self, config: LlamaConfig):
         super().__init__()
 
         self.hidden_size = config.hidden_size
         self.num_heads = config.num_attention_heads
         self.head_dim = self.hidden_size // self.num_heads
         self.num_key_value_heads = config.num_key_value_heads
-        self.sliding_window = config.sliding_window
 
         if (self.head_dim * self.num_heads) != self.hidden_size:
             raise ValueError(
                 f"hidden_size must be divisible by num_heads (got `hidden_size`: {self.hidden_size}"
                 f" and `num_heads`: {self.num_heads})."
             )
 
@@ -182,32 +177,34 @@
         query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, nz_position_ids)
 
         # flash attn
         attn_output = flash_attn_varlen_func(
             q=query_states, k=key_states, v=value_states,
             cu_seqlens_q=cu_seqlens, cu_seqlens_k=cu_seqlens,
             max_seqlen_q=max_seqlen, max_seqlen_k=max_seqlen,
-
-            dropout_p=0.0, causal=True,
-            window_size=(self.sliding_window, self.sliding_window))
+            dropout_p=0.0, causal=True)
 
         # attn_output: [total_nnz, num_heads, head_dim]
         attn_output = attn_output.view(-1, self.hidden_size)  # type: ignore
         return self.o_proj(attn_output)
 
 
-class UnpaddedMistralDecoderLayer(nn.Module):
-    def __init__(self, config: MistralConfig):
+class UnpaddedLlamaDecoderLayer(nn.Module):
+    def __init__(self, config: LlamaConfig):
         super().__init__()
 
         self.hidden_size = config.hidden_size
-        self.self_attn = UnpaddedMistralAttention(config=config)
-        self.mlp = UnpaddedMistralMLP(config=config)
-        self.input_layernorm = UnpaddedMistralRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
-        self.post_attention_layernorm = UnpaddedMistralRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
+        self.self_attn = UnpaddedLlamaAttention(config=config)
+        self.mlp = UnpaddedLlamaMLP(
+            hidden_size=self.hidden_size,
+            intermediate_size=config.intermediate_size,
+            hidden_act=config.hidden_act,
+        )
+        self.input_layernorm = UnpaddedLlamaRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
+        self.post_attention_layernorm = UnpaddedLlamaRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
     def forward(
         self,
         cos_sin: Tuple[torch.Tensor, torch.Tensor],
         # Unpadded inputs
         nz_hidden_states: torch.Tensor,
         nz_position_ids: torch.Tensor,
@@ -234,52 +231,52 @@
         nz_hidden_states = self.post_attention_layernorm(nz_hidden_states)
         nz_hidden_states = self.mlp(nz_hidden_states)
         nz_hidden_states = residual + nz_hidden_states
 
         return nz_hidden_states
 
 
-class UnpaddedMistralPreTrainedModel(PreTrainedModel):
-    config_class = MistralConfig
+class UnpaddedLlamaPreTrainedModel(PreTrainedModel):
+    config_class = LlamaConfig
     base_model_prefix = "model"
     supports_gradient_checkpointing = True
-    _no_split_modules = ["UnpaddedMistralDecoderLayer"]
+    _no_split_modules = ["UnpaddedLlamaDecoderLayer"]
 
     def _init_weights(self, module):
         std = self.config.initializer_range
         if isinstance(module, nn.Linear):
             module.weight.data.normal_(mean=0.0, std=std)
             if module.bias is not None:
                 module.bias.data.zero_()
         elif isinstance(module, nn.Embedding):
             module.weight.data.normal_(mean=0.0, std=std)
             if module.padding_idx is not None:
                 module.weight.data[module.padding_idx].zero_()
 
 
-class UnpaddedMistralModel(UnpaddedMistralPreTrainedModel):
+class UnpaddedLlamaModel(UnpaddedLlamaPreTrainedModel):
     """
-    Transformer decoder consisting of *config.num_hidden_layers* layers. Each layer is a [`UnpaddedMistralDecoderLayer`]
+    Transformer decoder consisting of *config.num_hidden_layers* layers. Each layer is a [`UnpaddedLlamaDecoderLayer`]
 
     Args:
-        config: MistralConfig
+        config: LlamaConfig
     """
 
-    def __init__(self, config: MistralConfig):
+    def __init__(self, config: LlamaConfig):
         super().__init__(config)
         self.padding_idx = config.pad_token_id
         self.vocab_size = config.vocab_size
 
         self.embed_tokens = nn.Embedding(config.vocab_size, config.hidden_size, self.padding_idx)
-        self.rotary_emb   = UnpaddedMistralRotaryEmbedding(config.hidden_size // config.num_attention_heads,
+        self.rotary_emb   = UnpaddedLlamaRotaryEmbedding(config.hidden_size // config.num_attention_heads,
                                                          max_position_embeddings=config.max_position_embeddings,
                                                          base=config.rope_theta)
 
-        self.layers = nn.ModuleList([UnpaddedMistralDecoderLayer(config) for _ in range(config.num_hidden_layers)])
-        self.norm = UnpaddedMistralRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
+        self.layers = nn.ModuleList([UnpaddedLlamaDecoderLayer(config) for _ in range(config.num_hidden_layers)])
+        self.norm = UnpaddedLlamaRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
         self.gradient_checkpointing = False
         # Initialize weights and apply final processing
         self.post_init()
 
     def get_input_embeddings(self):
         return self.embed_tokens
@@ -321,18 +318,21 @@
                 )
 
         nz_hidden_states = self.norm(nz_hidden_states)
 
         return nz_hidden_states
 
 
-class MistralForCausalLM(UnpaddedMistralPreTrainedModel):
+class LlamaForCausalLM(UnpaddedLlamaPreTrainedModel):
+    # Ignore rotary emb inv_freq on load, as they will be calculated on creation
+    _keys_to_ignore_on_load_unexpected = [r"model\.layers\.\d+\.self_attn\.rotary_emb\.inv_freq"]
+
     def __init__(self, config):
         super().__init__(config)
-        self.model = UnpaddedMistralModel(config)
+        self.model = UnpaddedLlamaModel(config)
 
         self.lm_head = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def get_input_embeddings(self):
@@ -367,71 +367,20 @@
         # Model logits
         hidden_states = self.model(
             nz_input_ids=nz_input_ids,
             nz_position_ids=nz_position_ids,
             cu_seqlens=cu_seqlens,
             max_seqlen=max_seqlen
         )
-        logits = self.lm_head(hidden_states)
-
-        loss = None
-        if nz_shifted_label_ids is not None:
-            assert nz_shifted_loss_weights is not None
 
-            loss = weighted_cross_entropy(logits, nz_shifted_label_ids, nz_shifted_loss_weights), \
-                   weighted_token_accuracy(logits.detach(), nz_shifted_label_ids, nz_shifted_loss_weights)
+        # Loss
+        # Fused LMHead with loss
+        loss = lm_head_with_loss(
+            self.lm_head.weight,
+            hidden_states,
+            nz_shifted_label_ids,
+            nz_shifted_loss_weights
+        )
 
         return CausalLMOutputWithPast(
-            loss=loss,  # type: ignore
-            logits=logits
+            loss=loss  # type: ignore
         )
-
-
-class PaddedMistralForCausalLM(MistralForCausalLM):
-    """Compat layer for padded inputs"""
-
-    def forward(
-        self,
-        input_ids: torch.Tensor,
-        attention_mask: torch.Tensor,
-        position_ids: Optional[torch.Tensor] = None,
-        # unused
-        return_dict: bool = True,
-        output_attentions: bool = False,
-        output_hidden_states: bool = False
-    ):
-        batch_size, seq_len = input_ids.shape
-        if position_ids is None:
-            position_ids = attention_mask.long().cumsum(-1) - 1
-            position_ids.masked_fill_(attention_mask == 0, 0)
-
-        # get indices
-        seqlens_in_batch = attention_mask.sum(dim=-1, dtype=torch.int32)
-        indices = torch.nonzero(attention_mask.flatten(), as_tuple=False).flatten()
-        max_seqlen_in_batch = int(seqlens_in_batch.max().item())
-        cu_seqlens = torch.nn.functional.pad(torch.cumsum(seqlens_in_batch, dim=0, dtype=torch.int32), (1, 0))
-
-        # Unpad inputs
-        nz_input_ids    = torch.take_along_dim(input_ids,    indices)
-        nz_position_ids = torch.take_along_dim(position_ids, indices)
-
-        # Unpadded forward
-        logits = super().forward(
-            nz_input_ids=nz_input_ids,
-            nz_position_ids=nz_position_ids,
-            cu_seqlens=cu_seqlens,
-            max_seqlen=max_seqlen_in_batch
-        ).logits
-
-        # Pad logits
-        logits = pad_input(logits, indices, batch_size, seq_len)
-
-        return CausalLMOutputWithPast(logits=logits)  # type: ignore
-
-    def prepare_inputs_for_generation(self,
-                                      input_ids: torch.Tensor,
-                                      **kwargs):
-        return {
-            "input_ids": input_ids,
-            "attention_mask": kwargs.get("attention_mask"),
-            "position_ids": kwargs.get("position_ids")
-        }
```

### Comparing `ochat-3.5.2/ochat/scripts/hf_add_tokens.py` & `ochat-3.6.0/ochat/scripts/hf_add_tokens.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/scripts/modify_eos_embedding.py` & `ochat-3.6.0/ochat/scripts/modify_eos_embedding.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/serving/async_tokenizer.py` & `ochat-3.6.0/ochat/serving/async_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/serving/openai_api_protocol.py` & `ochat-3.6.0/ochat/serving/openai_api_protocol.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/serving/openai_api_server.py` & `ochat-3.6.0/ochat/serving/openai_api_server.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/tests/test_model_config.py` & `ochat-3.6.0/ochat/tests/test_model_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 import pytest
+from colorama import Fore
 
 from ochat.config import MODEL_CONFIG_MAP, Conversation
 
 
+def visualize_tokens(tokenizer, tokens, weights):
+    COLORS = [Fore.RED, Fore.GREEN, Fore.YELLOW, Fore.BLUE]
+    if weights is None:
+        weights = [1.] * len(tokens)
+
+    color_index = 0
+    for item, w_item in zip(tokenizer.convert_ids_to_tokens(tokens), weights):
+        color = ""
+        item = item.replace("Ġ", "▁").replace("Ċ", "⏎\n")
+        if w_item != 0:
+            color = COLORS[color_index]
+            color_index = (color_index + 1) % len(COLORS)
+
+        print (color + item + Fore.RESET, end="")
+
+
 @pytest.mark.cpu
 def test_conv_template():
     # Training mode
     conversations = [
         # Normal conversations
         {
             "condition": "GPT4",
@@ -74,58 +91,123 @@
             ],
             "expected_weights": [
                 [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
                 [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.5, 0.5, 0.5, 0.5, 0.5, 0.0, 0.0, 0.0, 0.0, 0.0, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.0, 0.0, 0.0, 0.0, 0.0, 0.5, 0.5, 0.5, 0.5, 0.5, 0.0, 0.0, 0.0, 0.0, 0.0, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5],
                 [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1],
                 [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
             ]
+        },
+        {
+            "type": "openchat_3.6",
+            "model": ("meta-llama/Meta-Llama-3-8B", "imone/Llama-3-8B-fixed-special-embedding"),
+            "expected_tokens": [
+                [128000, 128006, 38, 2898, 19, 2724, 128007, 271, 3923, 596, 279, 9282, 1093, 30, 128009, 128006, 38, 2898, 19, 22103, 128007, 271, 40, 2846, 459, 15592, 323, 1541, 956, 617, 2680, 311, 1972, 7394, 828, 13, 128009, 128006, 38, 2898, 19, 2724, 128007, 271, 12174, 11, 1314, 13, 2650, 649, 358, 1440, 30, 128009, 128006, 38, 2898, 19, 22103, 128007, 271, 2675, 649, 1817, 264, 9282, 3997, 477, 917, 369, 279, 1455, 1510, 2038, 13, 128009],
+                [128000, 128006, 38, 2898, 18, 2724, 128007, 271, 3923, 374, 15592, 30, 128009, 128006, 38, 2898, 18, 22103, 128007, 271, 15836, 13656, 369, 59294, 22107, 13, 1102, 19813, 311, 279, 19576, 315, 3823, 11478, 11618, 555, 12933, 13, 128009, 128006, 38, 2898, 18, 2724, 128007, 271, 6854, 499, 4048, 30, 128009, 128006, 38, 2898, 18, 22103, 128007, 271, 40, 649, 956, 4048, 477, 6227, 2038, 1093, 12966, 13, 358, 7068, 14847, 3196, 389, 864, 50457, 828, 13, 128009],
+                [128000, 128006, 2374, 128007, 271, 2675, 527, 264, 11190, 18328, 13, 128009, 128006, 38, 2898, 18, 2724, 128007, 271, 6854, 499, 7079, 264, 2363, 30, 128009, 128006, 38, 2898, 18, 22103, 128007, 271, 40914, 13, 364, 50, 2113, 729, 25, 362, 37618, 11346, 315, 20449, 70370, 6, 555, 28372, 838, 43084, 5340, 2850, 374, 264, 2294, 1373, 13, 128009, 128006, 38, 2898, 18, 2724, 128007, 271, 3923, 596, 433, 922, 30, 128009, 128006, 38, 2898, 18, 22103, 128007, 271, 2181, 596, 922, 279, 3925, 315, 279, 3823, 9606, 505, 279, 15740, 315, 84497, 328, 2113, 729, 304, 10384, 709, 311, 279, 3118, 1938, 13, 128009],
+                [128000, 128006, 2374, 128007, 271, 45147, 55621, 527, 264, 11190, 18328, 13, 128009, 128006, 38, 2898, 19, 2724, 128007, 271, 3923, 656, 366, 82, 29, 694, 82, 29, 83739, 408, 3659, 38374, 91, 29, 3152, 30, 128009, 128006, 38, 2898, 19, 22103, 128007, 271, 45147, 29, 694, 82, 29, 83739, 408, 3659, 38374, 91, 29, 527, 3361, 11460, 13, 128009]],
+            "expected_weights": [
+                [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
+                [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.5, 0.5, 0.5, 0.5, 0.5, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.5, 0.5, 0.5, 0.5, 0.5, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5],
+                [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1],
+                [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0]
+            ]
         }
     ]
 
     for case in testcases:
-        for model in case["model"]:
+        for model_idx, model in enumerate(case["model"]):
             config = MODEL_CONFIG_MAP[case["type"]]
             tokenizer = config.model_tokenizer_create(model)
             conv_template = config.conversation_template(tokenizer=tokenizer)
 
             tokens, weights = conv_template.tokenize_conversations([Conversation(**conv) for conv in conversations], inference=False)
 
-            assert tokens == case["expected_tokens"]
-            assert weights == case["expected_weights"]
+            if "expected_tokens" in case:
+                assert tokens == case["expected_tokens"]
+                assert weights == case["expected_weights"]
+            else:
+                # Visualize the tokens if testcase does not exist yet.
+                if model_idx == 0:
+                    print ("Tokens ", tokens)
+                    print ("Weights ", weights)
+                    print ("\n\n")
+
+                    for conv_tokens, conv_weights in zip(tokens, weights):
+                        visualize_tokens(tokenizer, conv_tokens, conv_weights)
+                        print("\n\n")
 
     # Inference mode
     conversations = [
         {
             "items": [
                 {"role": "user", "content": "Who won the 2018 World Cup?"},
                 {"role": "assistant", "content": "The 2018 FIFA World Cup was won by France."},
                 {"role": "user", "content": "Okay, who won the 2022 World Cup?"},
                 {"role": "assistant", "content": ""},
             ]
+        },
+        {
+            "system": "You are a helpful assistant.",
+            "items": [
+                {"role": "user", "content": "Hi"},
+                {"role": "assistant", "content": ""},
+            ]
         }
     ]
     testcases = [
         {
             "type": "openchat_v3.2",
             "model": ("imone/Llama2_13B_with_EOT_token", "openchat/openchat_v3.2_super"),
             "expected_tokens": [
                 [1, 402, 7982, 29946, 4911, 29901, 11644, 2113, 278, 29871, 29906, 29900, 29896, 29947, 2787, 6536, 29973, 32000, 402, 7982, 29946, 4007, 22137, 29901, 450, 29871, 29906, 29900, 29896, 29947, 21581, 2787, 6536, 471, 2113, 491, 3444, 29889, 32000, 402, 7982, 29946, 4911, 29901, 20419, 29892, 1058, 2113, 278, 29871, 29906, 29900, 29906, 29906, 2787, 6536, 29973, 32000, 402, 7982, 29946, 4007, 22137, 29901],
+                [1, 887, 526, 263, 8444, 20255, 29889, 32000, 402, 7982, 29946, 4911, 29901, 6324, 32000, 402, 7982, 29946, 4007, 22137, 29901],
             ]
         },
         {
             "type": "openchat_v3.2_mistral",
             "model": ("imone/Mistral_7B_with_EOT_token", "openchat/openchat_3.5"),
             "expected_tokens": [
                 [1, 420, 6316, 28781, 3198, 3123, 1247, 28747, 6526, 1747, 272, 28705, 28750, 28734, 28740, 28783, 3304, 7440, 28804, 32000, 420, 6316, 28781, 3198, 3123, 21631, 28747, 415, 28705, 28750, 28734, 28740, 28783, 28702, 3304, 7440, 403, 1747, 486, 4843, 28723, 32000, 420, 6316, 28781, 3198, 3123, 1247, 28747, 19811, 28725, 693, 1747, 272, 28705, 28750, 28734, 28750, 28750, 3304, 7440, 28804, 32000, 420, 6316, 28781, 3198, 3123, 21631, 28747],
+                [1, 995, 460, 264, 10865, 13892, 28723, 32000, 420, 6316, 28781, 3198, 3123, 1247, 28747, 15359, 32000, 420, 6316, 28781, 3198, 3123, 21631, 28747],
             ]
-        }
+        },
+        {
+            "type": "openchat_3.6",
+            "model": ("meta-llama/Meta-Llama-3-8B", "imone/Llama-3-8B-fixed-special-embedding"),
+            "expected_tokens": [
+                [128000, 128006, 38, 2898, 19, 41070, 2724, 128007, 271, 15546, 2834, 279, 220, 679, 23, 4435, 11098, 30, 128009, 128006, 38, 2898, 19, 41070, 22103, 128007, 271, 791, 220, 679, 23, 44742, 4435, 11098, 574, 2834, 555, 9822, 13, 128009, 128006, 38, 2898, 19, 41070, 2724, 128007, 271, 33413, 11, 889, 2834, 279, 220, 2366, 17, 4435, 11098, 30, 128009, 128006, 38, 2898, 19, 41070, 22103, 128007, 271],
+                [128000, 128006, 2374, 128007, 271, 2675, 527, 264, 11190, 18328, 13, 128009, 128006, 38, 2898, 19, 41070, 2724, 128007, 271, 13347, 128009, 128006, 38, 2898, 19, 41070, 22103, 128007, 271]
+            ]
+        },
     ]
 
     for case in testcases:
-        for model in case["model"]:
+        for model_idx, model in enumerate(case["model"]):
             config = MODEL_CONFIG_MAP[case["type"]]
             tokenizer = config.model_tokenizer_create(model)
             conv_template = config.conversation_template(tokenizer=tokenizer)
 
             tokens, _ = conv_template.tokenize_conversations([Conversation(**conv) for conv in conversations], inference=True)  # type: ignore
 
-            assert tokens == case["expected_tokens"]
+            if "expected_tokens" in case:
+                assert tokens == case["expected_tokens"]
+            else:
+                # Visualize the tokens if testcase does not exist yet.
+                if model_idx == 0:
+                    print ("Tokens ", tokens)
+                    print ("\n\n")
+
+                    for conv_tokens in tokens:
+                        visualize_tokens(tokenizer, conv_tokens, None)
+                        print("\n\n")
+
+            # Additional assert for HF chat template
+            if config.hf_chat_template is not None:
+                tokenizer.chat_template = config.hf_chat_template
+                for conv, tokenized_conv in zip(conversations, tokens):
+                    # Add system turn
+                    turns = conv["items"][:-1]
+                    system = conv.get("system", "")
+                    if system:
+                        turns = [{"role": "system", "content": system}] + turns
+
+                    assert tokenized_conv == tokenizer.apply_chat_template(turns, tokenize=True, add_generation_prompt=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ochat-3.5.2/ochat/training_deepspeed/multipack_sampler.py` & `ochat-3.6.0/ochat/training_deepspeed/multipack_sampler.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/training_deepspeed/openchat_dataset.py` & `ochat-3.6.0/ochat/training_deepspeed/openchat_dataset.py`

 * *Files identical despite different names*

### Comparing `ochat-3.5.2/ochat/training_deepspeed/train.py` & `ochat-3.6.0/ochat/training_deepspeed/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import tqdm
 import wandb
 import numpy as np
 
 from ochat.config import MODEL_CONFIG_MAP
 from ochat.training_deepspeed.openchat_dataset import OpenchatDataset
+from ochat.training_deepspeed.hf_hub import hub_upload_check, hub_upload_model_async
 
 try:
     import deepspeed
 except ImportError:
     raise ImportError("Please install deepspeed to train models.")
 
 
@@ -27,14 +28,20 @@
     parser.add_argument("--local_rank", type=int, required=True)
 
     # Model type and data
     parser.add_argument("--model_path", type=str, required=True)
     parser.add_argument("--data_prefix", type=str, required=True)
     parser.add_argument("--save_path",  type=str, required=True)
     parser.add_argument("--save_every", type=int, default=None)
+    parser.add_argument("--push_to_hub", type=str, default=None, 
+                        help="Specify repository prefix for pushing to HuggingFace Hub. "
+                             "For example, 'openchat/openchat-3.6' will create repositories "
+                             "like 'openchat/openchat-3.6-ep0', 'openchat/openchat-3.6-ep1', ..."
+                                "If not specified, will not push to Hub.")
+    parser.add_argument("--push_to_hub_delete_local", action="store_true")
 
     # Hyperparameters
     parser.add_argument("--batch_max_len",      type=int, default=81920)
     parser.add_argument("--epochs",             type=int,   default=5)
 
     # Set lr to None to automatically estimate from LLaMA pretraining parameters (e.g. lr ~ sqrt(batch_size))
     parser.add_argument("--lr",                 type=float, default=None)
@@ -42,14 +49,17 @@
     parser.add_argument("--lr_warmup_ratio",    type=int,   default=0.05)
 
     parser.add_argument("--weight_decay",       type=float, default=0.1)
 
     parser.add_argument("--beta1",              type=float, default=0.9)
     parser.add_argument("--beta2",              type=float, default=0.95)
     parser.add_argument("--eps",                type=float, default=1e-5)
+    
+    parser.add_argument("--wandb_entity",       type=str, default=None)
+    parser.add_argument("--wandb_project",      type=str, default=None)
 
     # DeepSpeed parameters
     parser = deepspeed.add_config_arguments(parser)
 
     # Parse known args
     args, unknown = parser.parse_known_args()
     return args
@@ -132,15 +142,18 @@
         min_ratio=args.lr_min_ratio
     )
 
     return lr_scheduler
 
 
 def save_tokenizer(args, save_path):
-    MODEL_CONFIG_MAP[args.model_type].model_tokenizer_create(args.model_path).save_pretrained(save_path)
+    model_config = MODEL_CONFIG_MAP[args.model_type]
+    tokenizer = model_config.model_tokenizer_create(args.model_path)
+    tokenizer.chat_template = model_config.hf_chat_template
+    tokenizer.save_pretrained(save_path)
 
 
 def save_openchat_metadata(args, epoch, save_path):
     metadata = vars(args)
     metadata["epoch"] = epoch
 
     with open(os.path.join(save_path, "openchat.json"), "w") as f:
@@ -155,14 +168,17 @@
     # FIXME: Only 7B/13B is supported
     base_lr = 3e-4
     base_bs = 4_000_000
     if "mistral" in model_type.lower():
         base_lr /= 6.0
     elif "gemma" in model_type.lower():
         base_lr /= 5.5  # NOTE(one): Maybe MLP and Attn layers are using different lr?
+    elif "openchat_3.6" in model_type.lower():  # Llama 3 estimated hyperparams
+        # NOTE(one): Estimated divisor: 1.5 * sqrt(25000 H100s / 2000 H100s)
+        base_lr /= 5.3
 
     loss_weights = np.concatenate(train_dataset.dataset["nz_shifted_loss_weights"])
     supervised_ratio = np.sum(loss_weights != 0) / len(loss_weights)
 
     supervised_tokens = batch_max_len * dist.get_world_size() * supervised_ratio
     lr = base_lr * math.sqrt(supervised_tokens / base_bs)
 
@@ -188,14 +204,16 @@
     deepspeed.init_distributed(dist_backend="nccl")
     RANK = dist.get_rank()
     WORLD_SIZE = dist.get_world_size()
 
     # Args
     args       = parse_args()
 
+    hub_upload_check(args.push_to_hub)
+
     # Dataset
     train_dataset, train_loader = create_dataset_and_dataloader(args, 0)
 
     if train_dataset is None:
         raise RuntimeError("Training data not found.")
 
     # Load model type
@@ -213,15 +231,15 @@
     lr_scheduler = create_lr_scheduler(args, train_total_steps)
 
     # Progress bar and logger
     progress_bar = None
     if RANK == 0:
         progress_bar = tqdm.tqdm(total=train_total_steps)
 
-        wandb.init(project=os.path.basename(args.model_path), config=args)
+        wandb.init(project=args.wandb_project or os.path.basename(args.model_path), entity=args.wandb_entity, config=args)
 
     # Training Loop
     step = 0
     lr_this_step = None
     for epoch in range(args.epochs):
         print (f"[rank {RANK} of {WORLD_SIZE}]: Epoch {epoch}")
 
@@ -277,10 +295,18 @@
 
                 # Also save tokenizer from base model
                 save_tokenizer(args, save_path)
 
                 # Write metadata
                 save_openchat_metadata(args, epoch, save_path)
 
+                # Upload to hub
+                hub_upload_model_async(
+                    args.push_to_hub,
+                    args.push_to_hub_delete_local,
+                    save_path,
+                    epoch
+                )
+
 
 if __name__ == "__main__":
     train()
```

### Comparing `ochat-3.5.2/ochat.egg-info/PKG-INFO` & `ochat-3.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,30 @@
-Metadata-Version: 2.1
-Name: ochat
-Version: 3.5.2
-Summary: An efficient framework for training and serving top-tier, open-source conversational LLMs.
-Project-URL: Homepage, https://github.com/imoneoi/openchat
-Project-URL: Bug Tracker, https://github.com/imoneoi/openchat/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify
-Requires-Dist: openai
-Requires-Dist: tenacity
-Requires-Dist: tiktoken
-Requires-Dist: tqdm
-Requires-Dist: wandb
-Requires-Dist: numba
-Requires-Dist: datasets
-Requires-Dist: orjson
-Requires-Dist: torch
-Requires-Dist: ray
-Requires-Dist: sentencepiece
-Requires-Dist: transformers>=4.38.2
-Requires-Dist: accelerate
-Requires-Dist: protobuf
-Requires-Dist: fastapi
-Requires-Dist: pydantic
-Requires-Dist: shortuuid
-Requires-Dist: uvicorn
-Requires-Dist: vllm>=0.3.3
-Requires-Dist: pytest
-
 # OpenChat: Advancing Open-source Language Models with Mixed-Quality Data
 
 <div align="center">
   <img src="assets/logo_new.png" style="width: 65%">
 </div>
 
 <p align="center">
   <a href="https://openchat.team">💻Online Demo</a> |
   <a href="https://huggingface.co/openchat">🤗Huggingface</a> |
   <a href="https://arxiv.org/pdf/2309.11235.pdf">📃Paper</a> |
   <a href="https://discord.gg/pQjnXvNKHY">💭Discord</a> 
-  <br><br>
-  <strong>🏆 The Overall Best Performing Open Source 7B Model 🏆</strong>
-  <br>
-  <strong>🤖 Outperforms ChatGPT (March) and Grok-1 🤖</strong>
-  <br>
 </p>
 
-<div align="center">
-  <img src="https://raw.githubusercontent.com/imoneoi/openchat/master/assets/openchat-bench-0106.png" style="width: 95%;">
-</div>
-
 - OpenChat is an innovative library of **open-source language models**, fine-tuned with [**C-RLFT**](https://arxiv.org/pdf/2309.11235.pdf) - a strategy inspired by offline reinforcement learning.
 - Our models learn from mixed-quality data without preference labels, delivering exceptional performance on par with `ChatGPT`, even with a `7B` model which can be run on a **consumer GPU (e.g. RTX 3090)**.
 - Despite our simple approach, we are committed to developing a high-performance, commercially viable, open-source large language model, and we continue to make significant strides toward this vision.
 
 [![DOI](https://zenodo.org/badge/645397533.svg)](https://zenodo.org/badge/latestdoi/645397533)
 
 # ✨ News
 
+ - [2024/05/22] We released the Llama-3 based version [OpenChat 3.6 20240522](https://huggingface.co/openchat/openchat-3.6-8b-20240522), outperforming official Llama 3 8B Instruct and open-source finetunes/merges.
+
 - [2024/01/06] We released the second update, [OpenChat 3.5 0106](openchat/openchat-3.5-0106), further improved coding and overall performance 🏆.
 
 - [2023/12/10] We released the first update, [OpenChat 3.5 1210](openchat/openchat-3.5-1210), improved coding by 15 points 🚀.
 
 - [2023/11/01] We released the [OpenChat-3.5-7B](https://huggingface.co/openchat/openchat_3.5) model, surpassing ChatGPT on various benchmarks 🔥.
 
 - [2023/09/21] We released our paper [OpenChat: Advancing Open-source Language Models with Mixed-Quality Data](https://arxiv.org/pdf/2309.11235.pdf).
@@ -80,21 +39,39 @@
 - [2023/07/30] We are thrilled to introduce the [OpenChat V3 model series](#models), based on Llama 2, and now available for free for commercial use!
 
 - [2023/07/07] We released the [OpenChat V2 model series](#legacy-models).
 
 - [2023/07/01] We released the [OpenChat V1 model series](#legacy-models).
 </details>
 
-# 🏷️ Benchmarks
+# 🏷️ Benchmarks - OpenChat 3.6
+
+<div align="center">
+  <img src="https://raw.githubusercontent.com/imoneoi/openchat/master/assets/benchmarks-openchat-3.6-20240522.svg" style="width: 95%;">
+</div>
+
+
+<details>
+  <summary>Reproducing benchmarks</summary>
+
+Note: Please run the following commands at the base directory of this repository.
+
+```bash
+python -m ochat.evaluation.run_eval --condition "GPT4 Correct" --model openchat/openchat-3.6-8b-20240522 --eval_sets fs_cothub/mmlu fs_cothub/gsm8k fs_cothub/math
+python -m ochat.evaluation.run_eval --condition "GPT4" --model openchat/openchat-3.6-8b-20240522 --eval_sets zs/gpqa
+```
+
+HumanEval is run using the official [EvalPlus repository](https://github.com/evalplus/evalplus).
+</details>
+
+# 🏷️ Benchmarks - OpenChat 3.5
 
 | Model                 | # Params | Average  | MT-Bench     | HumanEval       | BBH MC   | AGIEval  | TruthfulQA    | MMLU         | GSM8K        | BBH CoT     |
 |-----------------------|----------|----------|--------------|-----------------|----------|----------|---------------|--------------|--------------|-------------|
 | **OpenChat-3.5-0106** | **7B**   | **64.5** | 7.8          | **71.3**        | **51.5** | **49.1** | 61.0          | 65.8         | **77.4**     | 62.2        |
-| OpenChat-3.5-1210     | **7B**   | 63.8     | 7.76         | 68.9            | 49.5     | 48.0     | **61.8**      | 65.3         | 77.3         | 61.8        |
-| OpenChat-3.5          | **7B**   | 61.6     | 7.81         | 55.5            | 47.6     | 47.4     | 59.1          | 64.3         | 77.3         | 63.5        |
 | ChatGPT (March)*      | ???B     | 61.5     | **7.94**     | 48.1            | 47.6     | 47.1     | 57.7          | **67.3**     | 74.9         | **70.1**    |
 |                       |          |          |              |                 |          |          |               |              |              |             |
 | OpenHermes 2.5        | 7B       | 59.3     | 7.54         | 48.2            | 49.4     | 46.5     | 57.5          | 63.8         | 73.5         | 59.9        |
 | OpenOrca Mistral      | 7B       | 52.7     | 6.86         | 38.4            | 49.4     | 42.9     | 45.9          | 59.3         | 59.1         | 58.1        |
 | Zephyr-β^             | 7B       | 34.6     | 7.34         | 22.0            | 40.6     | 39.0     | 40.8          | 39.8         | 5.1          | 16.0        |
 | Mistral               | 7B       | -        | 6.84         | 30.5            | 39.0     | 38.0     | -             | 60.1         | 52.2         | -           |
 | Open-source SOTA**    | 13B-70B  | 61.4     | 7.71         | 73.2            | 49.7     | 41.7     | 62.3          | 63.7         | 82.3         | 41.4        |
@@ -156,16 +133,14 @@
 ## 🎇 Comparison with [X.AI Grok](https://x.ai/)
 
 🔥 OpenChat-3.5-0106 (7B) now outperforms Grok-0 (33B) on **all 4 benchmarks** and Grok-1 (???B) on average and **3/4 benchmarks**.
 
 |                       | License     | # Param | Average  | MMLU   | HumanEval | MATH     | GSM8k    |
 |-----------------------|-------------|---------|----------|--------|-----------|----------|----------|
 | **OpenChat-3.5-0106** | Apache-2.0  | **7B**  | **61.0** | 65.8   | **71.3**  | **29.3** | **77.4** |
-| OpenChat-3.5-1210     | Apache-2.0  | **7B**  | 60.1     | 65.3   | 68.9      | 28.9     | 77.3     |
-| OpenChat-3.5          | Apache-2.0  | **7B**  | 56.4     | 64.3   | 55.5      | 28.6     | 77.3     |
 | Grok-0                | Proprietary | 33B     | 44.5     | 65.7   | 39.7      | 15.7     | 56.8     |
 | Grok-1                | Proprietary | ???B    | 55.8     | **73** | 63.2      | 23.9     | 62.9     |
 
 # ⬇️ Installation
 > [!NOTE]
 > Need [`pytorch`](https://pytorch.org/get-started/locally/#start-locally) to run OpenChat
 
@@ -303,23 +278,22 @@
 
 # <a id="training"></a> 🛠️ Training
 
 The OpenChat training system utilizes padding-free training and the [Multipack Sampler](https://github.com/imoneoi/multipack_sampler), achieving a **3~10x** speedup compared to the conventional padded training.
 
 ## Choose a base model
 
-OpenChat supports Llama 2 and Mistral models. Please first choose a base model to fit your needs. Each base model has a corresponding weight repo, model type, and recommended batch size as listed below, they should be filled into `BASE_REPO`, `MODEL_TYPE`, and `BATCH_SIZE` in the following instructions.
+OpenChat supports Llama 3 and Mistral models. Please first choose a base model to fit your needs. Each base model has a corresponding weight repo, model type, and recommended batch size as listed below, they should be filled into `BASE_REPO`, `MODEL_TYPE`, and `BATCH_SIZE` in the following instructions.
 
-| Base Model | Size | Weights (with EOT token)          | Model Type              | Recommended Batch Size per GPU (8xA100 80GB) |
-|------------|------|-----------------------------------|-------------------------|--------------------------------------|
-| Mistral    | 7B   | `imone/Mistral_7B_with_EOT_token` | `openchat_v3.2_mistral` | 77824                                |
-| Llama 2    | 7B   | `imone/LLaMA2_7B_with_EOT_token`  | `openchat_v3.2`         | 77824                                |
-| Llama 2    | 13B  | `imone/Llama2_13B_with_EOT_token` | `openchat_v3.2`         | 36864                                |
+| Base Model | Size | Weights (with EOT token)                   | Model Type              | Recommended Batch Size per GPU (8xA100 80GB) |
+|------------|------|--------------------------------------------|-------------------------|----------------------------------------------|
+| Llama 3    | 8B   | `imone/Llama-3-8B-fixed-special-embedding` | `openchat_3.6`          | 40960                                        |
+| Mistral    | 7B   | `imone/Mistral_7B_with_EOT_token`          | `openchat_v3.2_mistral` | 77824                                        |
 
-Note: The OpenChat conversation template requires an `<|end_of_turn|>` special token. The base model specified must include this token. Our provided weights are the original base weights with this token added. If you want to add them manually, use the `convert_llama_weights_to_hf_add_tokens.py` or `mistral_add_tokens.py` in the `scripts` directory.
+Note: The OpenChat conversation template requires `<|eot_id|>, <|start_header_id|>, <|end_header_id|>` (Llama 3) `<|end_of_turn|>` (Mistral) special tokens. The base model specified must include these tokens with initialized embeddings. Our provided weights are the original base weights with this token added and embeddings initialized. If you want to add them manually, use the `init_special_embedding_llama3.py` or `mistral_add_tokens.py` in the `scripts` directory.
 
 ## Installing DeepSpeed and Flash Attention
 
 First, ensure that the CUDA `nvcc` compiler is available in your environment. If it is not, install the CUDA toolkit that matches the version used by PyTorch.
 
 Next, install building dependencies:
 
@@ -420,57 +394,47 @@
 OpenChat may sometimes generate information that does not exist or is not accurate, also known as "hallucination". Users should be aware of this possibility and verify any critical information obtained the model.
 
 ## Safety
 OpenChat may sometimes generate harmful, hate speech, biased responses, or answer unsafe questions. It's crucial to apply additional AI safety measures in use cases that require safe and moderated responses.
 
 # License
 
-Our OpenChat 3.5 `code` and `models` are distributed under the **Apache License 2.0**.
-
-# <a id="models"></a> Models
-
-| Model        | Size | Context | Weights                                                     | Serving                                                                                                     |
-|--------------|------|---------|-------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|
-| OpenChat 3.5 0106 | 7B   | 8192    | [Huggingface](https://huggingface.co/openchat/openchat-3.5-0106) | `python -m ochat.serving.openai_api_server --model openchat/openchat-3.5-0106 --engine-use-ray --worker-use-ray` |
-| OpenChat 3.5 1210 | 7B   | 8192    | [Huggingface](https://huggingface.co/openchat/openchat-3.5-1210) | `python -m ochat.serving.openai_api_server --model openchat/openchat-3.5-1210 --engine-use-ray --worker-use-ray` |
-| OpenChat 3.5 | 7B   | 8192    | [Huggingface](https://huggingface.co/openchat/openchat_3.5) | `python -m ochat.serving.openai_api_server --model openchat/openchat_3.5 --engine-use-ray --worker-use-ray` |
-
-## <a id="legacy-models"></a> Legacy Models
-
-The following models are older versions of OpenChat and have inferior performance compared to the latest version. They will be deprecated in the next release. Please note that OpenChat V1 and V2 series are now deprecated, [please install 3.1.x for using V1 and V2 models](https://github.com/imoneoi/openchat/tree/83a683c775c77867cc45937fafdf48e8dcb68daa)
-
-To run the models on multiple GPUs with smaller VRAM, you can enable tensor parallelization, for example, using the `--tensor-parallel-size 2` flag.
-
-| Model        | Size | Context | Weights                                                      | Serving                                                                                                      |
-|--------------|------|---------|--------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|
-| OpenChat 3.2 SUPER | 13B  | 4096    | [Huggingface](https://huggingface.co/openchat/openchat_v3.2_super) | `python -m ochat.serving.openai_api_server --model openchat/openchat_v3.2_super --engine-use-ray --worker-use-ray` |
+Code is distributed under the **Apache License 2.0**.
 
 # Citation
 
 ```
 @article{wang2023openchat,
   title={OpenChat: Advancing Open-source Language Models with Mixed-Quality Data},
   author={Wang, Guan and Cheng, Sijie and Zhan, Xianyuan and Li, Xiangang and Song, Sen and Liu, Yang},
   journal={arXiv preprint arXiv:2309.11235},
   year={2023}
 }
 ```
 
 # 💌Contact
 
-We are a student team at Tsinghua University, working on OpenChat, a project that requires additional computing power or LLMs API keys for further development. If you are interested in our project and would like to offer support, please feel free to reach out to us:
-
-**Project Leader:**
+**Project Lead:**
 - Guan Wang [imonenext at gmail dot com]
-- [Sijie Cheng](https://adacheng.github.io/) [csj23 at mails dot tsinghua dot edu dot cn]
+- [Alpay Ariyak](https://github.com/alpayariyak) [aariyak at wpi dot edu]
 
 **Main Contributors:**
-- [Xianyuan Zhan](https://scholar.google.com.hk/citations?user=pDMnGloAAAAJ&hl=zh-CN) (Tsinghua University): Provided invaluable advice on paper writing.
-- [Alpay Ariyak](https://github.com/alpayariyak): Responsible for data collection, documentation, model cards and PR for `openchat-3.5-1210`, `openchat-3.5-0106`.
-- LDJ: Tasked with partial data collection for `openchat-3.5`.
+- [Xianyuan Zhan](https://scholar.google.com.hk/citations?user=pDMnGloAAAAJ) (Tsinghua University)
+- Qiying Yu (Tsinghua University)
+- Changling Liu (GPT Desk Pte. Ltd.)
+- LDJ
+- AutoMeta (Alignment Lab AI)
 
 **Sponsors:**
-- [Sen Song](https://scholar.google.com/citations?user=cYgtRP4AAAAJ&hl=en) (Tsinghua University), [Yang Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University), [01.AI Company](https://www.lingyiwanwu.com/en), [RunPod](https://www.runpod.io/), Changling Liu (GPT Desk Pte. Ltd.), Qiying Yu (Tsinghua University), AutoMeta (Alignment Lab AI).
+- [Sen Song](https://scholar.google.com/citations?user=cYgtRP4AAAAJ) (Tsinghua University)
+- [Yang Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University)
+- [01.AI Company](https://www.lingyiwanwu.com/en)
+- [RunPod](https://www.runpod.io/)
 
 **Special Thanks:**
-- We express our profound gratitude to Alignment Lab AI, Nous Research, and Pygmalion AI for their significant contributions to data collection and model training. We also extend our special thanks to Xiangang Li, Baochang Ma, and Hao Wan from 01.AI company for their generous provision of resources. We also thank Jianxiong Li and Peng Li at Tsinghua University for their insightful discussions that have enriched our work.
-- We acknowledge and thank the developers behind these projects: [Mistral](https://mistral.ai/), [Chain-of-Thought Hub](https://github.com/FranxYao/chain-of-thought-hub), [Llama 2](https://ai.meta.com/llama/), [Self-Instruct](https://arxiv.org/abs/2212.10560), [FastChat (Vicuna)](https://github.com/lm-sys/FastChat), [Alpaca](https://github.com/tatsu-lab/stanford_alpaca.git), and [StarCoder](https://github.com/bigcode-project/starcoder). Their work has been instrumental in driving our research forward.
+ - [Mistral](https://mistral.ai/)
+ - [Chain-of-Thought Hub](https://github.com/FranxYao/chain-of-thought-hub)
+ - [Llama 2](https://ai.meta.com/llama/)
+ - [Self-Instruct](https://arxiv.org/abs/2212.10560)
+ - [FastChat (Vicuna)](https://github.com/lm-sys/FastChat)
+ - [Alpaca](https://github.com/tatsu-lab/stanford_alpaca.git)
+ - [StarCoder](https://github.com/bigcode-project/starcoder)
```

#### html2text {}

```diff
@@ -1,125 +1,114 @@
-Metadata-Version: 2.1 Name: ochat Version: 3.5.2 Summary: An efficient
-framework for training and serving top-tier, open-source conversational LLMs.
-Project-URL: Homepage, https://github.com/imoneoi/openchat Project-URL: Bug
-Tracker, https://github.com/imoneoi/openchat/issues Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
-License Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
-Requires-Dist: openai Requires-Dist: tenacity Requires-Dist: tiktoken Requires-
-Dist: tqdm Requires-Dist: wandb Requires-Dist: numba Requires-Dist: datasets
-Requires-Dist: orjson Requires-Dist: torch Requires-Dist: ray Requires-Dist:
-sentencepiece Requires-Dist: transformers>=4.38.2 Requires-Dist: accelerate
-Requires-Dist: protobuf Requires-Dist: fastapi Requires-Dist: pydantic
-Requires-Dist: shortuuid Requires-Dist: uvicorn Requires-Dist: vllm>=0.3.3
-Requires-Dist: pytest # OpenChat: Advancing Open-source Language Models with
-Mixed-Quality Data
+# OpenChat: Advancing Open-source Language Models with Mixed-Quality Data
                              [assets/logo_new.png]
-         _ð___»_O_n_l_i_n_e_ _D_e_m_o | _ð__¤__H_u_g_g_i_n_g_f_a_c_e | _ð____P_a_p_e_r | _ð___­_D_i_s_c_o_r_d
-
-          ?ð??? TThhee OOvveerraallll BBeesstt PPeerrffoorrmmiinngg OOppeenn SSoouurrccee 77BB MMooddeell ?ð???
-               ?ð??¤? OOuuttppeerrffoorrmmss CChhaattGGPPTT ((MMaarrcchh)) aanndd GGrrookk--11 ?ð??¤?
-  [https://raw.githubusercontent.com/imoneoi/openchat/master/assets/openchat-
-                                bench-0106.png]
+          _ð___»_O_n_l_i_n_e_ _D_e_m_o | _ð__¤__H_u_g_g_i_n_g_f_a_c_e | _ð____P_a_p_e_r | _ð___­_D_i_s_c_o_r_d
 - OpenChat is an innovative library of **open-source language models**, fine-
 tuned with [**C-RLFT**](https://arxiv.org/pdf/2309.11235.pdf) - a strategy
 inspired by offline reinforcement learning. - Our models learn from mixed-
 quality data without preference labels, delivering exceptional performance on
 par with `ChatGPT`, even with a `7B` model which can be run on a **consumer GPU
 (e.g. RTX 3090)**. - Despite our simple approach, we are committed to
 developing a high-performance, commercially viable, open-source large language
 model, and we continue to make significant strides toward this vision. [![DOI]
 (https://zenodo.org/badge/645397533.svg)](https://zenodo.org/badge/latestdoi/
-645397533) # â¨ News - [2024/01/06] We released the second update, [OpenChat
-3.5 0106](openchat/openchat-3.5-0106), further improved coding and overall
+645397533) # â¨ News - [2024/05/22] We released the Llama-3 based version
+[OpenChat 3.6 20240522](https://huggingface.co/openchat/openchat-3.6-8b-
+20240522), outperforming official Llama 3 8B Instruct and open-source
+finetunes/merges. - [2024/01/06] We released the second update, [OpenChat 3.5
+0106](openchat/openchat-3.5-0106), further improved coding and overall
 performance ð. - [2023/12/10] We released the first update, [OpenChat 3.5
 1210](openchat/openchat-3.5-1210), improved coding by 15 points ð. - [2023/
 11/01] We released the [OpenChat-3.5-7B](https://huggingface.co/openchat/
 openchat_3.5) model, surpassing ChatGPT on various benchmarks ð¥. - [2023/09/
 21] We released our paper [OpenChat: Advancing Open-source Language Models with
 Mixed-Quality Data](https://arxiv.org/pdf/2309.11235.pdf). Read more - [2023/
 09/03] We released the [OpenChat V3.2 SUPER]([#models](https://huggingface.co/
 openchat/openchat_v3.2_super)) model. - [2023/08/04] We have launched an
 [Online Demo](https://openchat.team) featuring the latest version, OpenChat
 3.2. - [2023/07/30] We are thrilled to introduce the [OpenChat V3 model series]
 (#models), based on Llama 2, and now available for free for commercial use! -
 [2023/07/07] We released the [OpenChat V2 model series](#legacy-models). -
 [2023/07/01] We released the [OpenChat V1 model series](#legacy-models). #
-ð·ï¸ Benchmarks | Model | # Params | Average | MT-Bench | HumanEval | BBH MC
-| AGIEval | TruthfulQA | MMLU | GSM8K | BBH CoT | |-----------------------|----
-------|----------|--------------|-----------------|----------|----------|------
----------|--------------|--------------|-------------| | **OpenChat-3.5-0106**
-| **7B** | **64.5** | 7.8 | **71.3** | **51.5** | **49.1** | 61.0 | 65.8 |
-**77.4** | 62.2 | | OpenChat-3.5-1210 | **7B** | 63.8 | 7.76 | 68.9 | 49.5 |
-48.0 | **61.8** | 65.3 | 77.3 | 61.8 | | OpenChat-3.5 | **7B** | 61.6 | 7.81 |
-55.5 | 47.6 | 47.4 | 59.1 | 64.3 | 77.3 | 63.5 | | ChatGPT (March)* | ???B |
-61.5 | **7.94** | 48.1 | 47.6 | 47.1 | 57.7 | **67.3** | 74.9 | **70.1** | | |
-| | | | | | | | | | | OpenHermes 2.5 | 7B | 59.3 | 7.54 | 48.2 | 49.4 | 46.5 |
-57.5 | 63.8 | 73.5 | 59.9 | | OpenOrca Mistral | 7B | 52.7 | 6.86 | 38.4 | 49.4
-| 42.9 | 45.9 | 59.3 | 59.1 | 58.1 | | Zephyr-Î²^ | 7B | 34.6 | 7.34 | 22.0 |
-40.6 | 39.0 | 40.8 | 39.8 | 5.1 | 16.0 | | Mistral | 7B | - | 6.84 | 30.5 |
-39.0 | 38.0 | - | 60.1 | 52.2 | - | | Open-source SOTA** | 13B-70B | 61.4 |
-7.71 | 73.2 | 49.7 | 41.7 | 62.3 | 63.7 | 82.3 | 41.4 | | | | | WizardLM 70B |
-WizardCoder 34B | Orca 13B | Orca 13B | Platypus2 70B | WizardLM 70B | MetaMath
-70B | Flan-T5 11B | Evaluation details *: ChatGPT (March) results are from GPT-
-4 Technical Report, Chain-of-Thought Hub, and our evaluation. ^: Zephyr-Î²
-often fails to follow few-shot CoT instructions, likely because it was aligned
-with only chat data but not trained on few-shot data. **: Mistral and Open-
-source SOTA results are taken from reported results in instruction-tuned model
-papers and official repositories. All models are evaluated in chat mode (e.g.
-with the respective conversation template applied). All zero-shot benchmarks
-follow the same setting as in the AGIEval paper and Orca paper. CoT tasks use
-the same configuration as Chain-of-Thought Hub, HumanEval is evaluated with
-EvalPlus, and MT-bench is run using FastChat. To reproduce our results, follow
-the instructions below. Reproducing benchmarks Reasoning and Coding: Note:
-Please run the following commands at the base directory of this repository.
-```bash python -m ochat.evaluation.run_eval --condition "GPT4 Correct" --model
-openchat/openchat-3.5-0106 --eval_sets coding fs_cothub/bbh fs_cothub/mmlu zs/
-agieval zs/bbh_mc_orca zs/truthfulqa_orca python ochat/evaluation/
-view_results.py python ochat/evaluation/convert_to_evalplus.py ``` Then all
-humaneval code samples are placed in `ochat/evaluation/evalplus_codegen`. Use
-the following command to evaluate an individual code sample named
-`samples.jsonl` using Docker as a sandbox. ```bash docker run -v $(pwd):/app
-ganler/evalplus:latest --dataset humaneval --samples samples.jsonl ```
-Mathematical Reasoning: Note: Please run the following commands at the base
+ð·ï¸ Benchmarks - OpenChat 3.6
+ [https://raw.githubusercontent.com/imoneoi/openchat/master/assets/benchmarks-
+                          openchat-3.6-20240522.svg]
+Reproducing benchmarks Note: Please run the following commands at the base
 directory of this repository. ```bash python -m ochat.evaluation.run_eval --
-condition "Math Correct" --model openchat/openchat-3.5-0106 --eval_sets
-fs_cothub/gsm8k zs/math python ochat/evaluation/view_results.py ``` MT-Bench:
-Please first launch a local API server, then download FastChat and run the
-following commands. Note: Due to non-zero temperature and GPT-4 API changes
-over time, there might be variations in the results. ```bash cd fastchat/
-llm_judge python gen_api_answer.py --model openchat-3.5-0106 --max-tokens 4096
---parallel 128 --openai-api-base http://localhost:18888/v1 python
-gen_judgment.py --model-list openchat-3.5-0106 --parallel 8 --mode single ```
-## ð Comparison with [X.AI Grok](https://x.ai/) ð¥ OpenChat-3.5-0106 (7B)
-now outperforms Grok-0 (33B) on **all 4 benchmarks** and Grok-1 (???B) on
-average and **3/4 benchmarks**. | | License | # Param | Average | MMLU |
-HumanEval | MATH | GSM8k | |-----------------------|-------------|---------|---
--------|--------|-----------|----------|----------| | **OpenChat-3.5-0106** |
-Apache-2.0 | **7B** | **61.0** | 65.8 | **71.3** | **29.3** | **77.4** | |
-OpenChat-3.5-1210 | Apache-2.0 | **7B** | 60.1 | 65.3 | 68.9 | 28.9 | 77.3 | |
-OpenChat-3.5 | Apache-2.0 | **7B** | 56.4 | 64.3 | 55.5 | 28.6 | 77.3 | | Grok-
-0 | Proprietary | 33B | 44.5 | 65.7 | 39.7 | 15.7 | 56.8 | | Grok-1 |
-Proprietary | ???B | 55.8 | **73** | 63.2 | 23.9 | 62.9 | # â¬ï¸ Installation
-> [!NOTE] > Need [`pytorch`](https://pytorch.org/get-started/locally/#start-
-locally) to run OpenChat ## pip ```bash pip3 install ochat ``` > [!IMPORTANT] >
-If you are facing package compatibility issues with pip, try the conda method
-below or check [this issue](https://github.com/imoneoi/openchat/issues/41) ##
-conda ```bash conda create -y --name openchat python=3.11 conda activate
-openchat pip3 install ochat ``` ## Windows (WSL 1.x, Ubuntu-22.04) ```bash sudo
-apt update sudo apt install build-essential sudo apt install -y curl curl -
-o miniconda.sh https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-
-x86_64.sh bash miniconda.sh # Restart WSL terminal if the following conda
-command does not work conda create -y --name openchat python=3.11 conda
-activate openchat pip3 install ochat ``` ## From source Clone this repo and
-install openchat from source in editable mode ```bash git clone https://
-github.com/imoneoi/openchat cd openchat pip3 install --upgrade pip # enable PEP
-660 support pip3 install -e . # Editable mode, you can make changes in this
-cloned repo ``` # ð Deploying API server â¡ Our API server is ready for
-production use and compatible with the OpenAI API protocol. It is highly
+condition "GPT4 Correct" --model openchat/openchat-3.6-8b-20240522 --eval_sets
+fs_cothub/mmlu fs_cothub/gsm8k fs_cothub/math python -
+m ochat.evaluation.run_eval --condition "GPT4" --model openchat/openchat-3.6-
+8b-20240522 --eval_sets zs/gpqa ``` HumanEval is run using the official
+[EvalPlus repository](https://github.com/evalplus/evalplus). # ð·ï¸
+Benchmarks - OpenChat 3.5 | Model | # Params | Average | MT-Bench | HumanEval |
+BBH MC | AGIEval | TruthfulQA | MMLU | GSM8K | BBH CoT | |---------------------
+--|----------|----------|--------------|-----------------|----------|----------
+|---------------|--------------|--------------|-------------| | **OpenChat-3.5-
+0106** | **7B** | **64.5** | 7.8 | **71.3** | **51.5** | **49.1** | 61.0 | 65.8
+| **77.4** | 62.2 | | ChatGPT (March)* | ???B | 61.5 | **7.94** | 48.1 | 47.6 |
+47.1 | 57.7 | **67.3** | 74.9 | **70.1** | | | | | | | | | | | | | | OpenHermes
+2.5 | 7B | 59.3 | 7.54 | 48.2 | 49.4 | 46.5 | 57.5 | 63.8 | 73.5 | 59.9 | |
+OpenOrca Mistral | 7B | 52.7 | 6.86 | 38.4 | 49.4 | 42.9 | 45.9 | 59.3 | 59.1 |
+58.1 | | Zephyr-Î²^ | 7B | 34.6 | 7.34 | 22.0 | 40.6 | 39.0 | 40.8 | 39.8 | 5.1
+| 16.0 | | Mistral | 7B | - | 6.84 | 30.5 | 39.0 | 38.0 | - | 60.1 | 52.2 | - |
+| Open-source SOTA** | 13B-70B | 61.4 | 7.71 | 73.2 | 49.7 | 41.7 | 62.3 | 63.7
+| 82.3 | 41.4 | | | | | WizardLM 70B | WizardCoder 34B | Orca 13B | Orca 13B |
+Platypus2 70B | WizardLM 70B | MetaMath 70B | Flan-T5 11B | Evaluation details
+*: ChatGPT (March) results are from GPT-4 Technical Report, Chain-of-Thought
+Hub, and our evaluation. ^: Zephyr-Î² often fails to follow few-shot CoT
+instructions, likely because it was aligned with only chat data but not trained
+on few-shot data. **: Mistral and Open-source SOTA results are taken from
+reported results in instruction-tuned model papers and official repositories.
+All models are evaluated in chat mode (e.g. with the respective conversation
+template applied). All zero-shot benchmarks follow the same setting as in the
+AGIEval paper and Orca paper. CoT tasks use the same configuration as Chain-of-
+Thought Hub, HumanEval is evaluated with EvalPlus, and MT-bench is run using
+FastChat. To reproduce our results, follow the instructions below. Reproducing
+benchmarks Reasoning and Coding: Note: Please run the following commands at the
+base directory of this repository. ```bash python -m ochat.evaluation.run_eval
+--condition "GPT4 Correct" --model openchat/openchat-3.5-0106 --eval_sets
+coding fs_cothub/bbh fs_cothub/mmlu zs/agieval zs/bbh_mc_orca zs/
+truthfulqa_orca python ochat/evaluation/view_results.py python ochat/
+evaluation/convert_to_evalplus.py ``` Then all humaneval code samples are
+placed in `ochat/evaluation/evalplus_codegen`. Use the following command to
+evaluate an individual code sample named `samples.jsonl` using Docker as a
+sandbox. ```bash docker run -v $(pwd):/app ganler/evalplus:latest --dataset
+humaneval --samples samples.jsonl ``` Mathematical Reasoning: Note: Please run
+the following commands at the base directory of this repository. ```bash python
+-m ochat.evaluation.run_eval --condition "Math Correct" --model openchat/
+openchat-3.5-0106 --eval_sets fs_cothub/gsm8k zs/math python ochat/evaluation/
+view_results.py ``` MT-Bench: Please first launch a local API server, then
+download FastChat and run the following commands. Note: Due to non-zero
+temperature and GPT-4 API changes over time, there might be variations in the
+results. ```bash cd fastchat/llm_judge python gen_api_answer.py --model
+openchat-3.5-0106 --max-tokens 4096 --parallel 128 --openai-api-base http://
+localhost:18888/v1 python gen_judgment.py --model-list openchat-3.5-0106 --
+parallel 8 --mode single ``` ## ð Comparison with [X.AI Grok](https://x.ai/
+) ð¥ OpenChat-3.5-0106 (7B) now outperforms Grok-0 (33B) on **all 4
+benchmarks** and Grok-1 (???B) on average and **3/4 benchmarks**. | | License |
+# Param | Average | MMLU | HumanEval | MATH | GSM8k | |-----------------------
+|-------------|---------|----------|--------|-----------|----------|----------
+| | **OpenChat-3.5-0106** | Apache-2.0 | **7B** | **61.0** | 65.8 | **71.3** |
+**29.3** | **77.4** | | Grok-0 | Proprietary | 33B | 44.5 | 65.7 | 39.7 | 15.7
+| 56.8 | | Grok-1 | Proprietary | ???B | 55.8 | **73** | 63.2 | 23.9 | 62.9 | #
+â¬ï¸ Installation > [!NOTE] > Need [`pytorch`](https://pytorch.org/get-
+started/locally/#start-locally) to run OpenChat ## pip ```bash pip3 install
+ochat ``` > [!IMPORTANT] > If you are facing package compatibility issues with
+pip, try the conda method below or check [this issue](https://github.com/
+imoneoi/openchat/issues/41) ## conda ```bash conda create -y --name openchat
+python=3.11 conda activate openchat pip3 install ochat ``` ## Windows (WSL 1.x,
+Ubuntu-22.04) ```bash sudo apt update sudo apt install build-essential sudo apt
+install -y curl curl -o miniconda.sh https://repo.anaconda.com/miniconda/
+Miniconda3-latest-Linux-x86_64.sh bash miniconda.sh # Restart WSL terminal if
+the following conda command does not work conda create -y --name openchat
+python=3.11 conda activate openchat pip3 install ochat ``` ## From source Clone
+this repo and install openchat from source in editable mode ```bash git clone
+https://github.com/imoneoi/openchat cd openchat pip3 install --upgrade pip #
+enable PEP 660 support pip3 install -e . # Editable mode, you can make changes
+in this cloned repo ``` # ð Deploying API server â¡ Our API server is ready
+for production use and compatible with the OpenAI API protocol. It is highly
 optimized with vLLM and can dynamically batch requests. ð Note: For 20
 series or older GPUs that do not support `bfloat16`, add `--dtype float16` to
 the server args. ### For a single GPU (e.g. RTX 3090, 4090) ```bash python -
 m ochat.serving.openai_api_server --model openchat/openchat-3.5-0106 ``` ###
 For multiple GPUs (tensor parallel) ```bash # N is the number of tensor
 parallel GPUs python -m ochat.serving.openai_api_server --model openchat/
 openchat-3.5-0106 --engine-use-ray --worker-use-ray --tensor-parallel-size N
@@ -154,141 +143,102 @@
 Correct User: 10.3 â 7988.8133=<|end_of_turn|>Math Correct Assistant: ```
 â ï¸ **Notice:** Remember to set `<|end_of_turn|>` as end of generation
 token. The default (GPT4 Correct) template is also available as the integrated
 `tokenizer.chat_template`, which can be used instead of manually specifying the
 template. # ð ï¸ Training The OpenChat training system utilizes padding-free
 training and the [Multipack Sampler](https://github.com/imoneoi/
 multipack_sampler), achieving a **3~10x** speedup compared to the conventional
-padded training. ## Choose a base model OpenChat supports Llama 2 and Mistral
+padded training. ## Choose a base model OpenChat supports Llama 3 and Mistral
 models. Please first choose a base model to fit your needs. Each base model has
 a corresponding weight repo, model type, and recommended batch size as listed
 below, they should be filled into `BASE_REPO`, `MODEL_TYPE`, and `BATCH_SIZE`
 in the following instructions. | Base Model | Size | Weights (with EOT token) |
 Model Type | Recommended Batch Size per GPU (8xA100 80GB) | |------------|-----
--|-----------------------------------|-------------------------|---------------
------------------------| | Mistral | 7B | `imone/Mistral_7B_with_EOT_token` |
-`openchat_v3.2_mistral` | 77824 | | Llama 2 | 7B | `imone/
-LLaMA2_7B_with_EOT_token` | `openchat_v3.2` | 77824 | | Llama 2 | 13B | `imone/
-Llama2_13B_with_EOT_token` | `openchat_v3.2` | 36864 | Note: The OpenChat
-conversation template requires an `<|end_of_turn|>` special token. The base
-model specified must include this token. Our provided weights are the original
-base weights with this token added. If you want to add them manually, use the
-`convert_llama_weights_to_hf_add_tokens.py` or `mistral_add_tokens.py` in the
-`scripts` directory. ## Installing DeepSpeed and Flash Attention First, ensure
-that the CUDA `nvcc` compiler is available in your environment. If it is not,
-install the CUDA toolkit that matches the version used by PyTorch. Next,
-install building dependencies: ```bash pip install packaging ninja ``` Finally,
-install the packages: ```bash pip install deepspeed flash-attn ``` ###
-Preparing Your Data To utilize the OpenChat trainer, prepare your SFT data into
-a JSON Lines format where each line corresponds to a `Conversation` object:
-```python class Message(BaseModel): role: str # Must be "user" or "assistant"
-content: str # Message content weight: Optional[float] = None # Loss weight for
-this message. Typically 0 for user and 1 for assistant to supervise assistant's
-responses only class Conversation(BaseModel): items: List[Message] # All
-messages within the conversation condition: str = "" # C-RLFT condition, can be
-any string or empty. system: str = "" # System message for this conversation
-``` For basic SFT, assign `weight` as `0` for human messages and `1` for
-assistant responses. SFT example: ```json {"items":[{"role":"user","content":
-"Hello","weight":0.0},{"role":"assistant","content":"Hi","weight":1.0},{"role":
-"user","content":"How are you today?","weight":0.0},{"role":
-"assistant","content":"I'm fine.","weight":1.0}],"system":""} {"items":[
-{"role":"user","content":"Who are you?","weight":0.0},{"role":
-"assistant","content":"I'm OpenChat.","weight":1.0}],"system":"You are a
-helpful assistant named OpenChat."} ``` For C-RLFT, `condition` should be set
-as the class the conversation belongs to (e.g. `GPT3` or `GPT4`). The `weight`
-is assigned as `0` for human messages and `w` for assistant responses, where
-`w` is the weight of the class (e.g. `0.1` for `GPT3` and `1` for `GPT4`, as
-found in our C-RLFT paper). C-RLFT example: ```json {"items":[{"role":
-"user","content":"What is C-RLFT?","weight":0.0},{"role":"assistant","content":
-"C-RLFT is a method for improving open-source LLMs with mixed-quality
-data.","weight":1.0}],"condition":"GPT4","system":""} {"items":[{"role":
-"user","content":"What is C-RLFT?","weight":0.0},{"role":"assistant","content":
-"I don't know.","weight":0.1}],"condition":"GPT3","system":""} ``` ### Pre-
-tokenizing the Dataset You'll then need to pre-tokenize the dataset using the
-command (please specify a filename as `PRETOKENIZED_DATA_OUTPUT_PATH` to store
-the pretokenized dataset): ```bash python -m ochat.data.generate_dataset --
-model-type MODEL_TYPE --model-path BASE_REPO --in-files data.jsonl --out-prefix
-PRETOKENIZED_DATA_OUTPUT_PATH ``` ### Launching the OpenChat Trainer You can
-now launch the OpenChat trainer using the command below. - 13B model requires
-eight `A/H100s` with 80GB VRAM - 7B model can be trained with four `A/H100s`
-with 80GB VRAM or eight `A/H100s` with 40GB VRAM. For hyperparameters, we
-recommend first setting the batch size to the recommended batch size. If OOM
-occurs, try setting it to the exact maximum that VRAM can hold and as a
-multiple of `2048`. Other hyperparameters have been carefully selected as the
-default. Furthermore, the learning rate is automatically determined based on
-the [inverse square-root rule](https://arxiv.org/abs/2006.09092). Training
-Commands (click to expand) ```bash NUM_GPUS=8 deepspeed --num_gpus=$NUM_GPUS --
-module ochat.training_deepspeed.train \ --model_path BASE_REPO \ --data_prefix
+-|--------------------------------------------|-------------------------|------
+----------------------------------------| | Llama 3 | 8B | `imone/Llama-3-8B-
+fixed-special-embedding` | `openchat_3.6` | 40960 | | Mistral | 7B | `imone/
+Mistral_7B_with_EOT_token` | `openchat_v3.2_mistral` | 77824 | Note: The
+OpenChat conversation template requires `<|eot_id|>, <|start_header_id|>,
+<|end_header_id|>` (Llama 3) `<|end_of_turn|>` (Mistral) special tokens. The
+base model specified must include these tokens with initialized embeddings. Our
+provided weights are the original base weights with this token added and
+embeddings initialized. If you want to add them manually, use the
+`init_special_embedding_llama3.py` or `mistral_add_tokens.py` in the `scripts`
+directory. ## Installing DeepSpeed and Flash Attention First, ensure that the
+CUDA `nvcc` compiler is available in your environment. If it is not, install
+the CUDA toolkit that matches the version used by PyTorch. Next, install
+building dependencies: ```bash pip install packaging ninja ``` Finally, install
+the packages: ```bash pip install deepspeed flash-attn ``` ### Preparing Your
+Data To utilize the OpenChat trainer, prepare your SFT data into a JSON Lines
+format where each line corresponds to a `Conversation` object: ```python class
+Message(BaseModel): role: str # Must be "user" or "assistant" content: str #
+Message content weight: Optional[float] = None # Loss weight for this message.
+Typically 0 for user and 1 for assistant to supervise assistant's responses
+only class Conversation(BaseModel): items: List[Message] # All messages within
+the conversation condition: str = "" # C-RLFT condition, can be any string or
+empty. system: str = "" # System message for this conversation ``` For basic
+SFT, assign `weight` as `0` for human messages and `1` for assistant responses.
+SFT example: ```json {"items":[{"role":"user","content":"Hello","weight":0.0},
+{"role":"assistant","content":"Hi","weight":1.0},{"role":"user","content":"How
+are you today?","weight":0.0},{"role":"assistant","content":"I'm
+fine.","weight":1.0}],"system":""} {"items":[{"role":"user","content":"Who are
+you?","weight":0.0},{"role":"assistant","content":"I'm OpenChat.","weight":
+1.0}],"system":"You are a helpful assistant named OpenChat."} ``` For C-RLFT,
+`condition` should be set as the class the conversation belongs to (e.g. `GPT3`
+or `GPT4`). The `weight` is assigned as `0` for human messages and `w` for
+assistant responses, where `w` is the weight of the class (e.g. `0.1` for
+`GPT3` and `1` for `GPT4`, as found in our C-RLFT paper). C-RLFT example:
+```json {"items":[{"role":"user","content":"What is C-RLFT?","weight":0.0},
+{"role":"assistant","content":"C-RLFT is a method for improving open-source
+LLMs with mixed-quality data.","weight":1.0}],"condition":"GPT4","system":""}
+{"items":[{"role":"user","content":"What is C-RLFT?","weight":0.0},{"role":
+"assistant","content":"I don't know.","weight":0.1}],"condition":
+"GPT3","system":""} ``` ### Pre-tokenizing the Dataset You'll then need to pre-
+tokenize the dataset using the command (please specify a filename as
+`PRETOKENIZED_DATA_OUTPUT_PATH` to store the pretokenized dataset): ```bash
+python -m ochat.data.generate_dataset --model-type MODEL_TYPE --model-path
+BASE_REPO --in-files data.jsonl --out-prefix PRETOKENIZED_DATA_OUTPUT_PATH ```
+### Launching the OpenChat Trainer You can now launch the OpenChat trainer
+using the command below. - 13B model requires eight `A/H100s` with 80GB VRAM -
+7B model can be trained with four `A/H100s` with 80GB VRAM or eight `A/H100s`
+with 40GB VRAM. For hyperparameters, we recommend first setting the batch size
+to the recommended batch size. If OOM occurs, try setting it to the exact
+maximum that VRAM can hold and as a multiple of `2048`. Other hyperparameters
+have been carefully selected as the default. Furthermore, the learning rate is
+automatically determined based on the [inverse square-root rule](https://
+arxiv.org/abs/2006.09092). Training Commands (click to expand) ```bash
+NUM_GPUS=8 deepspeed --num_gpus=$NUM_GPUS --module
+ochat.training_deepspeed.train \ --model_path BASE_REPO \ --data_prefix
 PRETOKENIZED_DATA_OUTPUT_PATH \ --save_path PATH_TO_SAVE_MODEL \ --
 batch_max_len BATCH_SIZE \ --epochs 5 \ --save_every 1 \ --deepspeed \ --
 deepspeed_config ochat/training_deepspeed/deepspeed_config.json ``` You can
 find checkpoints of all epochs in `PATH_TO_SAVE_MODEL`. Then you may evaluate
 each epoch and choose the best one. # Limitations ## Foundation Model
 Limitations Despite its advanced capabilities, OpenChat is still bound by the
 limitations inherent in its foundation models. These limitations may impact the
 model's performance in areas such as: - Complex reasoning - Mathematical and
 arithmetic tasks - Programming and coding challenges ## Hallucination of Non-
 existent Information OpenChat may sometimes generate information that does not
 exist or is not accurate, also known as "hallucination". Users should be aware
 of this possibility and verify any critical information obtained the model. ##
 Safety OpenChat may sometimes generate harmful, hate speech, biased responses,
 or answer unsafe questions. It's crucial to apply additional AI safety measures
-in use cases that require safe and moderated responses. # License Our OpenChat
-3.5 `code` and `models` are distributed under the **Apache License 2.0**. #
-Models | Model | Size | Context | Weights | Serving | |--------------|------|--
--------|-------------------------------------------------------------|---------
--------------------------------------------------------------------------------
----------------------| | OpenChat 3.5 0106 | 7B | 8192 | [Huggingface](https://
-huggingface.co/openchat/openchat-3.5-0106) | `python -
-m ochat.serving.openai_api_server --model openchat/openchat-3.5-0106 --engine-
-use-ray --worker-use-ray` | | OpenChat 3.5 1210 | 7B | 8192 | [Huggingface]
-(https://huggingface.co/openchat/openchat-3.5-1210) | `python -
-m ochat.serving.openai_api_server --model openchat/openchat-3.5-1210 --engine-
-use-ray --worker-use-ray` | | OpenChat 3.5 | 7B | 8192 | [Huggingface](https://
-huggingface.co/openchat/openchat_3.5) | `python -
-m ochat.serving.openai_api_server --model openchat/openchat_3.5 --engine-use-
-ray --worker-use-ray` | ## Legacy Models The following models are older
-versions of OpenChat and have inferior performance compared to the latest
-version. They will be deprecated in the next release. Please note that OpenChat
-V1 and V2 series are now deprecated, [please install 3.1.x for using V1 and V2
-models](https://github.com/imoneoi/openchat/tree/
-83a683c775c77867cc45937fafdf48e8dcb68daa) To run the models on multiple GPUs
-with smaller VRAM, you can enable tensor parallelization, for example, using
-the `--tensor-parallel-size 2` flag. | Model | Size | Context | Weights |
-Serving | |--------------|------|---------|------------------------------------
---------------------------|----------------------------------------------------
-----------------------------------------------------------| | OpenChat 3.2
-SUPER | 13B | 4096 | [Huggingface](https://huggingface.co/openchat/
-openchat_v3.2_super) | `python -m ochat.serving.openai_api_server --model
-openchat/openchat_v3.2_super --engine-use-ray --worker-use-ray` | # Citation
-``` @article{wang2023openchat, title={OpenChat: Advancing Open-source Language
-Models with Mixed-Quality Data}, author={Wang, Guan and Cheng, Sijie and Zhan,
-Xianyuan and Li, Xiangang and Song, Sen and Liu, Yang}, journal={arXiv preprint
-arXiv:2309.11235}, year={2023} } ``` # ðContact We are a student team at
-Tsinghua University, working on OpenChat, a project that requires additional
-computing power or LLMs API keys for further development. If you are interested
-in our project and would like to offer support, please feel free to reach out
-to us: **Project Leader:** - Guan Wang [imonenext at gmail dot com] - [Sijie
-Cheng](https://adacheng.github.io/) [csj23 at mails dot tsinghua dot edu dot
-cn] **Main Contributors:** - [Xianyuan Zhan](https://scholar.google.com.hk/
-citations?user=pDMnGloAAAAJ&hl=zh-CN) (Tsinghua University): Provided
-invaluable advice on paper writing. - [Alpay Ariyak](https://github.com/
-alpayariyak): Responsible for data collection, documentation, model cards and
-PR for `openchat-3.5-1210`, `openchat-3.5-0106`. - LDJ: Tasked with partial
-data collection for `openchat-3.5`. **Sponsors:** - [Sen Song](https://
-scholar.google.com/citations?user=cYgtRP4AAAAJ&hl=en) (Tsinghua University),
-[Yang Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University), [01.AI
-Company](https://www.lingyiwanwu.com/en), [RunPod](https://www.runpod.io/),
-Changling Liu (GPT Desk Pte. Ltd.), Qiying Yu (Tsinghua University), AutoMeta
-(Alignment Lab AI). **Special Thanks:** - We express our profound gratitude to
-Alignment Lab AI, Nous Research, and Pygmalion AI for their significant
-contributions to data collection and model training. We also extend our special
-thanks to Xiangang Li, Baochang Ma, and Hao Wan from 01.AI company for their
-generous provision of resources. We also thank Jianxiong Li and Peng Li at
-Tsinghua University for their insightful discussions that have enriched our
-work. - We acknowledge and thank the developers behind these projects:
-[Mistral](https://mistral.ai/), [Chain-of-Thought Hub](https://github.com/
-FranxYao/chain-of-thought-hub), [Llama 2](https://ai.meta.com/llama/), [Self-
-Instruct](https://arxiv.org/abs/2212.10560), [FastChat (Vicuna)](https://
-github.com/lm-sys/FastChat), [Alpaca](https://github.com/tatsu-lab/
-stanford_alpaca.git), and [StarCoder](https://github.com/bigcode-project/
-starcoder). Their work has been instrumental in driving our research forward.
+in use cases that require safe and moderated responses. # License Code is
+distributed under the **Apache License 2.0**. # Citation ``` @article
+{wang2023openchat, title={OpenChat: Advancing Open-source Language Models with
+Mixed-Quality Data}, author={Wang, Guan and Cheng, Sijie and Zhan, Xianyuan and
+Li, Xiangang and Song, Sen and Liu, Yang}, journal={arXiv preprint arXiv:
+2309.11235}, year={2023} } ``` # ðContact **Project Lead:** - Guan Wang
+[imonenext at gmail dot com] - [Alpay Ariyak](https://github.com/alpayariyak)
+[aariyak at wpi dot edu] **Main Contributors:** - [Xianyuan Zhan](https://
+scholar.google.com.hk/citations?user=pDMnGloAAAAJ) (Tsinghua University) -
+Qiying Yu (Tsinghua University) - Changling Liu (GPT Desk Pte. Ltd.) - LDJ -
+AutoMeta (Alignment Lab AI) **Sponsors:** - [Sen Song](https://
+scholar.google.com/citations?user=cYgtRP4AAAAJ) (Tsinghua University) - [Yang
+Liu](https://nlp.csai.tsinghua.edu.cn/~ly/) (Tsinghua University) - [01.AI
+Company](https://www.lingyiwanwu.com/en) - [RunPod](https://www.runpod.io/
+) **Special Thanks:** - [Mistral](https://mistral.ai/) - [Chain-of-Thought Hub]
+(https://github.com/FranxYao/chain-of-thought-hub) - [Llama 2](https://
+ai.meta.com/llama/) - [Self-Instruct](https://arxiv.org/abs/2212.10560) -
+[FastChat (Vicuna)](https://github.com/lm-sys/FastChat) - [Alpaca](https://
+github.com/tatsu-lab/stanford_alpaca.git) - [StarCoder](https://github.com/
+bigcode-project/starcoder)
```

### Comparing `ochat-3.5.2/ochat.egg-info/SOURCES.txt` & `ochat-3.6.0/ochat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 .gitignore
 LICENSE
 README.md
 SECURITY.md
 pyproject.toml
 pytest.ini
 .github/workflows/pypi_publish.yaml
+assets/benchmarks-openchat-3.6-20240522.svg
 assets/embeddings.svg
 assets/logo_new.png
+assets/openchat-3.6-20240522.png
 assets/openchat-bench-0106.png
 assets/openchat.png
 assets/openchat_grok.png
 assets/vicuna_gpt35.svg
 assets/vicuna_gpt4.svg
 ochat/__init__.py
 ochat.egg-info/PKG-INFO
@@ -141,14 +143,15 @@
 ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl
 ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl
 ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl
 ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl
 ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl
 ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl
 ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl
+ochat/evaluation/eval_data/zs/gpqa/diamond.jsonl
 ochat/evaluation/eval_data/zs/math/MATH.jsonl
 ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl
 ochat/evaluation/grading/math_grader.py
 ochat/evaluation/grading/math_normalize.py
 ochat/experimental/generate_dataset_old.py
 ochat/experimental/sharegpt.ipynb
 ochat/experimental/test_multipack_dataloader.ipynb
@@ -157,16 +160,18 @@
 ochat/experimental/verify_dataset.ipynb
 ochat/experimental/verify_dataset_orca.ipynb
 ochat/models/__init__.py
 ochat/models/unpadded_gemma.py
 ochat/models/unpadded_llama.py
 ochat/models/unpadded_mistral.py
 ochat/scripts/hf_add_tokens.py
+ochat/scripts/init_special_embedding_llama3.py
 ochat/scripts/modify_eos_embedding.py
 ochat/serving/async_tokenizer.py
 ochat/serving/openai_api_protocol.py
 ochat/serving/openai_api_server.py
 ochat/tests/test_model_config.py
 ochat/training_deepspeed/deepspeed_config.json
+ochat/training_deepspeed/hf_hub.py
 ochat/training_deepspeed/multipack_sampler.py
 ochat/training_deepspeed/openchat_dataset.py
 ochat/training_deepspeed/train.py
```

### Comparing `ochat-3.5.2/pyproject.toml` & `ochat-3.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -11,40 +11,44 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "beautifulsoup4", 
     "markdownify", 
-    "openai", 
+    "pylatexenc",
+    "openai>=1",
     "tenacity", 
     "tiktoken", 
     "tqdm", 
     "wandb", 
     "numba", 
     "datasets", 
     "orjson", 
     "torch", 
+    "packaging",
+    "ninja",
+    "flash-attn",
     "ray", 
     "sentencepiece", 
-    "transformers>=4.38.2", 
+    "transformers>=4.40.1", 
     "accelerate", 
     "protobuf",
     "fastapi", 
     "pydantic", 
     "shortuuid", 
     "uvicorn", 
-    "vllm>=0.3.3",
+    "vllm>=0.4.0",
     "pytest"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/imoneoi/openchat"
 "Bug Tracker" = "https://github.com/imoneoi/openchat/issues"
 
 [tool.setuptools.packages.find]
 exclude = ["assets*", "ochat/experimental*"]
 
 [tool.wheel]
 exclude = ["assets*", "ochat/experimental*"]
 
-[tool.setuptools_scm]
+[tool.setuptools_scm]
```


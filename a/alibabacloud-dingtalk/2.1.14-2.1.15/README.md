# Comparing `tmp/alibabacloud_dingtalk-2.1.14.tar.gz` & `tmp/alibabacloud_dingtalk-2.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.14.tar", last modified: Thu May 23 06:21:27 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.15.tar", last modified: Fri May 24 10:50:54 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.1.14.tar` & `alibabacloud_dingtalk-2.1.15.tar`

### file list

```diff
@@ -1,433 +1,433 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/
--rw-r--r--   0 root         (0) root         (0)   134181 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2575 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2660 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10220 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15463 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24694 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    36448 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25446 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    24061 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51732 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    55896 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11812 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23886 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69836 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   171793 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19974 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25370 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30918 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47170 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31278 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27481 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   114212 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   145728 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   248134 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413198 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53158 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    64382 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6152 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4135 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   306758 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   657929 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98018 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   115937 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11616 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9944 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   192336 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   407651 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34906 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42901 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89960 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   237978 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10504 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88282 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124205 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185660 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   224275 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71002 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   126248 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   408970 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   425714 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25686 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43876 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40206 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44858 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21312 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30666 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23500 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10844 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14576 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6516 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10302 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   315868 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   638801 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5774 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7253 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37328 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46524 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   494304 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515207 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134392 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   150282 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16480 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15793 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70120 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56029 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79025 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81667 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   313048 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   322887 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260012 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   385294 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23366 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   168538 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   200479 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   672294 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   877133 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89270 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113792 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104118 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   121491 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22157 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20888 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   482712 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   556456 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191008 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   320947 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21190 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28705 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42854 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53610 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5681 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5155 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12390 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9744 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98153 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137888 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20603 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18299 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84750 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124476 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   195023 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   271289 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   396886 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413672 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28815 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33507 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107508 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    91958 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   815324 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   937150 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75114 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   157606 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78582 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108065 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   110044 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133326 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11628 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5990 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4381 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18311 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23610 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   181489 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   173547 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62895 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53887 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71486 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    63136 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42982 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44105 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10832 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7243 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107234 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   167406 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93818 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123438 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69184 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    59069 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35028 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68771 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   319400 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   411401 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21787 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30496 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44394 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164608 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172757 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115490 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105876 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   129210 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   167086 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47742 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46647 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   460426 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   551312 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38532 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26120 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54274 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95239 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   226462 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   350226 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70068 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95695 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16918 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28519 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84018 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152968 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17044 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16445 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17118 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22383 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16528 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17427 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91210 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135827 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92596 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   111817 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40437 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40791 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10216 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21704 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79864 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129013 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6226 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8459 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50430 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43338 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   262706 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   457245 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5688 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3678 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   590500 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   761218 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4472 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14334 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/
+-rw-r--r--   0 root         (0) root         (0)   135727 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2575 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2660 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10220 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15463 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24694 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    36448 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25446 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    24061 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51732 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    55896 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11812 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23886 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69836 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   171793 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19974 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25370 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30918 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47170 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31278 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27481 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   114212 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   145728 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   248134 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413198 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53158 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    64382 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6152 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   306758 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   657929 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98018 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   115937 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11616 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   192336 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   407651 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34906 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42901 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89960 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   237978 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10504 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88282 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124205 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185660 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   224275 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71002 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   126248 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   408970 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   425714 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25686 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43876 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40206 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44858 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21312 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30666 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23500 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10844 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14576 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6516 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10302 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   315868 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   638801 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5774 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7253 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37328 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46524 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494304 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515207 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134392 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   150282 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16480 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15793 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70120 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56029 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79025 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81667 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   313048 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   322887 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260012 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   385294 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23366 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   168538 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   200479 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   672294 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   877133 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89270 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113792 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104118 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   121491 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22157 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20888 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   482712 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   556456 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191008 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   320947 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21190 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28705 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42854 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53610 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12390 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98153 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137888 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20603 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18299 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84750 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124476 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   199981 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   276424 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   396886 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413672 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28815 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33507 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107508 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    91958 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   824822 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   952300 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75114 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   157606 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78582 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108065 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   110044 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133326 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11628 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18311 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23610 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   181489 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   173547 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62895 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53887 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71486 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    63136 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42982 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44105 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10832 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107234 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   167406 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93818 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123438 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69184 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    59069 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35028 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68771 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   319400 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   411401 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21787 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30496 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44394 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164608 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172757 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115490 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105876 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129210 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   167086 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47742 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46647 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   460426 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   551312 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38532 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26120 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54274 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95239 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   226462 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   350226 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70068 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95695 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16918 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28519 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84018 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152968 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17044 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16445 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17118 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22383 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16528 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17427 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91210 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135827 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92596 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   111817 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40437 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40791 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10216 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21704 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79864 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129013 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8459 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50430 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43338 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   262706 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   457246 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3678 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   590500 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   761218 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4472 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14334 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-24 10:50:54.000000 alibabacloud_dingtalk-2.1.15/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-05-24 10:50:53.000000 alibabacloud_dingtalk-2.1.15/setup.py
```

### Comparing `alibabacloud_dingtalk-2.1.14/ChangeLog.md` & `alibabacloud_dingtalk-2.1.15/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-05-23 Version: 2.1.14
+- Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-05-22 Version: 2.1.13
 - Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-05-18 Version: 2.1.12
 - Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-05-14 Version: 2.1.11
```

### Comparing `alibabacloud_dingtalk-2.1.14/LICENSE` & `alibabacloud_dingtalk-2.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/PKG-INFO` & `alibabacloud_dingtalk-2.1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.1.14
+Version: 2.1.15
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.14/README-CN.md` & `alibabacloud_dingtalk-2.1.15/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/README.md` & `alibabacloud_dingtalk-2.1.15/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/agoal_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/amdp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -959,14 +959,132 @@
         @param request: GetEmployeeRosterByFieldRequest
         @return: GetEmployeeRosterByFieldResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkhrm__1__0_models.GetEmployeeRosterByFieldHeaders()
         return await self.get_employee_roster_by_field_with_options_async(request, headers, runtime)
 
+    def hrm_auth_resources_query_with_options(
+        self,
+        request: dingtalkhrm__1__0_models.HrmAuthResourcesQueryRequest,
+        headers: dingtalkhrm__1__0_models.HrmAuthResourcesQueryHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.HrmAuthResourcesQueryResponse:
+        """
+        @summary 智能人事权限查询
+        
+        @param request: HrmAuthResourcesQueryRequest
+        @param headers: HrmAuthResourcesQueryHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: HrmAuthResourcesQueryResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.auth_resource_ids):
+            body['authResourceIds'] = request.auth_resource_ids
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='HrmAuthResourcesQuery',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/authResources/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.HrmAuthResourcesQueryResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def hrm_auth_resources_query_with_options_async(
+        self,
+        request: dingtalkhrm__1__0_models.HrmAuthResourcesQueryRequest,
+        headers: dingtalkhrm__1__0_models.HrmAuthResourcesQueryHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.HrmAuthResourcesQueryResponse:
+        """
+        @summary 智能人事权限查询
+        
+        @param request: HrmAuthResourcesQueryRequest
+        @param headers: HrmAuthResourcesQueryHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: HrmAuthResourcesQueryResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.auth_resource_ids):
+            body['authResourceIds'] = request.auth_resource_ids
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='HrmAuthResourcesQuery',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/authResources/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.HrmAuthResourcesQueryResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def hrm_auth_resources_query(
+        self,
+        request: dingtalkhrm__1__0_models.HrmAuthResourcesQueryRequest,
+    ) -> dingtalkhrm__1__0_models.HrmAuthResourcesQueryResponse:
+        """
+        @summary 智能人事权限查询
+        
+        @param request: HrmAuthResourcesQueryRequest
+        @return: HrmAuthResourcesQueryResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.HrmAuthResourcesQueryHeaders()
+        return self.hrm_auth_resources_query_with_options(request, headers, runtime)
+
+    async def hrm_auth_resources_query_async(
+        self,
+        request: dingtalkhrm__1__0_models.HrmAuthResourcesQueryRequest,
+    ) -> dingtalkhrm__1__0_models.HrmAuthResourcesQueryResponse:
+        """
+        @summary 智能人事权限查询
+        
+        @param request: HrmAuthResourcesQueryRequest
+        @return: HrmAuthResourcesQueryResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkhrm__1__0_models.HrmAuthResourcesQueryHeaders()
+        return await self.hrm_auth_resources_query_with_options_async(request, headers, runtime)
+
     def hrm_benefit_query_with_options(
         self,
         request: dingtalkhrm__1__0_models.HrmBenefitQueryRequest,
         headers: dingtalkhrm__1__0_models.HrmBenefitQueryHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkhrm__1__0_models.HrmBenefitQueryResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1713,14 +1713,191 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetEmployeeRosterByFieldResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class HrmAuthResourcesQueryHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class HrmAuthResourcesQueryRequest(TeaModel):
+    def __init__(
+        self,
+        auth_resource_ids: List[str] = None,
+        user_id: str = None,
+    ):
+        # This parameter is required.
+        self.auth_resource_ids = auth_resource_ids
+        # This parameter is required.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_resource_ids is not None:
+            result['authResourceIds'] = self.auth_resource_ids
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('authResourceIds') is not None:
+            self.auth_resource_ids = m.get('authResourceIds')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class HrmAuthResourcesQueryResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        authorized: bool = None,
+        resource_id: str = None,
+    ):
+        self.authorized = authorized
+        self.resource_id = resource_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.authorized is not None:
+            result['authorized'] = self.authorized
+        if self.resource_id is not None:
+            result['resourceId'] = self.resource_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('authorized') is not None:
+            self.authorized = m.get('authorized')
+        if m.get('resourceId') is not None:
+            self.resource_id = m.get('resourceId')
+        return self
+
+
+class HrmAuthResourcesQueryResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[HrmAuthResourcesQueryResponseBodyResult] = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = HrmAuthResourcesQueryResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        return self
+
+
+class HrmAuthResourcesQueryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: HrmAuthResourcesQueryResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = HrmAuthResourcesQueryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class HrmBenefitQueryHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,128 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
+    def batch_get_task_result_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.BatchGetTaskResultRequest,
+        headers: dingtalkindustry__1__0_models.BatchGetTaskResultHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.BatchGetTaskResultResponse:
+        """
+        @summary 批量查询任务结果
+        
+        @param request: BatchGetTaskResultRequest
+        @param headers: BatchGetTaskResultHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: BatchGetTaskResultResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.task_ids):
+            body['taskIds'] = request.task_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchGetTaskResult',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/ai/taskResults/batchQuery',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.BatchGetTaskResultResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def batch_get_task_result_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.BatchGetTaskResultRequest,
+        headers: dingtalkindustry__1__0_models.BatchGetTaskResultHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.BatchGetTaskResultResponse:
+        """
+        @summary 批量查询任务结果
+        
+        @param request: BatchGetTaskResultRequest
+        @param headers: BatchGetTaskResultHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: BatchGetTaskResultResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.task_ids):
+            body['taskIds'] = request.task_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchGetTaskResult',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/ai/taskResults/batchQuery',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.BatchGetTaskResultResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def batch_get_task_result(
+        self,
+        request: dingtalkindustry__1__0_models.BatchGetTaskResultRequest,
+    ) -> dingtalkindustry__1__0_models.BatchGetTaskResultResponse:
+        """
+        @summary 批量查询任务结果
+        
+        @param request: BatchGetTaskResultRequest
+        @return: BatchGetTaskResultResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.BatchGetTaskResultHeaders()
+        return self.batch_get_task_result_with_options(request, headers, runtime)
+
+    async def batch_get_task_result_async(
+        self,
+        request: dingtalkindustry__1__0_models.BatchGetTaskResultRequest,
+    ) -> dingtalkindustry__1__0_models.BatchGetTaskResultResponse:
+        """
+        @summary 批量查询任务结果
+        
+        @param request: BatchGetTaskResultRequest
+        @return: BatchGetTaskResultResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.BatchGetTaskResultHeaders()
+        return await self.batch_get_task_result_with_options_async(request, headers, runtime)
+
     def business_match_with_options(
         self,
         request: dingtalkindustry__1__0_models.BusinessMatchRequest,
         headers: dingtalkindustry__1__0_models.BusinessMatchHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkindustry__1__0_models.BusinessMatchResponse:
         """
@@ -15501,14 +15615,136 @@
         @param request: SaveUserExtendValuesRequest
         @return: SaveUserExtendValuesResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkindustry__1__0_models.SaveUserExtendValuesHeaders()
         return await self.save_user_extend_values_with_options_async(user_id, request, headers, runtime)
 
+    def submit_task_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SubmitTaskRequest,
+        headers: dingtalkindustry__1__0_models.SubmitTaskHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SubmitTaskResponse:
+        """
+        @summary 提交ai解析任务
+        
+        @param request: SubmitTaskRequest
+        @param headers: SubmitTaskHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SubmitTaskResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_id):
+            body['appId'] = request.app_id
+        if not UtilClient.is_unset(request.biz_code):
+            body['bizCode'] = request.biz_code
+        if not UtilClient.is_unset(request.data):
+            body['data'] = request.data
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SubmitTask',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/ai/tasks/submit',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SubmitTaskResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def submit_task_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SubmitTaskRequest,
+        headers: dingtalkindustry__1__0_models.SubmitTaskHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SubmitTaskResponse:
+        """
+        @summary 提交ai解析任务
+        
+        @param request: SubmitTaskRequest
+        @param headers: SubmitTaskHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SubmitTaskResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_id):
+            body['appId'] = request.app_id
+        if not UtilClient.is_unset(request.biz_code):
+            body['bizCode'] = request.biz_code
+        if not UtilClient.is_unset(request.data):
+            body['data'] = request.data
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SubmitTask',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/ai/tasks/submit',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SubmitTaskResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def submit_task(
+        self,
+        request: dingtalkindustry__1__0_models.SubmitTaskRequest,
+    ) -> dingtalkindustry__1__0_models.SubmitTaskResponse:
+        """
+        @summary 提交ai解析任务
+        
+        @param request: SubmitTaskRequest
+        @return: SubmitTaskResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SubmitTaskHeaders()
+        return self.submit_task_with_options(request, headers, runtime)
+
+    async def submit_task_async(
+        self,
+        request: dingtalkindustry__1__0_models.SubmitTaskRequest,
+    ) -> dingtalkindustry__1__0_models.SubmitTaskResponse:
+        """
+        @summary 提交ai解析任务
+        
+        @param request: SubmitTaskRequest
+        @return: SubmitTaskResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SubmitTaskHeaders()
+        return await self.submit_task_with_options_async(request, headers, runtime)
+
     def suppl_add_role_with_options(
         self,
         request: dingtalkindustry__1__0_models.SupplAddRoleRequest,
         headers: dingtalkindustry__1__0_models.SupplAddRoleHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkindustry__1__0_models.SupplAddRoleResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,300 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List, Any
 
 
+class BatchGetTaskResultHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class BatchGetTaskResultRequest(TeaModel):
+    def __init__(
+        self,
+        task_ids: List[str] = None,
+    ):
+        self.task_ids = task_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.task_ids is not None:
+            result['taskIds'] = self.task_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('taskIds') is not None:
+            self.task_ids = m.get('taskIds')
+        return self
+
+
+class BatchGetTaskResultResponseBodyTasksResultItems(TeaModel):
+    def __init__(
+        self,
+        info: str = None,
+        name: str = None,
+        point: int = None,
+    ):
+        self.info = info
+        self.name = name
+        self.point = point
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.info is not None:
+            result['info'] = self.info
+        if self.name is not None:
+            result['name'] = self.name
+        if self.point is not None:
+            result['point'] = self.point
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('info') is not None:
+            self.info = m.get('info')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('point') is not None:
+            self.point = m.get('point')
+        return self
+
+
+class BatchGetTaskResultResponseBodyTasksResult(TeaModel):
+    def __init__(
+        self,
+        audio_text: str = None,
+        date: str = None,
+        desc: str = None,
+        id: int = None,
+        items: List[BatchGetTaskResultResponseBodyTasksResultItems] = None,
+        name: str = None,
+        total: int = None,
+    ):
+        self.audio_text = audio_text
+        self.date = date
+        self.desc = desc
+        self.id = id
+        self.items = items
+        self.name = name
+        self.total = total
+
+    def validate(self):
+        if self.items:
+            for k in self.items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.audio_text is not None:
+            result['audioText'] = self.audio_text
+        if self.date is not None:
+            result['date'] = self.date
+        if self.desc is not None:
+            result['desc'] = self.desc
+        if self.id is not None:
+            result['id'] = self.id
+        result['items'] = []
+        if self.items is not None:
+            for k in self.items:
+                result['items'].append(k.to_map() if k else None)
+        if self.name is not None:
+            result['name'] = self.name
+        if self.total is not None:
+            result['total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('audioText') is not None:
+            self.audio_text = m.get('audioText')
+        if m.get('date') is not None:
+            self.date = m.get('date')
+        if m.get('desc') is not None:
+            self.desc = m.get('desc')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        self.items = []
+        if m.get('items') is not None:
+            for k in m.get('items'):
+                temp_model = BatchGetTaskResultResponseBodyTasksResultItems()
+                self.items.append(temp_model.from_map(k))
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        return self
+
+
+class BatchGetTaskResultResponseBodyTasks(TeaModel):
+    def __init__(
+        self,
+        result: BatchGetTaskResultResponseBodyTasksResult = None,
+        status: str = None,
+        task_id: str = None,
+    ):
+        self.result = result
+        self.status = status
+        self.task_id = task_id
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.status is not None:
+            result['status'] = self.status
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = BatchGetTaskResultResponseBodyTasksResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        return self
+
+
+class BatchGetTaskResultResponseBody(TeaModel):
+    def __init__(
+        self,
+        tasks: List[BatchGetTaskResultResponseBodyTasks] = None,
+    ):
+        self.tasks = tasks
+
+    def validate(self):
+        if self.tasks:
+            for k in self.tasks:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['tasks'] = []
+        if self.tasks is not None:
+            for k in self.tasks:
+                result['tasks'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.tasks = []
+        if m.get('tasks') is not None:
+            for k in m.get('tasks'):
+                temp_model = BatchGetTaskResultResponseBodyTasks()
+                self.tasks.append(temp_model.from_map(k))
+        return self
+
+
+class BatchGetTaskResultResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BatchGetTaskResultResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = BatchGetTaskResultResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BusinessMatchHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -25741,14 +26028,260 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SaveUserExtendValuesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SubmitTaskHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SubmitTaskRequestData(TeaModel):
+    def __init__(
+        self,
+        date: str = None,
+        desc: str = None,
+        file_type: str = None,
+        file_url: List[str] = None,
+        id: int = None,
+        name: str = None,
+    ):
+        self.date = date
+        self.desc = desc
+        self.file_type = file_type
+        self.file_url = file_url
+        self.id = id
+        self.name = name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.date is not None:
+            result['date'] = self.date
+        if self.desc is not None:
+            result['desc'] = self.desc
+        if self.file_type is not None:
+            result['fileType'] = self.file_type
+        if self.file_url is not None:
+            result['fileUrl'] = self.file_url
+        if self.id is not None:
+            result['id'] = self.id
+        if self.name is not None:
+            result['name'] = self.name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('date') is not None:
+            self.date = m.get('date')
+        if m.get('desc') is not None:
+            self.desc = m.get('desc')
+        if m.get('fileType') is not None:
+            self.file_type = m.get('fileType')
+        if m.get('fileUrl') is not None:
+            self.file_url = m.get('fileUrl')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        return self
+
+
+class SubmitTaskRequest(TeaModel):
+    def __init__(
+        self,
+        app_id: int = None,
+        biz_code: str = None,
+        data: List[SubmitTaskRequestData] = None,
+    ):
+        self.app_id = app_id
+        self.biz_code = biz_code
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_id is not None:
+            result['appId'] = self.app_id
+        if self.biz_code is not None:
+            result['bizCode'] = self.biz_code
+        result['data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['data'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('appId') is not None:
+            self.app_id = m.get('appId')
+        if m.get('bizCode') is not None:
+            self.biz_code = m.get('bizCode')
+        self.data = []
+        if m.get('data') is not None:
+            for k in m.get('data'):
+                temp_model = SubmitTaskRequestData()
+                self.data.append(temp_model.from_map(k))
+        return self
+
+
+class SubmitTaskResponseBodyTasks(TeaModel):
+    def __init__(
+        self,
+        id: int = None,
+        task_id: str = None,
+    ):
+        self.id = id
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['id'] = self.id
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        return self
+
+
+class SubmitTaskResponseBody(TeaModel):
+    def __init__(
+        self,
+        tasks: List[SubmitTaskResponseBodyTasks] = None,
+    ):
+        self.tasks = tasks
+
+    def validate(self):
+        if self.tasks:
+            for k in self.tasks:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['tasks'] = []
+        if self.tasks is not None:
+            for k in self.tasks:
+                result['tasks'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.tasks = []
+        if m.get('tasks') is not None:
+            for k in m.get('tasks'):
+                temp_model = SubmitTaskResponseBodyTasks()
+                self.tasks.append(temp_model.from_map(k))
+        return self
+
+
+class SubmitTaskResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SubmitTaskResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SubmitTaskResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SupplAddRoleHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13826,15 +13826,15 @@
             self.user_id = m.get('userId')
         return self
 
 
 class TodoTasksResponseBodyResult(TeaModel):
     def __init__(
         self,
-        has_more: str = None,
+        has_more: bool = None,
         list: List[TodoTasksResponseBodyResultList] = None,
     ):
         self.has_more = has_more
         self.list = list
 
     def validate(self):
         if self.list:
```

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.1.14
+Version: 2.1.15
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.1.15/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.14/setup.py` & `alibabacloud_dingtalk-2.1.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 23/05/2024
+Created on 24/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```


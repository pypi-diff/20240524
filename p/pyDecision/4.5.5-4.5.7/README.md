# Comparing `tmp/pyDecision-4.5.5.tar.gz` & `tmp/pyDecision-4.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-4.5.5.tar", last modified: Mon May 20 01:14:40 2024, max compression
+gzip compressed data, was "dist\pyDecision-4.5.7.tar", last modified: Fri May 24 01:47:40 2024, max compression
```

## Comparing `pyDecision-4.5.5.tar` & `pyDecision-4.5.7.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 01:14:40.000000 pyDecision-4.5.5/
--rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.5.5/LICENSE
--rw-rw-rw-   0        0        0    21036 2024-05-20 01:14:40.000000 pyDecision-4.5.5/PKG-INFO
--rw-rw-rw-   0        0        0    20530 2024-05-20 01:12:36.000000 pyDecision-4.5.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 01:14:39.000000 pyDecision-4.5.5/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.5.5/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:14:40.000000 pyDecision-4.5.5/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     3346 2024-05-20 01:04:37.000000 pyDecision-4.5.5/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1667 2024-05-18 20:21:19.000000 pyDecision-4.5.5/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.5.5/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.5.5/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.5.5/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.5.5/pyDecision/algorithm/bwm_s.py
--rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.5.5/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.5.5/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.5.5/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.5.5/pyDecision/algorithm/copeland.py
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.5.5/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.5.5/pyDecision/algorithm/cradis.py
--rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.5.5/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.5.5/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.5.5/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.5.5/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.5.5/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.5.5/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.5.5/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.5.5/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.5.5/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2764 2024-05-16 23:15:46.000000 pyDecision-4.5.5/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.5.5/pyDecision/algorithm/entropy.py
--rw-rw-rw-   0        0        0     2289 2024-04-24 15:29:47.000000 pyDecision-4.5.5/pyDecision/algorithm/fucom.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     2873 2024-05-20 00:52:49.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ahp_ppf.py
--rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_aras.py
--rw-rw-rw-   0        0        0     4635 2023-11-12 11:24:00.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_bwm.py
--rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_copras.py
--rw-rw-rw-   0        0        0     2500 2024-04-26 21:40:48.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_critic.py
--rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     5402 2024-04-27 00:21:30.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_fucom.py
--rw-rw-rw-   0        0        0     1786 2024-04-26 21:41:04.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_merec.py
--rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_moora.py
--rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ocra.py
--rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.5.5/pyDecision/algorithm/fuzzy_waspas.py
--rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.5.5/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.5.5/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.5.5/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.5.5/pyDecision/algorithm/macbeth.py
--rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.5.5/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     2598 2024-04-25 15:20:07.000000 pyDecision-4.5.5/pyDecision/algorithm/mara.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.5.5/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.5.5/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.5.5/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.5.5/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.5.5/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.5.5/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.5.5/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     5101 2024-05-20 01:01:36.000000 pyDecision-4.5.5/pyDecision/algorithm/opa.py
--rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.5.5/pyDecision/algorithm/oreste.py
--rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.5.5/pyDecision/algorithm/p_ec.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.5.5/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.5.5/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.5.5/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.5.5/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.5.5/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.5.5/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.5.5/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.5.5/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.5.5/pyDecision/algorithm/psi.py
--rw-rw-rw-   0        0        0      688 2024-04-25 15:23:46.000000 pyDecision-4.5.5/pyDecision/algorithm/psi_m.py
--rw-rw-rw-   0        0        0     3243 2024-04-28 14:55:21.000000 pyDecision-4.5.5/pyDecision/algorithm/rafsi.py
--rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:15.000000 pyDecision-4.5.5/pyDecision/algorithm/regime.py
--rw-rw-rw-   0        0        0      969 2024-04-26 21:38:23.000000 pyDecision-4.5.5/pyDecision/algorithm/roc.py
--rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.5.5/pyDecision/algorithm/rov.py
--rw-rw-rw-   0        0        0      970 2024-04-26 21:39:12.000000 pyDecision-4.5.5/pyDecision/algorithm/rrw.py
--rw-rw-rw-   0        0        0      929 2024-04-26 21:38:49.000000 pyDecision-4.5.5/pyDecision/algorithm/rsw.py
--rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.5.5/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     1991 2024-04-27 19:45:13.000000 pyDecision-4.5.5/pyDecision/algorithm/seca.py
--rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.5.5/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.5.5/pyDecision/algorithm/spotis.py
--rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.5.5/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.5.5/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.5.5/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.5.5/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2687 2024-05-01 01:06:43.000000 pyDecision-4.5.5/pyDecision/algorithm/wings.py
--rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.5.5/pyDecision/algorithm/wisp.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:14:40.000000 pyDecision-4.5.5/pyDecision/compare/
--rw-rw-rw-   0        0        0      127 2024-04-27 00:17:39.000000 pyDecision-4.5.5/pyDecision/compare/__init__.py
--rw-rw-rw-   0        0        0    26816 2024-04-28 14:47:45.000000 pyDecision-4.5.5/pyDecision/compare/compare.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:14:40.000000 pyDecision-4.5.5/pyDecision/util/
--rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.5.5/pyDecision/util/LLM.py
--rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.5.5/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.5.5/pyDecision/util/ga.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:14:39.000000 pyDecision-4.5.5/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    21036 2024-05-20 01:14:37.000000 pyDecision-4.5.5/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2867 2024-05-20 01:14:38.000000 pyDecision-4.5.5/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 01:14:37.000000 pyDecision-4.5.5/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-20 01:14:37.000000 pyDecision-4.5.5/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 01:14:37.000000 pyDecision-4.5.5/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 01:14:40.000000 pyDecision-4.5.5/setup.cfg
--rw-rw-rw-   0        0        0      744 2024-05-20 01:05:15.000000 pyDecision-4.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:47:40.000000 pyDecision-4.5.7/
+-rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.5.7/LICENSE
+-rw-rw-rw-   0        0        0    21036 2024-05-24 01:47:40.000000 pyDecision-4.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0    20530 2024-05-20 01:12:36.000000 pyDecision-4.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 01:47:39.000000 pyDecision-4.5.7/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.5.7/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:47:40.000000 pyDecision-4.5.7/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     3346 2024-05-20 01:04:37.000000 pyDecision-4.5.7/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1667 2024-05-18 20:21:19.000000 pyDecision-4.5.7/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.5.7/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.5.7/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.5.7/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.5.7/pyDecision/algorithm/bwm_s.py
+-rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.5.7/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.5.7/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.5.7/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.5.7/pyDecision/algorithm/copeland.py
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.5.7/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.5.7/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.5.7/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.5.7/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.5.7/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.5.7/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.5.7/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.5.7/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.5.7/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.5.7/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.5.7/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2764 2024-05-16 23:15:46.000000 pyDecision-4.5.7/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.5.7/pyDecision/algorithm/entropy.py
+-rw-rw-rw-   0        0        0     2289 2024-04-24 15:29:47.000000 pyDecision-4.5.7/pyDecision/algorithm/fucom.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     2924 2024-05-24 01:45:07.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_ahp_ppf.py
+-rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_aras.py
+-rw-rw-rw-   0        0        0     5638 2024-05-24 01:46:10.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_bwm.py
+-rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_copras.py
+-rw-rw-rw-   0        0        0     2500 2024-04-26 21:40:48.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_critic.py
+-rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     5402 2024-04-27 00:21:30.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_fucom.py
+-rw-rw-rw-   0        0        0     1786 2024-04-26 21:41:04.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_merec.py
+-rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_moora.py
+-rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_ocra.py
+-rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.5.7/pyDecision/algorithm/fuzzy_waspas.py
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.5.7/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.5.7/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.5.7/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.5.7/pyDecision/algorithm/macbeth.py
+-rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.5.7/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     2598 2024-04-25 15:20:07.000000 pyDecision-4.5.7/pyDecision/algorithm/mara.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.5.7/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.5.7/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.5.7/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.5.7/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.5.7/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.5.7/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.5.7/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     5101 2024-05-20 01:01:36.000000 pyDecision-4.5.7/pyDecision/algorithm/opa.py
+-rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.5.7/pyDecision/algorithm/oreste.py
+-rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.5.7/pyDecision/algorithm/p_ec.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.5.7/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.5.7/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.5.7/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.5.7/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.5.7/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.5.7/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.5.7/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.5.7/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.5.7/pyDecision/algorithm/psi.py
+-rw-rw-rw-   0        0        0      688 2024-04-25 15:23:46.000000 pyDecision-4.5.7/pyDecision/algorithm/psi_m.py
+-rw-rw-rw-   0        0        0     3243 2024-04-28 14:55:21.000000 pyDecision-4.5.7/pyDecision/algorithm/rafsi.py
+-rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:15.000000 pyDecision-4.5.7/pyDecision/algorithm/regime.py
+-rw-rw-rw-   0        0        0      969 2024-04-26 21:38:23.000000 pyDecision-4.5.7/pyDecision/algorithm/roc.py
+-rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.5.7/pyDecision/algorithm/rov.py
+-rw-rw-rw-   0        0        0      970 2024-04-26 21:39:12.000000 pyDecision-4.5.7/pyDecision/algorithm/rrw.py
+-rw-rw-rw-   0        0        0      929 2024-04-26 21:38:49.000000 pyDecision-4.5.7/pyDecision/algorithm/rsw.py
+-rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.5.7/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     1991 2024-04-27 19:45:13.000000 pyDecision-4.5.7/pyDecision/algorithm/seca.py
+-rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.5.7/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.5.7/pyDecision/algorithm/spotis.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.5.7/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.5.7/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.5.7/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.5.7/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2687 2024-05-01 01:06:43.000000 pyDecision-4.5.7/pyDecision/algorithm/wings.py
+-rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.5.7/pyDecision/algorithm/wisp.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:47:40.000000 pyDecision-4.5.7/pyDecision/compare/
+-rw-rw-rw-   0        0        0      127 2024-04-27 00:17:39.000000 pyDecision-4.5.7/pyDecision/compare/__init__.py
+-rw-rw-rw-   0        0        0    26816 2024-04-28 14:47:45.000000 pyDecision-4.5.7/pyDecision/compare/compare.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:47:40.000000 pyDecision-4.5.7/pyDecision/util/
+-rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.5.7/pyDecision/util/LLM.py
+-rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.5.7/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.5.7/pyDecision/util/ga.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:47:39.000000 pyDecision-4.5.7/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    21036 2024-05-24 01:47:38.000000 pyDecision-4.5.7/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2867 2024-05-24 01:47:39.000000 pyDecision-4.5.7/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 01:47:38.000000 pyDecision-4.5.7/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-24 01:47:38.000000 pyDecision-4.5.7/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 01:47:38.000000 pyDecision-4.5.7/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 01:47:40.000000 pyDecision-4.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      744 2024-05-24 01:46:47.000000 pyDecision-4.5.7/setup.py
```

### Comparing `pyDecision-4.5.5/LICENSE` & `pyDecision-4.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/PKG-INFO` & `pyDecision-4.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.5.5
+Version: 4.5.7
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyDecision-4.5.5/README.md` & `pyDecision-4.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/__init__.py` & `pyDecision-4.5.7/pyDecision/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/ahp.py` & `pyDecision-4.5.7/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/aras.py` & `pyDecision-4.5.7/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/borda.py` & `pyDecision-4.5.7/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/bwm.py` & `pyDecision-4.5.7/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/bwm_s.py` & `pyDecision-4.5.7/pyDecision/algorithm/bwm_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/cilos.py` & `pyDecision-4.5.7/pyDecision/algorithm/cilos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/cocoso.py` & `pyDecision-4.5.7/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/codas.py` & `pyDecision-4.5.7/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/copeland.py` & `pyDecision-4.5.7/pyDecision/algorithm/copeland.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/copras.py` & `pyDecision-4.5.7/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/cradis.py` & `pyDecision-4.5.7/pyDecision/algorithm/cradis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/critic.py` & `pyDecision-4.5.7/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/dematel.py` & `pyDecision-4.5.7/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/e_i.py` & `pyDecision-4.5.7/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/e_i_s.py` & `pyDecision-4.5.7/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/e_i_v.py` & `pyDecision-4.5.7/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/e_ii.py` & `pyDecision-4.5.7/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/e_iii.py` & `pyDecision-4.5.7/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/e_iv.py` & `pyDecision-4.5.7/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/e_tri_b.py` & `pyDecision-4.5.7/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/edas.py` & `pyDecision-4.5.7/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/entropy.py` & `pyDecision-4.5.7/pyDecision/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fucom.py` & `pyDecision-4.5.7/pyDecision/algorithm/fucom.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ahp_ppf.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_ahp_ppf.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                     if (score > 0):
                         crisp_matrix[i, j] = score
                     else:
                         crisp_matrix[i, j] = score_n
         return crisp_matrix
     
     def normalize_matrix(crisp_matrix):
-        n_matrix = crisp_matrix / crisp_matrix.sum(axis = 0)
+        n_matrix = np.abs(crisp_matrix) / crisp_matrix.sum(axis = 0)
         return n_matrix
 
     def consistency_ratio(crisp_matrix):
         eigenvalues, eigenvectors = np.linalg.eig(crisp_matrix)
         eigenvalues_real          = np.real(eigenvalues)
         lamb_max_index            = np.argmax(eigenvalues_real)
         lamb_max                  = eigenvalues_real[lamb_max_index]
@@ -59,11 +59,12 @@
         return weights
     ################################################
 
     triple_matrix = ppf_to_triple(comparison_matrix)
     crisp_matrix  = triple_to_crisp(triple_matrix)
     n_matrix      = normalize_matrix(crisp_matrix)
     weights       = calculate_weights(n_matrix)
+    weights       = weights/np.sum(weights)
     rc            = consistency_ratio(crisp_matrix)
     return weights, rc
 
-###############################################################################
+###############################################################################
```

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_aras.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_bwm.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_fucom.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,112 +1,122 @@
 ###############################################################################
 
 # Required Libraries
 import numpy as np
+import re
 import warnings
 warnings.filterwarnings('ignore', message = 'delta_grad == 0.0. Check if the approximated')
+warnings.filterwarnings('ignore', message = 'Values in x were outside bounds during a minimize step, clipping to bounds')
 
-from scipy.optimize import minimize, Bounds
+from scipy.optimize import minimize, Bounds, LinearConstraint, NonlinearConstraint
 
 ###############################################################################
 
-# Function: Fuzzy BWM
-def fuzzy_bw_method(mic, lic, eps_penalty = 1, verbose = True): 
-    priority_tuples = [(7/2, 4, 9/2), (5/2, 3, 7/2), (3/2, 2, 5/2), (2/3, 1, 3/2), (1, 1, 1)]
-    ci              = [8.04, 6.69, 5.29, 3.8, 3.0 ]
-    tuple_to_ci     = dict(zip(priority_tuples, ci))
-    
-    ###############################################
-    
-    def find_index(criteria_list, priority_tuples):
-        for tup in priority_tuples:
-            if tup in criteria_list:
-                return criteria_list.index(tup)
-        return None
-    
-    ###############################################
-    
-    ib       = find_index(mic, priority_tuples)
-    iw       = find_index(lic, priority_tuples)
-    ci_value = tuple_to_ci.get(mic[ib])
-    pairs_w  = [(iw, i) for i in range(0, len(lic)) if i != iw]
-    pairs_b  = [(i, ib) for i in range(0, len(mic)) if i != ib and i != iw]
-   
+# Function: Fuzzy FUCOM (Full Consistency Method)
+def fuzzy_fucom_method(criteria_rank, criteria_priority, n_starts = 250, sort_criteria = True, verbose = True):
+    
     ################################################
-   
-    def operation(wv, eps, vector, idx_a = 2, idx_b = 0, idx_m = 0):
-        a, b, c = wv[idx_a]
-        d, e, f = wv[idx_b]
-        fn      = (a - vector[idx_m][0]*f - eps*f, b - vector[idx_m][1]*e - eps*e, c - vector[idx_m][2]*d - eps*d)
-        return fn
     
-    def target_function(variables):
-        eps     = variables[-1] 
-        cn1     = []
-        wv      = [(1, 1, 1) for item in mic]
-        penalty = 0
-        j       = 0
-        for i in range(0, len(wv)):
-            wv[i] = (variables[j], variables[j+1], variables[j+2])
-            j     = j + 3
-        for i in range(0, len(pairs_w)):
-            a, b, c = operation(wv = wv, eps = eps, vector = mic, idx_a = pairs_w[i][0], idx_b = pairs_w[i][1], idx_m = i)
-            cn1.append( a)
-            cn1.append( b)
-            cn1.append( c)
-            cn1.append(-a)
-            cn1.append(-b)
-            cn1.append(-c)
-        for i in range(0, len(pairs_b)):
-            a, b, c = operation(wv = wv, eps = eps, vector = lic, idx_a = pairs_b[i][0], idx_b = pairs_b[i][1], idx_m = i)
-            cn1.append( a)
-            cn1.append( b)
-            cn1.append( c)
-            cn1.append(-a)
-            cn1.append(-b)
-            cn1.append(-c)
-        for item in cn1:
-            if (item > eps):
-                penalty = penalty + abs(item - eps) * 1
-        penalty = penalty + eps * eps_penalty
-        return penalty
-
-    def one_constraint(variables):
-        wv  = [(variables[i], variables[i+1], variables[i+2]) for i in range(0, len(variables) - 1, 3)]
-        cn2 = [(w[0] + 4*w[1] + w[2])/6 for w in wv]
-        return sum(cn2) - 1  
-    
-    def LMU_constraint(variables):
-        constraints = []
-        for i in range(0, len(variables) - 1, 3):
-            L, m, u = variables[i], variables[i+1], variables[i+2]
-            constraints.append(L)  
-            constraints.append(m - L)  
-            constraints.append(u - m)
-        return constraints
-   
-    constraint_1 = {'type': 'eq',   'fun': one_constraint}
-    constraint_2 = {'type': 'ineq', 'fun': LMU_constraint}
-    constraints  = [constraint_1, constraint_2]
+    def extract_number(text):
+        match = re.search(r'\d+', text)
+        return int(match.group()) if match else None
+    
+    def generate_ordered_triplets(num_criteria):
+        variables = np.zeros(3 * num_criteria)
+        for i in range(0, num_criteria):
+            x1                   = np.random.uniform(low = 0.0001, high = 1.0)
+            x2                   = np.random.uniform(low = x1,    high = 1.0)
+            x3                   = np.random.uniform(low = x2,    high = 1.0)
+            variables[3 * i]     = x1
+            variables[3 * i + 1] = x2
+            variables[3 * i + 2] = x3
+        fuzzy_set = [(variables[i], variables[i + 1], variables[i + 2]) for i in range(0, len(variables), 3)]
+        weights   = np.array([(a + 4 * b + c) / 6 for a, b, c in fuzzy_set])
+        total     = np.sum(weights)
+        scale_fac = 1 / total
+        variables = variables * scale_fac
+        return variables
     
     ################################################
     
-    np.random.seed(42)
-    variables  = np.random.uniform(low = 0.001, high = 1.0, size = len(mic)*3)
-    variables_ = []
-    for i in range(0, len(variables), 3):
-        group   = variables[i:i+3]
-        s_group = np.sort(group)
-        variables_.extend(s_group)
-    variables = np.array([item for item in variables_])
-    variables = np.append(variables, [0])
-    bounds    = Bounds([0]*len(mic)*3 + [0], [1]*len(mic)*3 + [1])
-    results   = minimize(target_function, variables, method = 'trust-constr', bounds = bounds, constraints = constraints)
-    f_weights = results.x[:-1]
-    f_weights = [(f_weights[i], f_weights[i+1], f_weights[i+2]) for i in range(0, len(f_weights) - 1, 3)]
-    weights   = [(w[0] + 4*w[1] + w[2])/6 for w in f_weights]
+    def target_function(variables):
+        fuzzy_set       = [(variables[i], variables[i + 1], variables[i + 2]) for i in range(0, len(variables), 3)]
+        skip            = 1
+        pairs_1         = [(i, i + skip) for i in range(len(fuzzy_set) - skip)]
+        comparative_imp = []
+        for i, j in pairs_1:
+            a, b, c = criteria_priority[j]
+            d, e, f = criteria_priority[i]
+            comparative_imp.append((a/f, b/e, c/d))
+        pairs_2         = [(i, i + skip) for i in range(len(comparative_imp) - skip)]
+        for i, j in pairs_2:
+            a, b, c = comparative_imp[i]
+            d, e, f = comparative_imp[j]
+            comparative_imp.append((a*d, b*e, c*f))
+        chi             = []
+        skip            = 2
+        pairs_3         = [(i, i + skip) for i in range(len(fuzzy_set) - skip)]
+        pairs           = pairs_1 + pairs_3
+        count           = 0
+        for i, j in pairs:
+            a, b, c = fuzzy_set[i]
+            d, e, f = fuzzy_set[j]
+            x, y, z = comparative_imp[count]
+            count   = count + 1
+            chi.append( abs((a / f) - x) ) 
+            chi.append( abs((b / e) - y) )
+            chi.append( abs((c / d) - z) ) 
+        return np.max(chi)
+    
+    def weights_constraint(variables):
+        fuzzy_set = [(variables[i], variables[i + 1], variables[i + 2]) for i in range(0, len(variables), 3)]
+        w         = [(a + 4 * b + c) / 6 for a, b, c in fuzzy_set]
+        return np.sum(w)
+
+    ################################################
+
+    lower_bounds  = []
+    upper_bounds  = []
+    for i in range(0, len(criteria_priority) * 3, 3):
+        lower_bounds = lower_bounds + [0.0001, 0.0001, 0.0001]
+        upper_bounds = upper_bounds + [1, 1, 1]
+    bounds        = Bounds(lower_bounds, upper_bounds)
+    constraints_1 = NonlinearConstraint(weights_constraint, 1, 1)
+    const_matrix  = []
+    constraint_lb = []
+    constraint_ub = []
+    for i in range(0, len(criteria_priority) * 3, 3):
+        row        = np.zeros(len(criteria_priority) * 3)
+        row[i]     = -1
+        row[i + 1] =  1
+        const_matrix.append(row)
+        constraint_lb.append(0)
+        constraint_ub.append(np.inf)
+        row        = np.zeros(len(criteria_priority)*3)
+        row[i + 1] = -1
+        row[i + 2] =  1
+        const_matrix.append(row)
+        constraint_lb.append(0)
+        constraint_ub.append(np.inf)
+    constraints_2 = LinearConstraint(const_matrix, constraint_lb, constraint_ub)
+    chi           = np.inf
+    solution      = None
+    for i in range(0, n_starts):  
+        if (i == 0):
+            guess = generate_ordered_triplets(len(criteria_priority))
+        else:
+            guess = solution
+        result = minimize(target_function, guess, method = 'SLSQP', constraints = [constraints_1, constraints_2], bounds = bounds)
+        if (result.fun < chi):
+            chi      = result.fun
+            solution = result.x
+    f_weights     = [(solution[i], solution[i + 1], solution[i + 2]) for i in range(0, len(solution), 3)]
+    weights       = [(a + 4 * b + c) / 6 for a, b, c in f_weights]
+    if (sort_criteria == True):
+        idx       = sorted(range(0, len(criteria_rank)), key = lambda x: extract_number(criteria_rank[x]))
+        f_weights = [f_weights[i] for i in idx]
+        weights   = [  weights[i] for i in idx]
     if (verbose == True):
-        print('Epsilon Value:', np.round(results.x[-1], 4)) 
-        print('CR: ', np.round(results.x[-1]/ci_value , 4))
-    return  results.x[-1], results.x[-1]/ci_value, f_weights, weights
+        print('Chi:', np.round(chi, 4))
+    return f_weights, weights
 
-###############################################################################
+###############################################################################
```

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_copras.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_critic.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_fucom.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_bwm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,122 +1,133 @@
 ###############################################################################
 
 # Required Libraries
 import numpy as np
-import re
 import warnings
 warnings.filterwarnings('ignore', message = 'delta_grad == 0.0. Check if the approximated')
 warnings.filterwarnings('ignore', message = 'Values in x were outside bounds during a minimize step, clipping to bounds')
 
-from scipy.optimize import minimize, Bounds, LinearConstraint, NonlinearConstraint
+from scipy.optimize import minimize, Bounds, NonlinearConstraint
 
 ###############################################################################
 
-# Function: Fuzzy FUCOM (Full Consistency Method)
-def fuzzy_fucom_method(criteria_rank, criteria_priority, n_starts = 250, sort_criteria = True, verbose = True):
-    
-    ################################################
-    
-    def extract_number(text):
-        match = re.search(r'\d+', text)
-        return int(match.group()) if match else None
+# Function: Fuzzy BWM
+def fuzzy_bw_method(mic, lic, eps_penalty = 1, verbose = True): 
+    priority_tuples = [(7/2, 4, 9/2), (5/2, 3, 7/2), (3/2, 2, 5/2), (2/3, 1, 3/2), (1, 1, 1)]
+    ci              = [8.04, 6.69, 5.29, 3.8, 3.0 ]
+    tuple_to_ci     = dict(zip(priority_tuples, ci))
+    
+    ###############################################
+    
+    def find_index(criteria_list, priority_tuples):
+        for tup in priority_tuples:
+            if tup in criteria_list:
+                return criteria_list.index(tup)
+        return None
     
     def generate_ordered_triplets(num_criteria):
         variables = np.zeros(3 * num_criteria)
         for i in range(0, num_criteria):
             x1                   = np.random.uniform(low = 0.0001, high = 1.0)
-            x2                   = np.random.uniform(low = x1,    high = 1.0)
-            x3                   = np.random.uniform(low = x2,    high = 1.0)
+            x2                   = np.random.uniform(low = x1,     high = 1.0)
+            x3                   = np.random.uniform(low = x2,     high = 1.0)
             variables[3 * i]     = x1
             variables[3 * i + 1] = x2
             variables[3 * i + 2] = x3
         fuzzy_set = [(variables[i], variables[i + 1], variables[i + 2]) for i in range(0, len(variables), 3)]
         weights   = np.array([(a + 4 * b + c) / 6 for a, b, c in fuzzy_set])
         total     = np.sum(weights)
         scale_fac = 1 / total
         variables = variables * scale_fac
         return variables
     
+    ###############################################
+    
+    ib       = find_index(mic, priority_tuples)
+    iw       = find_index(lic, priority_tuples)
+    ci_value = tuple_to_ci.get(mic[ib])
+    pairs_w  = [(iw, i) for i in range(0, len(lic)) if i != iw]
+    pairs_b  = [(i, ib) for i in range(0, len(mic)) if i != ib and i != iw]
+   
     ################################################
+   
+    def operation(wv, eps, vector, idx_a = 2, idx_b = 0, idx_m = 0):
+        a, b, c = wv[idx_a]
+        d, e, f = wv[idx_b]
+        fn      = (a - vector[idx_m][0]*f - eps*f, b - vector[idx_m][1]*e - eps*e, c - vector[idx_m][2]*d - eps*d)
+        return fn
     
     def target_function(variables):
-        fuzzy_set       = [(variables[i], variables[i + 1], variables[i + 2]) for i in range(0, len(variables), 3)]
-        skip            = 1
-        pairs_1         = [(i, i + skip) for i in range(len(fuzzy_set) - skip)]
-        comparative_imp = []
-        for i, j in pairs_1:
-            a, b, c = criteria_priority[j]
-            d, e, f = criteria_priority[i]
-            comparative_imp.append((a/f, b/e, c/d))
-        pairs_2         = [(i, i + skip) for i in range(len(comparative_imp) - skip)]
-        for i, j in pairs_2:
-            a, b, c = comparative_imp[i]
-            d, e, f = comparative_imp[j]
-            comparative_imp.append((a*d, b*e, c*f))
-        chi             = []
-        skip            = 2
-        pairs_3         = [(i, i + skip) for i in range(len(fuzzy_set) - skip)]
-        pairs           = pairs_1 + pairs_3
-        count           = 0
-        for i, j in pairs:
-            a, b, c = fuzzy_set[i]
-            d, e, f = fuzzy_set[j]
-            x, y, z = comparative_imp[count]
-            count   = count + 1
-            chi.append( abs((a / f) - x) ) 
-            chi.append( abs((b / e) - y) )
-            chi.append( abs((c / d) - z) ) 
-        return np.max(chi)
-    
+        eps     = variables[-1] 
+        cn1     = []
+        wv      = [(1, 1, 1) for item in mic]
+        penalty = 0
+        j       = 0
+        for i in range(0, len(wv)):
+            wv[i] = (variables[j], variables[j+1], variables[j+2])
+            j     = j + 3
+        for i in range(0, len(pairs_w)):
+            a, b, c = operation(wv = wv, eps = eps, vector = mic, idx_a = pairs_w[i][0], idx_b = pairs_w[i][1], idx_m = i)
+            cn1.append( a)
+            cn1.append( b)
+            cn1.append( c)
+            cn1.append(-a)
+            cn1.append(-b)
+            cn1.append(-c)
+        for i in range(0, len(pairs_b)):
+            a, b, c = operation(wv = wv, eps = eps, vector = lic, idx_a = pairs_b[i][0], idx_b = pairs_b[i][1], idx_m = i)
+            cn1.append( a)
+            cn1.append( b)
+            cn1.append( c)
+            cn1.append(-a)
+            cn1.append(-b)
+            cn1.append(-c)
+        for item in cn1:
+            if (item > eps):
+                penalty = penalty + (item - eps) * 1
+        penalty = penalty + eps * eps_penalty
+        return penalty
+    
+    def LMU_constraint(variables):
+        constraints = []
+        for i in range(0, len(variables) - 1, 3):
+            L, m, u = variables[i], variables[i+1], variables[i+2]
+            constraints.append(L)  
+            constraints.append(m - L)  
+            constraints.append(u - m)
+        return constraints
+
     def weights_constraint(variables):
-        fuzzy_set = [(variables[i], variables[i + 1], variables[i + 2]) for i in range(0, len(variables), 3)]
+        fuzzy_set = [(variables[i], variables[i + 1], variables[i + 2]) for i in range(0, len(variables)-1, 3)]
         w         = [(a + 4 * b + c) / 6 for a, b, c in fuzzy_set]
         return np.sum(w)
-
+   
+    constraint_1 = NonlinearConstraint(weights_constraint, 1, 1)
+    constraint_2 = {'type': 'ineq', 'fun': LMU_constraint}
+    constraints  = [constraint_1, constraint_2]
+    
     ################################################
-
-    lower_bounds  = []
-    upper_bounds  = []
-    for i in range(0, len(criteria_priority) * 3, 3):
-        lower_bounds = lower_bounds + [0.0001, 0.0001, 0.0001]
-        upper_bounds = upper_bounds + [1, 1, 1]
-    bounds        = Bounds(lower_bounds, upper_bounds)
-    constraints_1 = NonlinearConstraint(weights_constraint, 1, 1)
-    const_matrix  = []
-    constraint_lb = []
-    constraint_ub = []
-    for i in range(0, len(criteria_priority) * 3, 3):
-        row        = np.zeros(len(criteria_priority) * 3)
-        row[i]     = -1
-        row[i + 1] =  1
-        const_matrix.append(row)
-        constraint_lb.append(0)
-        constraint_ub.append(np.inf)
-        row        = np.zeros(len(criteria_priority)*3)
-        row[i + 1] = -1
-        row[i + 2] =  1
-        const_matrix.append(row)
-        constraint_lb.append(0)
-        constraint_ub.append(np.inf)
-    constraints_2 = LinearConstraint(const_matrix, constraint_lb, constraint_ub)
-    chi           = np.inf
-    solution      = None
+    
+    np.random.seed(42)
+    bounds   = Bounds([0]*len(mic)*3 + [0], [1]*len(mic)*3 + [1])
+    n_starts = 500
+    solution = None
+    obj_fun  = np.inf
     for i in range(0, n_starts):  
         if (i == 0):
-            guess = generate_ordered_triplets(len(criteria_priority))
+            guess = generate_ordered_triplets(len(mic))
+            guess = np.append(guess, [0])
         else:
             guess = solution
-        result = minimize(target_function, guess, method = 'SLSQP', constraints = [constraints_1, constraints_2], bounds = bounds)
-        if (result.fun < chi):
-            chi      = result.fun
-            solution = result.x
-    f_weights     = [(solution[i], solution[i + 1], solution[i + 2]) for i in range(0, len(solution), 3)]
+        
+        results = minimize(target_function, guess, method = 'trust-constr', bounds = bounds, constraints = constraints)
+        if (results.fun < obj_fun):
+            obj_fun  = results.fun
+            solution = results.x
+    f_weights     = [(solution[i], solution[i + 1], solution[i + 2]) for i in range(0, len(solution)-1, 3)]
     weights       = [(a + 4 * b + c) / 6 for a, b, c in f_weights]
-    if (sort_criteria == True):
-        idx       = sorted(range(0, len(criteria_rank)), key = lambda x: extract_number(criteria_rank[x]))
-        f_weights = [f_weights[i] for i in idx]
-        weights   = [  weights[i] for i in idx]
     if (verbose == True):
-        print('Chi:', np.round(chi, 4))
-    return f_weights, weights
+        print('Epsilon Value:', np.round(results.x[-1], 4)) 
+        print('CR: ', np.round(results.x[-1]/ci_value , 4))
+    return  results.x[-1], results.x[-1]/ci_value, f_weights, weights
 
-###############################################################################
+###############################################################################
```

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_merec.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_moora.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_ocra.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/fuzzy_waspas.py` & `pyDecision-4.5.7/pyDecision/algorithm/fuzzy_waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/gra.py` & `pyDecision-4.5.7/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/idocriw.py` & `pyDecision-4.5.7/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/mabac.py` & `pyDecision-4.5.7/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/macbeth.py` & `pyDecision-4.5.7/pyDecision/algorithm/macbeth.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/mairca.py` & `pyDecision-4.5.7/pyDecision/algorithm/mairca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/mara.py` & `pyDecision-4.5.7/pyDecision/algorithm/mara.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/marcos.py` & `pyDecision-4.5.7/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/maut.py` & `pyDecision-4.5.7/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/merec.py` & `pyDecision-4.5.7/pyDecision/algorithm/merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/moora.py` & `pyDecision-4.5.7/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/moosra.py` & `pyDecision-4.5.7/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/multimoora.py` & `pyDecision-4.5.7/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/ocra.py` & `pyDecision-4.5.7/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/opa.py` & `pyDecision-4.5.7/pyDecision/algorithm/opa.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/oreste.py` & `pyDecision-4.5.7/pyDecision/algorithm/oreste.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/p_ec.py` & `pyDecision-4.5.7/pyDecision/algorithm/p_ec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/p_i.py` & `pyDecision-4.5.7/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/p_ii.py` & `pyDecision-4.5.7/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/p_iii.py` & `pyDecision-4.5.7/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/p_iv.py` & `pyDecision-4.5.7/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/p_v.py` & `pyDecision-4.5.7/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/p_vi.py` & `pyDecision-4.5.7/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/p_xgaia.py` & `pyDecision-4.5.7/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/piv.py` & `pyDecision-4.5.7/pyDecision/algorithm/piv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/psi.py` & `pyDecision-4.5.7/pyDecision/algorithm/psi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/psi_m.py` & `pyDecision-4.5.7/pyDecision/algorithm/psi_m.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/rafsi.py` & `pyDecision-4.5.7/pyDecision/algorithm/rafsi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/regime.py` & `pyDecision-4.5.7/pyDecision/algorithm/regime.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/roc.py` & `pyDecision-4.5.7/pyDecision/algorithm/roc.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/rov.py` & `pyDecision-4.5.7/pyDecision/algorithm/rov.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/rrw.py` & `pyDecision-4.5.7/pyDecision/algorithm/rrw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/rsw.py` & `pyDecision-4.5.7/pyDecision/algorithm/rsw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/saw.py` & `pyDecision-4.5.7/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/seca.py` & `pyDecision-4.5.7/pyDecision/algorithm/seca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/smart.py` & `pyDecision-4.5.7/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/spotis.py` & `pyDecision-4.5.7/pyDecision/algorithm/spotis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/todim.py` & `pyDecision-4.5.7/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/topsis.py` & `pyDecision-4.5.7/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/vikor.py` & `pyDecision-4.5.7/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/waspas.py` & `pyDecision-4.5.7/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/wings.py` & `pyDecision-4.5.7/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/algorithm/wisp.py` & `pyDecision-4.5.7/pyDecision/algorithm/wisp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/compare/compare.py` & `pyDecision-4.5.7/pyDecision/compare/compare.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/util/LLM.py` & `pyDecision-4.5.7/pyDecision/util/LLM.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision/util/ga.py` & `pyDecision-4.5.7/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/pyDecision.egg-info/PKG-INFO` & `pyDecision-4.5.7/pyDecision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.5.5
+Version: 4.5.7
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyDecision-4.5.5/pyDecision.egg-info/SOURCES.txt` & `pyDecision-4.5.7/pyDecision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyDecision-4.5.5/setup.py` & `pyDecision-4.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='4.5.5',
+    version='4.5.7',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```


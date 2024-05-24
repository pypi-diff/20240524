# Comparing `tmp/juriscraper-2.6.2.tar.gz` & `tmp/juriscraper-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juriscraper-2.6.2.tar", last modified: Mon May 20 22:39:06 2024, max compression
+gzip compressed data, was "juriscraper-2.6.3.tar", last modified: Fri May 24 20:37:23 2024, max compression
```

## Comparing `juriscraper-2.6.2.tar` & `juriscraper-2.6.3.tar`

### file list

```diff
@@ -1,448 +1,447 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.891760 juriscraper-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-20 22:38:57.000000 juriscraper-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 22:38:57.000000 juriscraper-2.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 22:38:57.000000 juriscraper-2.6.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-20 22:39:06.891760 juriscraper-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-05-20 22:38:57.000000 juriscraper-2.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.819759 juriscraper-2.6.2/juriscraper/
--rw-r--r--   0 runner    (1001) docker     (127)    17359 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/AbstractSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/DeferringList.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/OpinionSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/OpinionSiteLinear.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/OpinionSiteLinearWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/OpinionSiteWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/OralArgumentSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/OralArgumentSiteLinear.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/OralArgumentSiteLinearWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/WebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.819759 juriscraper-2.6.2/juriscraper/fdsys/
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/fdsys/FDSysSite.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/fdsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-20 22:38:57.000000 juriscraper-2.6.2/juriscraper/fdsys/scrape_court_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.819759 juriscraper-2.6.2/juriscraper/fdsys/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/fdsys/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/fdsys/utils/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/fdsys/utils/get_xpath_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.823759 juriscraper-2.6.2/juriscraper/lasc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lasc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lasc/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lasc/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.823759 juriscraper-2.6.2/juriscraper/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/cookie_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/diff_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/judge_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/log_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26813 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.823759 juriscraper-2.6.2/juriscraper/opinions/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/opinion_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.823759 juriscraper-2.6.2/juriscraper/opinions/united_states/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.827759 juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/asbca.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/bia.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/bva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/mspb_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/mspb_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/olc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.831759 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca11_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca11_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca2_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca2_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca3_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca3_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca7.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca9_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca9_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/cadc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/cadc_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/cafc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/scotus_relating.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.831759 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_bankruptcy/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_bankruptcy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.831759 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_district/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_district/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_district/dcd.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_district/ed_louisiana.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.835759 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/acca_memorandum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/acca_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/acca_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/afcca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/ag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/armfor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/cavc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/cit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/fisc.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/fiscr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/nmcca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscfc.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscfc_u.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscgcoca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.867760 juriscraper-2.6.2/juriscraper/opinions/united_states/state/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ala.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/alacivapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/alacrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/alaska.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/alaskactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ariz.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/arizctapp_div_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/arizctapp_div_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ark.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/arkctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/cal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calag.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_3rd.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_4th_div1.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_4th_div2.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_4th_div3.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_5th.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_6th.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_app_div.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/calctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/colo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/coloctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/conn.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/connappct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/dc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/delaware.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/delch.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/delctcompl.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/delsuperct.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/fla.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/fladistctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/fladistctapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/fladistctapp_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/fladistctapp_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/fladistctapp_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/fladistctapp_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/fladistctapp_6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/gactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/haw.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/haw_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/hawapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/idaho_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/idaho_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/idahoctapp_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/idahoctapp_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/idahoctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/illappct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ind.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/indctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/indtc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/iowa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/iowactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/kan_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/kan_u.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/kanctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/kanctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ky.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/kyctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/la.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/lactapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/massappct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/massappct_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/masslandct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/mdag.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/mdctspecapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/me.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/mesuperct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/mich.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/michctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/minn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/minnag.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/minnctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/minnctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/miss.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/miss_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/missctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/mo.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/moctapp_eastern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/moctapp_southern.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/moctapp_western.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/mont.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nc.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ncctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/neb.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nebctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nev.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nevapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nj.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/njsuperctappdiv_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/njsuperctappdiv_u.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/njtaxct_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/njtaxct_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nm.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nmctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ny.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyappdiv_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyappdiv_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyappdiv_3rd.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyappdiv_4th.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyappterm_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyappterm_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nycityct.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nycivct.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyclaimsct.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nycountyct.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nycrimct.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nydistct.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyfamct.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyjustct.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nysupct.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nysupct_commercial.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nysurct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/nytrial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohio.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_10.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_11.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_12.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_6.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_7.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_8.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctapp_9.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctcl.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/okla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/oklaag.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/oklacivapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/oklacrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/or.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/orctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/pa.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/pacommwct.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/pasuperct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ri_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/ri_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/sc.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/scctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/sd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/tenn.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/tenncrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/tennctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/tex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texag.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_10.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_11.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_12.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_13.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_14.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_6.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_7.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_8.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texapp_9.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/texcrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/utah.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/utahctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/va.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/vactapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/vactapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/vt.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/vt_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/vtsuperct_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/vtsuperct_environmental.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/vtsuperct_family.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/vtsuperct_probate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/wash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/washctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/washctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/wis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/wva.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/wvactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/state/wyo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.871760 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/as.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/guam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/nmariana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/prapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/prsupreme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/virginislands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/visuper_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states/territories/visuper_u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.871760 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.871760 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/administrative_agency/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/administrative_agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.871760 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.871760 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.875760 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2011.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.879760 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/cal_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/illappct_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/illappct_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/illappct_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/illappct_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/illappct_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/ind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/indctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/indtc.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/me.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/me_2013.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/ny.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_3rd.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_4th.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/sd.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.879760 juriscraper-2.6.2/juriscraper/oral_args/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/oral_argument_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.879760 juriscraper-2.6.2/juriscraper/oral_args/united_states/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.883760 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca11.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca7.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca9.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/cadc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/cafc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/scotus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.883760 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/illappct_1st_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/illappct_2nd_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/illappct_3rd_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/illappct_4th_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/illappct_5th_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/illappct_workers_comp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/oral_args/united_states/state/md.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.887760 juriscraper-2.6.2/juriscraper/pacer/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/acms_attachment_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/acms_docket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/appellate_attachment_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    30499 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/appellate_docket.py
--rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/attachment_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/case_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/case_query_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/claims_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/claims_register.py
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/docket_history_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    63141 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/docket_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/docket_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/download_confirmation_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    35421 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/email.py
--rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/free_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/hidden_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/internet_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/list_of_creditors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/mobile_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/rss_feeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacer/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/pacerdocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.891760 juriscraper-2.6.2/juriscraper/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.891760 juriscraper-2.6.2/juriscraper/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:38:58.000000 juriscraper-2.6.2/juriscraper/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:06.891760 juriscraper-2.6.2/juriscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-20 22:39:06.000000 juriscraper-2.6.2/juriscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22430 2024-05-20 22:39:06.000000 juriscraper-2.6.2/juriscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:39:06.000000 juriscraper-2.6.2/juriscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-20 22:39:06.000000 juriscraper-2.6.2/juriscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 22:39:06.000000 juriscraper-2.6.2/juriscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-20 22:38:58.000000 juriscraper-2.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-20 22:38:58.000000 juriscraper-2.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-20 22:39:06.891760 juriscraper-2.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-20 22:38:58.000000 juriscraper-2.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.833603 juriscraper-2.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-24 20:37:14.000000 juriscraper-2.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-24 20:37:14.000000 juriscraper-2.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-24 20:37:14.000000 juriscraper-2.6.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-24 20:37:23.833603 juriscraper-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-05-24 20:37:14.000000 juriscraper-2.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.761602 juriscraper-2.6.3/juriscraper/
+-rw-r--r--   0 runner    (1001) docker     (127)    17359 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/AbstractSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/DeferringList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/OpinionSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/OpinionSiteLinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/OpinionSiteLinearWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/OpinionSiteWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/OralArgumentSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/OralArgumentSiteLinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/OralArgumentSiteLinearWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/WebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.761602 juriscraper-2.6.3/juriscraper/fdsys/
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/fdsys/FDSysSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:14.000000 juriscraper-2.6.3/juriscraper/fdsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/fdsys/scrape_court_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.765602 juriscraper-2.6.3/juriscraper/fdsys/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/fdsys/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/fdsys/utils/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/fdsys/utils/get_xpath_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.765602 juriscraper-2.6.3/juriscraper/lasc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lasc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lasc/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lasc/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.765602 juriscraper-2.6.3/juriscraper/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/cookie_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/diff_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/judge_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/log_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26813 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.765602 juriscraper-2.6.3/juriscraper/opinions/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/opinion_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.765602 juriscraper-2.6.3/juriscraper/opinions/united_states/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.769602 juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/asbca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/bia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/bva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/mspb_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/mspb_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/olc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.773602 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca11_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca11_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca2_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca2_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca3_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca3_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca9_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca9_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/cadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/cadc_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/cafc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/scotus_relating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.773602 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_bankruptcy/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_bankruptcy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.773602 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_district/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_district/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_district/dcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_district/ed_louisiana.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.777603 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/acca_memorandum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/acca_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/acca_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/afcca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/ag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/armfor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/cavc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/cit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/fisc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/fiscr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/nmcca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscfc_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscgcoca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.809602 juriscraper-2.6.3/juriscraper/opinions/united_states/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ala.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/alacivapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/alacrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/alaska.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/alaskactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ariz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/arizctapp_div_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/arizctapp_div_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/arkctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_4th_div1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_4th_div2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_4th_div3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_5th.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_6th.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_app_div.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/calctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/colo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/coloctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/connappct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/dc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/delaware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/delch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/delctcompl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/delsuperct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/fla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/fladistctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/fladistctapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/fladistctapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/fladistctapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/fladistctapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/fladistctapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/fladistctapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/gactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/haw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/haw_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/hawapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/idaho_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/idaho_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/idahoctapp_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/idahoctapp_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/idahoctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/illappct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/indctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/indtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/iowa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/iowactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/kan_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/kan_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/kanctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/kanctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ky.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/kyctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/la.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/lactapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/massappct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/massappct_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/masslandct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/mdag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/mdctspecapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/mesuperct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/mich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/michctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/minn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/minnag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/minnctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/minnctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/miss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/miss_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/missctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/moctapp_eastern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/moctapp_southern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/moctapp_western.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/mont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ncctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nebctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nevapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/njsuperctappdiv_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/njsuperctappdiv_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/njtaxct_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/njtaxct_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nmctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyappdiv_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyappdiv_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyappdiv_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyappdiv_4th.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyappterm_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyappterm_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nycityct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nycivct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyclaimsct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nycountyct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nycrimct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nydistct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyfamct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyjustct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nysupct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nysupct_commercial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nysurct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/nytrial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctapp_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/okla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/oklaag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/oklacivapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/oklacrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/or.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/orctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/pa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/pacommwct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/pasuperct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ri_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/ri_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/scctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/sd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/tenn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/tenncrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/tennctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/tex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texapp_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/texcrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/utah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/utahctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/va.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/vactapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/vactapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/vt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/vt_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/vtsuperct_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/vtsuperct_environmental.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/vtsuperct_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/vtsuperct_probate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/wash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/washctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/washctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/wis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/wva.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/wvactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/state/wyo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.813603 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/as.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/guam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/nmariana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/prapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/prsupreme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/virginislands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/visuper_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states/territories/visuper_u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.813603 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.813603 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/administrative_agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/administrative_agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.813603 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.813603 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.817602 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2011.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.821602 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/cal_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/illappct_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/illappct_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/illappct_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/illappct_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/illappct_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/ind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/indctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/indtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/me.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/me_2013.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/ny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_4th.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.821602 juriscraper-2.6.3/juriscraper/oral_args/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/oral_argument_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.821602 juriscraper-2.6.3/juriscraper/oral_args/united_states/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.825602 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/cadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/cafc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/scotus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.825602 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/illappct_1st_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/illappct_2nd_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/illappct_3rd_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/illappct_4th_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/illappct_5th_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/illappct_workers_comp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/oral_args/united_states/state/md.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.829602 juriscraper-2.6.3/juriscraper/pacer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/acms_attachment_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/acms_docket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/appellate_attachment_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30499 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/appellate_docket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/attachment_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/case_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/case_query_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/claims_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/claims_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/docket_history_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63141 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/docket_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/docket_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/download_confirmation_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35828 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/free_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/hidden_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16860 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/internet_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/list_of_creditors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/mobile_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/rss_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacer/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/pacerdocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.829602 juriscraper-2.6.3/juriscraper/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.833603 juriscraper-2.6.3/juriscraper/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:15.000000 juriscraper-2.6.3/juriscraper/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:37:23.833603 juriscraper-2.6.3/juriscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-24 20:37:23.000000 juriscraper-2.6.3/juriscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22370 2024-05-24 20:37:23.000000 juriscraper-2.6.3/juriscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:37:23.000000 juriscraper-2.6.3/juriscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-24 20:37:23.000000 juriscraper-2.6.3/juriscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 20:37:23.000000 juriscraper-2.6.3/juriscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-24 20:37:15.000000 juriscraper-2.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-24 20:37:15.000000 juriscraper-2.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 20:37:23.833603 juriscraper-2.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-24 20:37:15.000000 juriscraper-2.6.3/setup.py
```

### Comparing `juriscraper-2.6.2/LICENSE` & `juriscraper-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/PKG-INFO` & `juriscraper-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juriscraper
-Version: 2.6.2
+Version: 2.6.3
 Summary: An API to scrape American court websites for metadata.
 Home-page: https://github.com/freelawproject/juriscraper
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
 License: BSD
```

### Comparing `juriscraper-2.6.2/README.rst` & `juriscraper-2.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/AbstractSite.py` & `juriscraper-2.6.3/juriscraper/AbstractSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/DeferringList.py` & `juriscraper-2.6.3/juriscraper/DeferringList.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/OpinionSite.py` & `juriscraper-2.6.3/juriscraper/OpinionSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/OpinionSiteLinear.py` & `juriscraper-2.6.3/juriscraper/OpinionSiteLinear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/OralArgumentSite.py` & `juriscraper-2.6.3/juriscraper/OralArgumentSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/OralArgumentSiteLinear.py` & `juriscraper-2.6.3/juriscraper/OralArgumentSiteLinear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/WebDriven.py` & `juriscraper-2.6.3/juriscraper/WebDriven.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/fdsys/FDSysSite.py` & `juriscraper-2.6.3/juriscraper/fdsys/FDSysSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/fdsys/scrape_court_names.py` & `juriscraper-2.6.3/juriscraper/fdsys/scrape_court_names.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/fdsys/utils/get_metadata.py` & `juriscraper-2.6.3/juriscraper/fdsys/utils/get_metadata.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/fdsys/utils/get_xpath_results.py` & `juriscraper-2.6.3/juriscraper/fdsys/utils/get_xpath_results.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lasc/fetch.py` & `juriscraper-2.6.3/juriscraper/lasc/fetch.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lasc/http.py` & `juriscraper-2.6.3/juriscraper/lasc/http.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/cookie_utils.py` & `juriscraper-2.6.3/juriscraper/lib/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/date_utils.py` & `juriscraper-2.6.3/juriscraper/lib/date_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/diff_tools.py` & `juriscraper-2.6.3/juriscraper/lib/diff_tools.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/exceptions.py` & `juriscraper-2.6.3/juriscraper/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/html_utils.py` & `juriscraper-2.6.3/juriscraper/lib/html_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/importer.py` & `juriscraper-2.6.3/juriscraper/lib/importer.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/judge_parsers.py` & `juriscraper-2.6.3/juriscraper/lib/judge_parsers.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/log_tools.py` & `juriscraper-2.6.3/juriscraper/lib/log_tools.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/network_utils.py` & `juriscraper-2.6.3/juriscraper/lib/network_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/string_utils.py` & `juriscraper-2.6.3/juriscraper/lib/string_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/test_utils.py` & `juriscraper-2.6.3/juriscraper/lib/test_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/lib/utils.py` & `juriscraper-2.6.3/juriscraper/lib/utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/opinion_template.py` & `juriscraper-2.6.3/juriscraper/opinions/opinion_template.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/asbca.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/asbca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/bia.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/bia.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/bva.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/bva.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/mspb_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/mspb_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/mspb_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/mspb_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/administrative_agency/olc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/administrative_agency/olc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca1.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca10.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca11_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca11_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca11_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca11_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca2_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca2_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca2_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca2_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca3_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca3_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca4.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca4.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca5.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca6.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca6.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca7.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca7.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca8.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca8.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca9_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca9_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/ca9_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/ca9_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/cadc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/cadc_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/cadc_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/cafc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/cafc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_district/dcd.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_district/dcd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/acca_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/acca_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/afcca.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/afcca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/ag.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/ag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/armfor.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/armfor.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/cavc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/cavc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/cit.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/cit.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/fisc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/fisc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/nmcca.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/nmcca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/tax.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/tax.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscfc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscfc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscfc_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscfc_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/federal_special/uscgcoca.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/federal_special/uscgcoca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/__init__.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/__init__.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ala.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ala.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/alaska.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/alaska.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ariz.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ariz.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/arizctapp_div_2.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/arizctapp_div_2.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ark.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ark.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/cal.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/cal.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/calag.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/calag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/colo.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/colo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/coloctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/coloctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/conn.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/conn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/connappct.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/connappct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/dc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/dc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/delaware.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/delaware.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/fla.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/fla.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/fladistctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/fladistctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/fladistctapp_5.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/fladistctapp_5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ga.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ga.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/gactapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/gactapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/haw.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/haw.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/haw_beginningofyear.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/haw_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/idaho_civil.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/idaho_civil.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/idahoctapp_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/idahoctapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ill.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/illappct.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/illappct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ind.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ind.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/iowa.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/iowa.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/iowactapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/iowactapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/kan_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/kan_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ky.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ky.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/kyctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/kyctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/la.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/la.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/lactapp_1.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/lactapp_1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/mass.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/mass.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/massappct_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/massappct_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/masslandct.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/masslandct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/md.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/md.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/mdag.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/mdag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/mdctspecapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/mdctspecapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/me.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/me.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/mesuperct.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/mesuperct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/mich.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/mich.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/michctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/michctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/minn.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/minn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/minnag.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/minnag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/minnctapp_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/minnctapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/miss.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/miss.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/miss_beginningofyear.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/miss_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/mo.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/mo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/moctapp_southern.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/moctapp_southern.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/mont.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/mont.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ncctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ncctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nd.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/neb.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/neb.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nev.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nev.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nevapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nevapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nh.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nh.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nj.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nj.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ny.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ny.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyag.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyappdiv_1st.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyappdiv_1st.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nyappterm_1st.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nyappterm_1st.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/nytrial.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/nytrial.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohio.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohio.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/okla.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/okla.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/oklaag.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/oklaag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/oklacivapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/oklacivapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/oklacrimapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/oklacrimapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/orctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/orctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/pa.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/pa.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/pacommwct.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/pacommwct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ri_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ri_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/ri_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/ri_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/sc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/sc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/scctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/scctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/sd.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/territories/nmariana.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,83 @@
-# Author: Michael Lissner
-# History:
-# - 2013-06-11: Birth.
-# - 2013-08-06: Revised by Brian Carver
-# - 2014-08-05: Updated URL by mlr
-# - 2021-12-28: Updated by flooie
-
+"""Scraper for Supreme Court of Northern Mariana Islands
+CourtID: nmi
+Court Short Name: NMI
+Author: William Edward Palin
+History:
+  2023-01-21: Created by William Palin
+"""
 import re
+from datetime import date
 from typing import Any, Dict
 
-from juriscraper.lib.html_utils import get_row_column_text
-from juriscraper.lib.string_utils import titlecase
+from juriscraper.lib.string_utils import normalize_dashes
 from juriscraper.OpinionSiteLinear import OpinionSiteLinear
 
 
 class Site(OpinionSiteLinear):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
+        year = str(date.today().year)[-2:]
+        self.url = f"https://www.cnmilaw.org/spm{year}.php#gsc.tab=0"
         self.status = "Published"
-        self.url = "https://ujs.sd.gov/Supreme_Court/opinions.aspx"
+
+    def _cleanup_judge_names(self, judges: str) -> [str]:
+        """Extract judge panel
+
+        Because of a judge Torres,Jr. - and the various permutations of his
+        Jr with and without commas and spacing we do a bit of cleanup to
+        get his and the other judges corretly.  Additionally the author is
+        sometimes denoted by a *.  This is cleaned up.
+
+        :param judges: Content of the panel as a string
+        :return: Judges as a string list
+        """
+        judges = [
+            j.replace(" Jr.", "Jr.").strip(" *") for j in judges.split(",")
+        ]
+        judges = [j.replace("Jr.", " Jr.") for j in judges]
+        return judges
+
+    def _fetch_author(self, judges: str) -> str:
+        """Parse the author from the judge text
+
+        :param judges: Cell content
+        :return: The author
+        """
+        if "*" not in judges:
+            author = "Per Curiam"
+        else:
+            author = [j for j in judges.split(",") if "*" in j][0].strip("*")
+        return author
 
     def _process_html(self):
-        rows = self.html.xpath(
-            "//div[@id='ContentPlaceHolder1_ChildContent1_UpdatePanel_Opinions']//tbody/tr"
-        )
-        for row in rows:
-            cite = re.findall(r"\d{4} S\.D\. \d+", get_row_column_text(row, 2))
-            if not cite:
-                continue
-
-            # https://ujs.sd.gov/uploads/sc/opinions/2928369ef9a6.pdf
-            # We abstract out the first part of the docket number here
-            # And process the full docket number in the `extract_from_text` method
-            # Called after the file has been downloaded.
-            docket = row.xpath(".//td[2]/a/@href")[0].split("/")[-1][:5]
+        for s in self.html.xpath(".//td/a/@href[contains(., 'pdf')]/../../.."):
+            cells = s.xpath(".//td")
+            judge_text = cells[3].text_content()
             self.cases.append(
                 {
-                    "date": get_row_column_text(row, 1),
-                    "name": titlecase(
-                        get_row_column_text(row, 2).rsplit(",", 1)[0]
-                    ),
-                    "citation": cite[0],
-                    "url": row.xpath(".//td[2]/a/@href")[0],
-                    "docket": docket,
+                    "name": cells[0].text_content(),
+                    "citation": cells[1].text_content(),
+                    "date": cells[2].text_content(),
+                    "judges": self._cleanup_judge_names(judge_text),
+                    "author": self._fetch_author(judge_text),
+                    "url": s.xpath(".//td/a/@href")[0],
+                    "docket": "",
                 }
             )
 
     def extract_from_text(self, scraped_text: str) -> Dict[str, Any]:
-        """Can we extract the date filed from the text?
+        """Pass scraped text into function and return data as a dictionary
 
-        :param scraped_text: The content of the document downloaded
-        :return: Metadata to be added to the case
+        :param scraped_text: Text of scraped content
+        :return: metadata containing the docket number
         """
-
-        # The docket number appears to be the first text on the page.
-        # So I crop the text to avoid any confusion that might occur in the
-        # body of an opinion.
-        docket = re.findall(r"#\d+.*-.-\w{3}", scraped_text)[0][:20]
+        normalized_content = normalize_dashes(scraped_text)
+        match = re.findall(r"Case No\.: (.*)", normalized_content)
+        docket_number = match[0] if match else ""
         metadata = {
             "Docket": {
-                "docket_number": docket,
+                "docket_number": docket_number,
             },
         }
         return metadata
```

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/tenn.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/tenn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/tex.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/tex.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/texag.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/texag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/utah.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/utah.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/utahctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/utahctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/va.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/va.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/vactapp_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/vactapp_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/vactapp_u.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/vactapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/vt.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/vt.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/wash.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/wash.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/washctapp_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/washctapp_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/wis.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/wis.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/wva.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/wva.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/state/wyo.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/wyo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/territories/guam.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/territories/guam.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/territories/prapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/territories/prapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/territories/prsupreme.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/territories/prsupreme.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/territories/virginislands.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/territories/virginislands.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states/territories/visuper_p.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/territories/visuper_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/ill.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/ind.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/ind.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/indctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/indctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/me.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/me.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/me_2013.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/me_2013.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/nd.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/nd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/sd.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states/state/sd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,153 @@
 # Author: Michael Lissner
 # History:
 # - 2013-06-11: Birth.
 # - 2013-08-06: Revised by Brian Carver
 # - 2014-08-05: Updated URL by mlr
-# - 2022-01-01: Updated by flooie
+# - 2021-12-28: Updated by flooie
+# - 2024-04-11: grossir, Merge backscraper and scraper; implement dynamic backscraper
 
-import datetime
 import re
+from datetime import datetime
 from typing import Any, Dict
 
+from juriscraper.AbstractSite import logger
 from juriscraper.lib.html_utils import get_row_column_text
 from juriscraper.lib.string_utils import titlecase
 from juriscraper.OpinionSiteLinear import OpinionSiteLinear
 
 
 class Site(OpinionSiteLinear):
+    start_year = 1996
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
         self.status = "Published"
         self.url = "https://ujs.sd.gov/Supreme_Court/opinions.aspx"
-        self.years = range(2010, datetime.date.today().year)
+        self.is_backscrape = False
+        self.make_backscrape_iterable(kwargs)
 
-    def _set_page_year(
-        self,
-        year: int,
-        view_state: str,
-        event_validation: str,
-    ) -> None:
-        a = self.html.xpath(
-            f".//a[contains(@id,'ContentPlaceHolder1_ChildContent1_Repeater_OpinionsYear_LinkButton1')][contains(text(), '{year}')]"
+    def _process_html(self) -> None:
+        """Parse HTML into case dictionaries
+
+        :return None
+        """
+        rows = self.html.xpath(
+            "//div[@id='ContentPlaceHolder1_ChildContent1_UpdatePanel_Opinions']//tbody/tr"
         )
-        link = a[0].get("href").split("'")[1]
+        for row in rows:
+            title = get_row_column_text(row, 2)
+            cite = re.findall(r"\d{4} S\.D\. \d+", title)
+            if not cite:
+                continue
+
+            # https://ujs.sd.gov/uploads/sc/opinions/2928369ef9a6.pdf
+            # We abstract out the first part of the docket number here
+            # And process the full docket number in the `extract_from_text` method
+            # Called after the file has been downloaded.
+            url = row.xpath(".//td[2]/a/@href")[0]
+            docket = url.split("/")[-1][:5]
+            self.cases.append(
+                {
+                    "date": get_row_column_text(row, 1),
+                    "name": titlecase(title.rsplit(",", 1)[0]),
+                    "citation": cite[0],
+                    "url": url,
+                    "docket": docket,
+                }
+            )
+
+        if self.is_backscrape:
+            page_count = self.html.xpath(
+                "//span[@id='ContentPlaceHolder1_ChildContent1_Label_Page']"
+            )[0].text_content()
+            page_of = re.findall(r"Page (\d+) of (\d+)", page_count)
+
+            if len(set(page_of[0])) == 1:
+                return
+
+            logger.info(
+                "Getting page %s of %s", int(page_of[0][0]) + 1, page_of[0][1]
+            )
+            self.get_next_page()
+            self._process_html()
+
+    def get_next_page(self) -> None:
+        """Gets next page"""
+        view_state = self.html.xpath("//input[@id='__VIEWSTATE']/@value")[0]
+        event_validation = self.html.xpath(
+            "//input[@id='__EVENTVALIDATION']/@value"
+        )[0]
         data = {
+            "ctl00$ctl00$ScriptManager1": "ctl00$ctl00$ContentPlaceHolder1$ChildContent1$UpdatePanel_Opinions|ctl00$ctl00$ContentPlaceHolder1$ChildContent1$LinkButton_Next",
+            "__EVENTTARGET": "ctl00$ctl00$ContentPlaceHolder1$ChildContent1$LinkButton_Next",
             "__VIEWSTATE": view_state,
             "__EVENTVALIDATION": event_validation,
-            "__EVENTTARGET": link,
         }
         self.parameters = data
-        self.method = "POST"
+        self.html = super()._download()
 
-    def _set_page_next(
-        self,
-        view_state: str,
-        event_validation: str,
-    ) -> None:
+    def _download_backwards(self, year: int) -> None:
+        """Get input year's page
+
+        We need to GET the homepage first to load hidden inputs
+        Then, we can POST for the desired year's page
+
+        :param year:
+        :return: None
+        """
+        logger.info("Backscraping for year %s", year)
+        self.is_backscrape = True
+
+        self.method = "GET"
+        self.html = super()._download()
+        view_state = self.html.xpath("//input[@id='__VIEWSTATE']/@value")[0]
+        event_validation = self.html.xpath(
+            "//input[@id='__EVENTVALIDATION']/@value"
+        )[0]
+        a = self.html.xpath(
+            f".//a[contains(@id,'ContentPlaceHolder1_ChildContent1_Repeater_OpinionsYear_LinkButton1')][contains(text(), '{year}')]/@href"
+        )
+        link = a[0].split("'")[1]
         data = {
-            "ctl00$ctl00$ScriptManager1": "ctl00$ctl00$ContentPlaceHolder1$ChildContent1$UpdatePanel_Opinions|ctl00$ctl00$ContentPlaceHolder1$ChildContent1$LinkButton_Next",
-            "__EVENTTARGET": "ctl00$ctl00$ContentPlaceHolder1$ChildContent1$LinkButton_Next",
             "__VIEWSTATE": view_state,
             "__EVENTVALIDATION": event_validation,
+            "__EVENTTARGET": link,
         }
         self.parameters = data
         self.method = "POST"
+        self.html = super()._download()
+        self._process_html()
 
-    def _process_html(self):
-        for year in self.years:
-            view_state = self.html.xpath("//input[@id='__VIEWSTATE']")[0].get(
-                "value"
-            )
-            event_validation = self.html.xpath(
-                "//input[@id='__EVENTVALIDATION']"
-            )[0].get("value")
-
-            self._set_page_year(year, view_state, event_validation)
-            self.html = super()._download()
-            while True:
-                rows = self.html.xpath(
-                    "//div[@id='ContentPlaceHolder1_ChildContent1_UpdatePanel_Opinions']//tbody/tr"
-                )
-                for row in rows:
-                    cite = re.findall(
-                        r"\d{4} S\.D\. \d+", get_row_column_text(row, 2)
-                    )
-                    if not cite:
-                        continue
-
-                    # https://ujs.sd.gov/uploads/sc/opinions/2928369ef9a6.pdf
-                    # We abstract out the first part of the docket number here
-                    # And process the full docket number in the `extract_from_text` method
-                    # Called after the file has been downloaded.
-                    docket = row.xpath(".//td[2]/a/@href")[0].split("/")[-1][
-                        :5
-                    ]
-                    self.cases.append(
-                        {
-                            "date": get_row_column_text(row, 1),
-                            "name": titlecase(
-                                get_row_column_text(row, 2).rsplit(",", 1)[0]
-                            ),
-                            "neutral_citation": cite[0],
-                            "url": row.xpath(".//td[2]/a/@href")[0],
-                            "docket": docket,
-                        }
-                    )
-                page_count = self.html.xpath(
-                    "//span[@id='ContentPlaceHolder1_ChildContent1_Label_Page']"
-                )[0].text_content()
-                page_of = re.findall(r"Page (\d+) of (\d+)", page_count)
-                if len(set(page_of[0])) == 1:
-                    break
-
-                vs = self.html.xpath("//input[@id='__VIEWSTATE']")[0].get(
-                    "value"
-                )
-                ev = self.html.xpath("//input[@id='__EVENTVALIDATION']")[
-                    0
-                ].get("value")
+    def make_backscrape_iterable(self, kwargs: Dict) -> None:
+        """Creates backscrape iterable from kwargs or defaults
 
-                self._set_page_next(view_state=vs, event_validation=ev)
-                self.html = super()._download()
+        :param kwargs: passed when initializing the scraper, may or
+            may not contain backscrape controlling arguments
+        :return None
+        """
+        start = kwargs.get("backscrape_start")
+        end = kwargs.get("backscrape_end")
+
+        start = int(start) if start else self.start_year
+        end = int(end) + 1 if end else datetime.today().year
+
+        self.back_scrape_iterable = range(start, end)
 
     def extract_from_text(self, scraped_text: str) -> Dict[str, Any]:
         """Can we extract the date filed from the text?
 
         :param scraped_text: The content of the document downloaded
         :return: Metadata to be added to the case
         """
+
         # The docket number appears to be the first text on the page.
         # So I crop the text to avoid any confusion that might occur in the
         # body of an opinion.
-        docket = re.findall(r"#\d+.*-.-\w{3}", scraped_text)[0][:20]
+        docket = re.findall(r"#\d+.*-.-\w{3}", scraped_text[:100])[0]
         metadata = {
             "Docket": {
                 "docket_number": docket,
             },
         }
         return metadata
```

### Comparing `juriscraper-2.6.2/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py` & `juriscraper-2.6.3/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/oral_argument_template.py` & `juriscraper-2.6.3/juriscraper/oral_args/oral_argument_template.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca1.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca10.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca11.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca11.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca2.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca2.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca3.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca3.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca4.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca4.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca5.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca6.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca6.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca7.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca7.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca8.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca8.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/ca9.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/ca9.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/cadc.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/cafc.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/cafc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/federal_appellate/scotus.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/federal_appellate/scotus.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/state/ill.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/state/illappct_1st_dist.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/state/illappct_1st_dist.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/oral_args/united_states/state/md.py` & `juriscraper-2.6.3/juriscraper/oral_args/united_states/state/md.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/__init__.py` & `juriscraper-2.6.3/juriscraper/pacer/__init__.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/acms_attachment_page.py` & `juriscraper-2.6.3/juriscraper/pacer/acms_attachment_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/acms_docket.py` & `juriscraper-2.6.3/juriscraper/pacer/acms_docket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/appellate_attachment_page.py` & `juriscraper-2.6.3/juriscraper/pacer/appellate_attachment_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/appellate_docket.py` & `juriscraper-2.6.3/juriscraper/pacer/appellate_docket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/attachment_page.py` & `juriscraper-2.6.3/juriscraper/pacer/attachment_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/case_query.py` & `juriscraper-2.6.3/juriscraper/pacer/case_query.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/case_query_advanced.py` & `juriscraper-2.6.3/juriscraper/pacer/case_query_advanced.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/claims_activity.py` & `juriscraper-2.6.3/juriscraper/pacer/claims_activity.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/claims_register.py` & `juriscraper-2.6.3/juriscraper/pacer/claims_register.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/docket_history_report.py` & `juriscraper-2.6.3/juriscraper/pacer/docket_history_report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/docket_report.py` & `juriscraper-2.6.3/juriscraper/pacer/docket_report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/docket_utils.py` & `juriscraper-2.6.3/juriscraper/pacer/docket_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/download_confirmation_page.py` & `juriscraper-2.6.3/juriscraper/pacer/download_confirmation_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/email.py` & `juriscraper-2.6.3/juriscraper/pacer/email.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,15 +540,15 @@
             # Docket number / case name from one or both of the 2 cases
             # may be used in the subject string
             if self.docket_numbers[1] in subject:
                 docket_number = self.docket_numbers[1]
             if self.case_names[1] in subject:
                 case_name = self.case_names[1]
 
-        if self.court_id in ["cacb", "ctb", "cob", "ianb"]:
+        if self.court_id in ["cacb", "ctb", "cob", "ianb", "nyeb"]:
             # In: 6:22-bk-13643-SY Request for courtesy Notice of Electronic Filing (NEF)
             # Out: Request for courtesy Notice of Electronic Filing (NEF)
             short_description = subject.split(docket_number)[-1]
 
             # Remove docket number traces "-AAA"
             regex = r"^-.*?\s"
             short_description = re.sub(regex, "", short_description)
@@ -571,20 +571,29 @@
             # Remove strings starting with "Ch" followed by a number
             regex = r"\bCh\d+\b"
             short_description = re.sub(regex, "", short_description)
 
             # Remove docket number traces "-AAA"
             regex = r"^-.*?\s"
             short_description = re.sub(regex, "", short_description)
-        elif self.court_id in ["pawb", "ndb", "deb"]:
+        elif self.court_id in ["pawb", "ndb", "deb", "pamb"]:
             # In: Ch-7 22-20823-GLT U LOCK INC Reply
             # Out: Reply
             if case_name in subject:
-                # See deb_2.txt for need of this check
                 short_description = subject.split(case_name)[-1]
+            elif case_name[:18] in subject:
+                # See deb_2.txt, pamb_1 and pamb_3 for examples
+                short_description = subject.split(case_name[:18])[-1]
+            elif (
+                " and " in case_name and case_name.split(" and ")[0] in subject
+            ):
+                # See pamb_2.txt
+                short_description = subject.split(case_name.split(" and ")[0])[
+                    -1
+                ]
         else:
             logger.error(
                 "Short description has no parsing for bankruptcy court '%s'",
                 self.court_id,
                 extra={
                     "fingerprint": [
                         f"{self.court_id}-not-parsing-short-description"
```

### Comparing `juriscraper-2.6.2/juriscraper/pacer/free_documents.py` & `juriscraper-2.6.3/juriscraper/pacer/free_documents.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/hidden_api.py` & `juriscraper-2.6.3/juriscraper/pacer/hidden_api.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/http.py` & `juriscraper-2.6.3/juriscraper/pacer/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,14 +259,37 @@
           </changes>
         </partial-response>
         """
         tree = get_xml_parsed_text(r.content)
         xpath = "//update[@id='j_id1:javax.faces.ViewState:0']/text()"
         return tree.xpath(xpath)[0]
 
+    def _prepare_login_request(self, url, data, headers, *args, **kwargs):
+        """Prepares and sends a POST request for login purposes.
+
+        This internal helper function constructs a POST request to the provided URL
+        using the given headers and data. It sets a timeout of 60 seconds for the
+        request.
+
+        :param url: The URL of the login endpoint.
+        :param data: A dictionary containing login credentials.
+        :param headers: Additional headers to include in the request.
+        :param *args: Additional arguments to be passed to the underlying POST
+               request.
+        :param **kwargs: Additional keyword arguments to be passed to the
+               underlying POST request.
+        :return: requests.Response: The response object from the login request.
+        """
+        return super().post(
+            url,
+            headers=headers,
+            timeout=60,
+            data=data,
+        )
+
     def login(self, url=None):
         """Attempt to log into the PACER site.
         The first step is to get an authentication token using a PACER
         username and password.
         To get the authentication token, it's necessary to send a POST request:
         curl --location --request POST 'https://pacer.login.uscourts.gov/services/cso-auth' \
             --header 'Accept: application/json' \
@@ -292,23 +315,21 @@
             "password": self.password,
             "redactFlag": "1",
         }
         # If optional client code information is included, include in login request
         if self.client_code:
             data["clientCode"] = self.client_code
 
-        login_post_r = super().post(
-            url,
-            headers={
-                "User-Agent": "Juriscraper",
-                "Content-type": "application/json",
-                "Accept": "application/json",
-            },
-            timeout=60,
-            data=json.dumps(data),
+        headers = {
+            "User-Agent": "Juriscraper",
+            "Content-type": "application/json",
+            "Accept": "application/json",
+        }
+        login_post_r = self._prepare_login_request(
+            url, data=json.dumps(data), headers=headers
         )
 
         if login_post_r.status_code != requests.codes.ok:
             message = f"Unable connect to PACER site: '{login_post_r.status_code}: {login_post_r.reason}'"
             logger.warning(message)
             raise PacerLoginException(message)
```

### Comparing `juriscraper-2.6.2/juriscraper/pacer/internet_archive.py` & `juriscraper-2.6.3/juriscraper/pacer/internet_archive.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/list_of_creditors.py` & `juriscraper-2.6.3/juriscraper/pacer/list_of_creditors.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/mobile_query.py` & `juriscraper-2.6.3/juriscraper/pacer/mobile_query.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/reports.py` & `juriscraper-2.6.3/juriscraper/pacer/reports.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/rss_feeds.py` & `juriscraper-2.6.3/juriscraper/pacer/rss_feeds.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacer/utils.py` & `juriscraper-2.6.3/juriscraper/pacer/utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/pacerdocket.py` & `juriscraper-2.6.3/juriscraper/pacerdocket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper/report.py` & `juriscraper-2.6.3/juriscraper/report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.6.2/juriscraper.egg-info/PKG-INFO` & `juriscraper-2.6.3/juriscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juriscraper
-Version: 2.6.2
+Version: 2.6.3
 Summary: An API to scrape American court websites for metadata.
 Home-page: https://github.com/freelawproject/juriscraper
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
 License: BSD
```

### Comparing `juriscraper-2.6.2/juriscraper.egg-info/SOURCES.txt` & `juriscraper-2.6.3/juriscraper.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,14 @@
 juriscraper/opinions/united_states_backscrapers/state/me_2013.py
 juriscraper/opinions/united_states_backscrapers/state/nd.py
 juriscraper/opinions/united_states_backscrapers/state/ny.py
 juriscraper/opinions/united_states_backscrapers/state/nyappdiv_1st.py
 juriscraper/opinions/united_states_backscrapers/state/nyappdiv_2nd.py
 juriscraper/opinions/united_states_backscrapers/state/nyappdiv_3rd.py
 juriscraper/opinions/united_states_backscrapers/state/nyappdiv_4th.py
-juriscraper/opinions/united_states_backscrapers/state/sd.py
 juriscraper/opinions/united_states_backscrapers/state/utahctapp.py
 juriscraper/oral_args/__init__.py
 juriscraper/oral_args/oral_argument_template.py
 juriscraper/oral_args/united_states/__init__.py
 juriscraper/oral_args/united_states/federal_appellate/__init__.py
 juriscraper/oral_args/united_states/federal_appellate/ca1.py
 juriscraper/oral_args/united_states/federal_appellate/ca10.py
```

### Comparing `juriscraper-2.6.2/setup.py` & `juriscraper-2.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 import os
 import unittest
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
-VERSION = "2.6.2"
+VERSION = "2.6.3"
 AUTHOR = "Free Law Project"
 EMAIL = "info@free.law"
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 
 reqs_path = f"{HERE}/requirements.txt"
 with open(reqs_path) as reqs_file:
```


# Comparing `tmp/oelint_adv-5.3.2.tar.gz` & `tmp/oelint_adv-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oelint_adv-5.3.2.tar", last modified: Fri May 17 05:39:43 2024, max compression
+gzip compressed data, was "oelint_adv-5.4.0.tar", last modified: Fri May 24 15:42:02 2024, max compression
```

## Comparing `oelint_adv-5.3.2.tar` & `oelint_adv-5.4.0.tar`

### file list

```diff
@@ -1,235 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:39:43.808006 oelint_adv-5.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34162 2024-05-17 05:39:43.808006 oelint_adv-5.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33034 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:39:43.776006 oelint_adv-5.3.2/oelint_adv/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/cls_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14944 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:39:43.792006 oelint_adv-5.3.2/oelint_adv/rule_base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_append_protvars.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_bbclass_exportfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_bbclass_underscores.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_include.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_includevsrequire.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_inlinesuppress_na.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_nospaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_patch_inactiveupstreamdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_patch_inappropriatemsg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_patch_signedoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_patch_upstreamstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_reqinc_norelpaths.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_require.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_underscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_func_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_newline_consecutive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_newline_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_nospace_line_begin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_nospace_line_cont.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_nospace_line_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_nospace_line_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_notabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_addnotaskbody.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_anon_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_customorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_doc_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_heredocs.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_multiappends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_no_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_no_mkdir.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_nopython_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_python_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_addpylib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_appendop.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_autorev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_bbvars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_bugtracker_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_depends_append.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_depends_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_depends_ordered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_descriptionsame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_descriptiontooshort.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_doublemodify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_filesextrapaths.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_filesextrapathsop.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_filesoverride.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_homepage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_homepageping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_inconsspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_insaneskip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_license_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_license_spdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_licfileprefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_misspell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_multilineindent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_notneededspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_override_append.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_p_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_pkgfunc_dusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_pkgspecific.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_pn_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_pn_usage_discouraged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_python_pn_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_quoted.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_rootfscmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_section_lowercase.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_spaces_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_append.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_gittag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_srcrevtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_wildcard.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_summary_80chars.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_summary_linebreaks.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_trailslash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_bbclassextends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_downloadfilename.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_filessetting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_improperinherit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_inherit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_inherit_devtool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_listappend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_mandatory_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_multiinclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_multiinherit.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_native_filename.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_nativesdk_filename.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_pathhardcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_suggested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_variable_override.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_virtual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:39:43.792006 oelint_adv-5.3.2/oelint_adv/rule_jetm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_jetm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/rule_jetm/rule_var_depends_singleline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/oelint_adv/tweaks.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 05:39:42.000000 oelint_adv-5.3.2/oelint_adv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:39:43.808006 oelint_adv-5.3.2/oelint_adv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34162 2024-05-17 05:39:43.000000 oelint_adv-5.3.2/oelint_adv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-05-17 05:39:43.000000 oelint_adv-5.3.2/oelint_adv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:39:43.000000 oelint_adv-5.3.2/oelint_adv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 05:39:43.000000 oelint_adv-5.3.2/oelint_adv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 05:39:43.000000 oelint_adv-5.3.2/oelint_adv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 05:39:43.000000 oelint_adv-5.3.2/oelint_adv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-17 05:39:43.808006 oelint_adv-5.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:39:43.808006 oelint_adv-5.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_append_protvars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_bbclass_underscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_exportfunctions_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_inappmsg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_includenotfound.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_nospaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_patchsignedoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_reqinc_relpaths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_requireinclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_requirenotfound.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_underscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_upstreamstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_file_upstreamstatus_inactiveupstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_func_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_inlinesupp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_jetm_vars_dependssingleline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_newline_consecutive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_newline_eof.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_spaces_emptyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_spaces_linebeginning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_spaces_linecont.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_spaces_lineend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_addnotaskbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_anonpython.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_customorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_heredocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_multifragments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_nocp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_nomkdir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_nopythonprefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_pythonprefix.py
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_task_taskorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_addpylib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_bbclassextend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_downloadfilename.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_filesoverride.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_improperinherit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_inherit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_inherit_devtool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_licenseremote.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_licensespdx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_mandatory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_multiinclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_multiinherit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_nativefilename.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_nativesdkfilename.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_override.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_rootfscmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_var_suggested.py
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_appendop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_autorev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_bbvars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_bugtrackerurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_dependsappend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_dependsclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_dependsordered.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_descriptionsame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_descriptiontoobrief.py
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_doublemodify.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_dusagepkgfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_fileextrapaths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_fileextrapathsop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_filessetting_double.py
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_filessetting_hidden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_homepageping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_homepageprefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_inconspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_insaneskip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_licensefileprefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_listappend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_misspell.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_multilineident.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_notneededspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_notrailingslash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_overrideappend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_pathhardcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_pbpusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_pkgspecific.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_pnbpnusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_pnusagedis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_pythonpnusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_sectionlowercase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_spaceassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_srcuriappend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurichecksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_srcuridomains.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurifile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurigittag.py
--rw-r--r--   0 runner    (1001) docker     (127)    32344 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurioptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurireqopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurisrcrevtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_srcuriswildcard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_summary80chars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_summarylinebreaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_valuequoted.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_class_oelint_vars_virtual.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_configfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_custom_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_inlinesuppressions.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_libmode.py
--rw-r--r--   0 runner    (1001) docker     (127)    42901 2024-05-17 05:39:26.000000 oelint_adv-5.3.2/tests/test_user_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:42:02.948648 oelint_adv-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-05-24 15:42:02.948648 oelint_adv-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33222 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:42:02.916648 oelint_adv-5.4.0/oelint_adv/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/cls_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14944 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:42:02.932648 oelint_adv-5.4.0/oelint_adv/rule_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_append_protvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_bbclass_exportfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_bbclass_underscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_includevsrequire.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_inlinesuppress_na.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_nospaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_patch_inactiveupstreamdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_patch_inappropriatemsg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_patch_signedoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_patch_upstreamstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_reqinc_norelpaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_require.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_underscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_func_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_newline_consecutive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_newline_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_nospace_line_begin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_nospace_line_cont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_nospace_line_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_nospace_line_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_notabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_addnotaskbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_anon_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_customorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_doc_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_heredocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_multiappends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_no_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_no_mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_nopython_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_python_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_addpylib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_appendop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_autorev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_bbvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_bugtracker_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_depends_append.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_depends_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_depends_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_descriptionsame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_descriptiontooshort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_doublemodify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_filesextrapaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_filesextrapathsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_filesoverride.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_homepage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_homepageping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_inconsspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_insaneskip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_license_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_license_spdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_licfileprefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_misspell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_multilineindent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_notneededspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_override_append.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_p_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_pkgfunc_dusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_pkgspecific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_pn_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_pn_usage_discouraged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_python_pn_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_quoted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_rootfscmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_section_lowercase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_spaces_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_append.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_gittag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_srcrevtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_summary_80chars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_summary_linebreaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_trailslash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_bbclassextends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_downloadfilename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_filessetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_improperinherit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_inherit_devtool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_listappend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_mandatory_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_multiinclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_multiinherit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_native_filename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_nativesdk_filename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_pathhardcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_suggested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_unpackdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_variable_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_virtual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:42:02.932648 oelint_adv-5.4.0/oelint_adv/rule_jetm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_jetm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/rule_jetm/rule_var_depends_singleline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/oelint_adv/tweaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 15:42:01.000000 oelint_adv-5.4.0/oelint_adv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:42:02.948648 oelint_adv-5.4.0/oelint_adv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-05-24 15:42:02.000000 oelint_adv-5.4.0/oelint_adv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-05-24 15:42:02.000000 oelint_adv-5.4.0/oelint_adv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:42:02.000000 oelint_adv-5.4.0/oelint_adv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-24 15:42:02.000000 oelint_adv-5.4.0/oelint_adv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-24 15:42:02.000000 oelint_adv-5.4.0/oelint_adv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:42:02.000000 oelint_adv-5.4.0/oelint_adv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-24 15:42:02.948648 oelint_adv-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:42:02.948648 oelint_adv-5.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_append_protvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_bbclass_underscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_exportfunctions_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_inappmsg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_includenotfound.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_nospaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_patchsignedoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_reqinc_relpaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_requireinclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_requirenotfound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_underscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_upstreamstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_file_upstreamstatus_inactiveupstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_func_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_inlinesupp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_jetm_vars_dependssingleline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_newline_consecutive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_newline_eof.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_spaces_emptyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_spaces_linebeginning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_spaces_linecont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_spaces_lineend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_addnotaskbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_anonpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_customorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_heredocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_multifragments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_nocp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_nomkdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_nopythonprefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_pythonprefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_task_taskorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_addpylib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_bbclassextend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_downloadfilename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_filesoverride.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_improperinherit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_inherit_devtool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_licenseremote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_licensespdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_mandatory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_multiinclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_multiinherit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_nativefilename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_nativesdkfilename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_rootfscmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_var_suggested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_appendop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_autorev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_bbvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_bugtrackerurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_dependsappend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_dependsclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_dependsordered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_descriptionsame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_descriptiontoobrief.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_doublemodify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_dusagepkgfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_fileextrapaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_fileextrapathsop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_filessetting_double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_filessetting_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_homepageping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_homepageprefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_inconspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_insaneskip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_licensefileprefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_listappend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_misspell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_multilineident.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_notneededspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_notrailingslash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_overrideappend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_pathhardcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_pbpusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_pkgspecific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_pnbpnusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_pnusagedis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_pythonpnusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_sectionlowercase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_spaceassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_srcuriappend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurichecksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_srcuridomains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurifile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurigittag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32344 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurioptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurireqopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurisrcrevtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_srcuriswildcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_summary80chars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_summarylinebreaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_unpackdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_valuequoted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_class_oelint_vars_virtual.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_configfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_custom_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_inlinesuppressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_libmode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42901 2024-05-24 15:41:44.000000 oelint_adv-5.4.0/tests/test_user_interface.py
```

### Comparing `oelint_adv-5.3.2/LICENSE` & `oelint_adv-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/PKG-INFO` & `oelint_adv-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oelint_adv
-Version: 5.3.2
+Version: 5.4.0
 Summary: Advanced bitbake-recipe linter
 Home-page: https://github.com/priv-kweihmann/oelint-adv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -238,14 +238,15 @@
 * [oelint.vars.srcuridomains](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcuridomains.md) - Recipe is pulling from different domains, this will likely cause issues
 * [oelint.vars.srcurifile](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurifile.md) - First item of SRC_URI should not be a file:// fetcher, if multiple fetcher are used
 * [oelint.vars.srcurigittag](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurigittag.md) - 'tag' in SRC_URI-options leads to not-reproducible builds
 * [oelint.vars.srcurioptions](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurioptions.md) - Unsupported fetcher or invalid options detected
 * [oelint.vars.srcurisrcrevtag](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurisrcrevtag.md) - 'tag' in SRC_URI and a SRCREV for the same component doesn't compute
 * [oelint.vars.summary80chars](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.summary80chars.md) - SUMMARY should max. be 80 characters long
 * [oelint.vars.summarylinebreaks](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.summarylinebreaks.md) - No line breaks in SUMMARY
+* [oelint.vars.unpackdir](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.unpackdir.md) - \$\{UNPACKDIR\} should be used instead of \$\{WORKDIR\} in S and B
 * [oelint.vars.valuequoted](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.valuequoted.md) - Variable values should be properly quoted
 * [oelint.vars.virtual](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.virtual.md) - no virtual/ items in RDEPENDS/RPROVIDES
 
 ### Non-default rulesets
 
 To enable rulesets that are not part of the standard ruleset pass
 **--addrules \<ruleset-name\>** to CLI.
```

### Comparing `oelint_adv-5.3.2/README.md` & `oelint_adv-5.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,15 @@
 * [oelint.vars.srcuridomains](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcuridomains.md) - Recipe is pulling from different domains, this will likely cause issues
 * [oelint.vars.srcurifile](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurifile.md) - First item of SRC_URI should not be a file:// fetcher, if multiple fetcher are used
 * [oelint.vars.srcurigittag](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurigittag.md) - 'tag' in SRC_URI-options leads to not-reproducible builds
 * [oelint.vars.srcurioptions](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurioptions.md) - Unsupported fetcher or invalid options detected
 * [oelint.vars.srcurisrcrevtag](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurisrcrevtag.md) - 'tag' in SRC_URI and a SRCREV for the same component doesn't compute
 * [oelint.vars.summary80chars](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.summary80chars.md) - SUMMARY should max. be 80 characters long
 * [oelint.vars.summarylinebreaks](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.summarylinebreaks.md) - No line breaks in SUMMARY
+* [oelint.vars.unpackdir](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.unpackdir.md) - \$\{UNPACKDIR\} should be used instead of \$\{WORKDIR\} in S and B
 * [oelint.vars.valuequoted](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.valuequoted.md) - Variable values should be properly quoted
 * [oelint.vars.virtual](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.virtual.md) - no virtual/ items in RDEPENDS/RPROVIDES
 
 ### Non-default rulesets
 
 To enable rulesets that are not part of the standard ruleset pass
 **--addrules \<ruleset-name\>** to CLI.
```

### Comparing `oelint_adv-5.3.2/oelint_adv/__main__.py` & `oelint_adv-5.4.0/oelint_adv/__main__.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/cls_rule.py` & `oelint_adv-5.4.0/oelint_adv/cls_rule.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/core.py` & `oelint_adv-5.4.0/oelint_adv/core.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_append_protvars.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_append_protvars.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_bbclass_exportfunctions.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_bbclass_exportfunctions.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_bbclass_underscores.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_bbclass_underscores.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_include.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_include.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_includevsrequire.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_includevsrequire.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_inlinesuppress_na.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_inlinesuppress_na.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_nospaces.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_nospaces.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_patch_inactiveupstreamdetails.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_patch_inactiveupstreamdetails.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_patch_inappropriatemsg.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_patch_inappropriatemsg.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_patch_signedoff.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_patch_signedoff.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_patch_upstreamstatus.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_patch_upstreamstatus.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_reqinc_norelpaths.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_reqinc_norelpaths.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_require.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_require.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_file_underscores.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_file_underscores.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_func_spec.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_func_spec.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_newline_consecutive.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_newline_consecutive.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_newline_end.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_newline_end.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_nospace_line_begin.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_nospace_line_begin.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_nospace_line_cont.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_nospace_line_cont.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_nospace_line_empty.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_nospace_line_empty.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_nospace_line_end.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_nospace_line_end.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_notabs.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_notabs.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_addnotaskbody.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_addnotaskbody.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_anon_python.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_anon_python.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_customorder.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_customorder.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_dash.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_dash.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_doc_strings.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_doc_strings.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_heredocs.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_heredocs.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_multiappends.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_multiappends.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_no_cp.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_no_cp.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_no_mkdir.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_no_mkdir.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_nopython_prefix.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_nopython_prefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_order.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_order.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_tasks_python_prefix.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_tasks_python_prefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_addpylib.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_addpylib.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_appendop.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_appendop.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_autorev.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_autorev.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_bbvars.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_bbvars.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_bugtracker_url.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_bugtracker_url.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_depends_append.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_depends_append.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_depends_class.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_depends_class.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_depends_ordered.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_depends_ordered.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_descriptionsame.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_descriptionsame.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_descriptiontooshort.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_descriptiontooshort.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_doublemodify.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_doublemodify.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_duplicates.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_duplicates.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_filesextrapaths.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_filesextrapaths.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_filesextrapathsop.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_filesextrapathsop.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_filesoverride.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_filesoverride.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_homepage.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_homepage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_homepageping.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_homepageping.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_inconsspaces.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_inconsspaces.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_insaneskip.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_insaneskip.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_license_remote.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_license_remote.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_license_spdx.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_license_spdx.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_licfileprefix.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_licfileprefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_misspell.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_misspell.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_multilineindent.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_multilineindent.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_notneededspace.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_notneededspace.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_override_append.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_override_append.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_p_usage.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_p_usage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_pkgfunc_dusage.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_pkgfunc_dusage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_pkgspecific.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_pkgspecific.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_pn_usage.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_pn_usage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_pn_usage_discouraged.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_pn_usage_discouraged.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_python_pn_usage.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_python_pn_usage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_quoted.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_quoted.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_rootfscmd.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_rootfscmd.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_section_lowercase.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_section_lowercase.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_spaces_assignment.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_spaces_assignment.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_spec.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_spec.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_append.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_append.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_checksum.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_checksum.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_domains.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_domains.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_file.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_file.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_gittag.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_gittag.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_srcrevtag.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_srcrevtag.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_src_uri_wildcard.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_src_uri_wildcard.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_summary_80chars.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_summary_80chars.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_summary_linebreaks.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_summary_linebreaks.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_var_trailslash.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_var_trailslash.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_bbclassextends.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_bbclassextends.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_downloadfilename.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_downloadfilename.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_filessetting.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_filessetting.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_improperinherit.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_improperinherit.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_inherit.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_inherit.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_inherit_devtool.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_inherit_devtool.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_listappend.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_listappend.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_mandatory_exists.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_mandatory_exists.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_multiinclude.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_multiinclude.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_multiinherit.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_multiinherit.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_native_filename.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_native_filename.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_nativesdk_filename.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_nativesdk_filename.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_order.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_order.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_pathhardcode.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_pathhardcode.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_suggested.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_suggested.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_variable_override.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_variable_override.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_base/rule_vars_virtual.py` & `oelint_adv-5.4.0/oelint_adv/rule_base/rule_vars_virtual.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/rule_jetm/rule_var_depends_singleline.py` & `oelint_adv-5.4.0/oelint_adv/rule_jetm/rule_var_depends_singleline.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/state.py` & `oelint_adv-5.4.0/oelint_adv/state.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/oelint_adv/tweaks.py` & `oelint_adv-5.4.0/oelint_adv/tweaks.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "hardknott": {},
         "honister": {},
         "kirkstone": {"_stash_args": {"new_style_override_syntax": True}},
         "langdale": {},
         "mickledore": {"constantmods": {"-": {"variables": {"known": ["PACKAGEBUILDPKGD"]}}}},
         "nanbield": {"constantmods": {"-": {"variables": {"suggested": ["AUTHOR"]}}}},
         "scarthgap": {},
-        "styhead": {},
+        "styhead": {"constantmods": {"+": {"variables": {"known": ["UNPACKDIR"]}}}},
         "latest": {},
     }
 
     @staticmethod
     def tweak_args(args: argparse.Namespace) -> argparse.Namespace:
         """Tweak the passed arguments for specific releases
```

### Comparing `oelint_adv-5.3.2/oelint_adv.egg-info/PKG-INFO` & `oelint_adv-5.4.0/oelint_adv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oelint_adv
-Version: 5.3.2
+Version: 5.4.0
 Summary: Advanced bitbake-recipe linter
 Home-page: https://github.com/priv-kweihmann/oelint-adv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -238,14 +238,15 @@
 * [oelint.vars.srcuridomains](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcuridomains.md) - Recipe is pulling from different domains, this will likely cause issues
 * [oelint.vars.srcurifile](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurifile.md) - First item of SRC_URI should not be a file:// fetcher, if multiple fetcher are used
 * [oelint.vars.srcurigittag](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurigittag.md) - 'tag' in SRC_URI-options leads to not-reproducible builds
 * [oelint.vars.srcurioptions](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurioptions.md) - Unsupported fetcher or invalid options detected
 * [oelint.vars.srcurisrcrevtag](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.srcurisrcrevtag.md) - 'tag' in SRC_URI and a SRCREV for the same component doesn't compute
 * [oelint.vars.summary80chars](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.summary80chars.md) - SUMMARY should max. be 80 characters long
 * [oelint.vars.summarylinebreaks](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.summarylinebreaks.md) - No line breaks in SUMMARY
+* [oelint.vars.unpackdir](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.unpackdir.md) - \$\{UNPACKDIR\} should be used instead of \$\{WORKDIR\} in S and B
 * [oelint.vars.valuequoted](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.valuequoted.md) - Variable values should be properly quoted
 * [oelint.vars.virtual](https://github.com/priv-kweihmann/oelint-adv/blob/master/docs/wiki/oelint.vars.virtual.md) - no virtual/ items in RDEPENDS/RPROVIDES
 
 ### Non-default rulesets
 
 To enable rulesets that are not part of the standard ruleset pass
 **--addrules \<ruleset-name\>** to CLI.
```

### Comparing `oelint_adv-5.3.2/oelint_adv.egg-info/SOURCES.txt` & `oelint_adv-5.4.0/oelint_adv.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 oelint_adv/rule_base/rule_vars_multiinclude.py
 oelint_adv/rule_base/rule_vars_multiinherit.py
 oelint_adv/rule_base/rule_vars_native_filename.py
 oelint_adv/rule_base/rule_vars_nativesdk_filename.py
 oelint_adv/rule_base/rule_vars_order.py
 oelint_adv/rule_base/rule_vars_pathhardcode.py
 oelint_adv/rule_base/rule_vars_suggested.py
+oelint_adv/rule_base/rule_vars_unpackdir.py
 oelint_adv/rule_base/rule_vars_variable_override.py
 oelint_adv/rule_base/rule_vars_virtual.py
 oelint_adv/rule_jetm/__init__.py
 oelint_adv/rule_jetm/rule_var_depends_singleline.py
 tests/test_class_oelint_append_protvars.py
 tests/test_class_oelint_bbclass_underscore.py
 tests/test_class_oelint_exportfunctions_dash.py
@@ -214,14 +215,15 @@
 tests/test_class_oelint_vars_srcurigittag.py
 tests/test_class_oelint_vars_srcurioptions.py
 tests/test_class_oelint_vars_srcurireqopt.py
 tests/test_class_oelint_vars_srcurisrcrevtag.py
 tests/test_class_oelint_vars_srcuriswildcard.py
 tests/test_class_oelint_vars_summary80chars.py
 tests/test_class_oelint_vars_summarylinebreaks.py
+tests/test_class_oelint_vars_unpackdir.py
 tests/test_class_oelint_vars_valuequoted.py
 tests/test_class_oelint_vars_virtual.py
 tests/test_color.py
 tests/test_configfile.py
 tests/test_custom_rules.py
 tests/test_inlinesuppressions.py
 tests/test_libmode.py
```

### Comparing `oelint_adv-5.3.2/setup.cfg` & `oelint_adv-5.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/setup.py` & `oelint_adv-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_append_protvars.py` & `oelint_adv-5.4.0/tests/test_class_oelint_append_protvars.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_bbclass_underscore.py` & `oelint_adv-5.4.0/tests/test_class_oelint_bbclass_underscore.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_exportfunctions_dash.py` & `oelint_adv-5.4.0/tests/test_class_oelint_exportfunctions_dash.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_inappmsg.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_inappmsg.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_includenotfound.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_includenotfound.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_nospaces.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_nospaces.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_patchsignedoff.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_patchsignedoff.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_reqinc_relpaths.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_reqinc_relpaths.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_requireinclude.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_requireinclude.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_requirenotfound.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_requirenotfound.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_underscores.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_underscores.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_upstreamstatus.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_upstreamstatus.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_file_upstreamstatus_inactiveupstream.py` & `oelint_adv-5.4.0/tests/test_class_oelint_file_upstreamstatus_inactiveupstream.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_func_specific.py` & `oelint_adv-5.4.0/tests/test_class_oelint_func_specific.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_inlinesupp.py` & `oelint_adv-5.4.0/tests/test_class_oelint_inlinesupp.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_jetm_vars_dependssingleline.py` & `oelint_adv-5.4.0/tests/test_class_oelint_jetm_vars_dependssingleline.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_newline_consecutive.py` & `oelint_adv-5.4.0/tests/test_class_oelint_newline_consecutive.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_newline_eof.py` & `oelint_adv-5.4.0/tests/test_class_oelint_newline_eof.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_spaces_emptyline.py` & `oelint_adv-5.4.0/tests/test_class_oelint_spaces_emptyline.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_spaces_linebeginning.py` & `oelint_adv-5.4.0/tests/test_class_oelint_spaces_linebeginning.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_spaces_linecont.py` & `oelint_adv-5.4.0/tests/test_class_oelint_spaces_linecont.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_spaces_lineend.py` & `oelint_adv-5.4.0/tests/test_class_oelint_spaces_lineend.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_addnotaskbody.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_addnotaskbody.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_anonpython.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_anonpython.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_customorder.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_customorder.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_dash.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_dash.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_docstrings.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_docstrings.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_heredocs.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_heredocs.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_multifragments.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_multifragments.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_nocp.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_nocp.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_nomkdir.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_nomkdir.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_nopythonprefix.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_nopythonprefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_pythonprefix.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_pythonprefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_task_taskorder.py` & `oelint_adv-5.4.0/tests/test_class_oelint_task_taskorder.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_addpylib.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_addpylib.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_bbclassextend.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_bbclassextend.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_downloadfilename.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_downloadfilename.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_filesoverride.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_filesoverride.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_improperinherit.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_improperinherit.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_inherit.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_inherit.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_inherit_devtool.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_inherit_devtool.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_licenseremote.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_licenseremote.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_licensespdx.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_licensespdx.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_mandatory.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_mandatory.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_multiinclude.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_multiinclude.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_multiinherit.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_multiinherit.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_nativefilename.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_nativefilename.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_nativesdkfilename.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_nativesdkfilename.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_order.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_order.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_override.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_override.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_rootfscmd.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_rootfscmd.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_var_suggested.py` & `oelint_adv-5.4.0/tests/test_class_oelint_var_suggested.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_appendop.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_appendop.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_autorev.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_autorev.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_bbvars.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_bbvars.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_bugtrackerurl.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_bugtrackerurl.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_dependsappend.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_dependsappend.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_dependsclass.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_dependsclass.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_dependsordered.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_dependsordered.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_descriptionsame.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_descriptionsame.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_descriptiontoobrief.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_descriptiontoobrief.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_doublemodify.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_doublemodify.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_duplicate.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_duplicate.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_dusagepkgfunc.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_dusagepkgfunc.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_fileextrapaths.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_fileextrapaths.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_fileextrapathsop.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_fileextrapathsop.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_filessetting_double.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_filessetting_double.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_filessetting_hidden.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_filessetting_hidden.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_homepageping.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_homepageping.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_homepageprefix.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_homepageprefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_inconspaces.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_inconspaces.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_insaneskip.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_insaneskip.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_licensefileprefix.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_licensefileprefix.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_listappend.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_listappend.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_misspell.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_misspell.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_multilineident.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_multilineident.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_notneededspace.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_notneededspace.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_notrailingslash.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_notrailingslash.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_overrideappend.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_overrideappend.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_pathhardcode.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_pathhardcode.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_pbpusage.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_pbpusage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_pkgspecific.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_pkgspecific.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_pnbpnusage.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_pnbpnusage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_pnusagedis.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_pnusagedis.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_pythonpnusage.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_pythonpnusage.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_sectionlowercase.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_sectionlowercase.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_spaceassignment.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_spaceassignment.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_specific.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_specific.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_srcuriappend.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_srcuriappend.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurichecksum.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurichecksum.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_srcuridomains.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_srcuridomains.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurifile.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurifile.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurigittag.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurigittag.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurioptions.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurioptions.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurireqopt.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurireqopt.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_srcurisrcrevtag.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_srcurisrcrevtag.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_srcuriswildcard.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_srcuriswildcard.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_summary80chars.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_summary80chars.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_summarylinebreaks.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_summarylinebreaks.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_valuequoted.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_valuequoted.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_class_oelint_vars_virtual.py` & `oelint_adv-5.4.0/tests/test_class_oelint_vars_virtual.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_color.py` & `oelint_adv-5.4.0/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_configfile.py` & `oelint_adv-5.4.0/tests/test_configfile.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_custom_rules.py` & `oelint_adv-5.4.0/tests/test_custom_rules.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_inlinesuppressions.py` & `oelint_adv-5.4.0/tests/test_inlinesuppressions.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_libmode.py` & `oelint_adv-5.4.0/tests/test_libmode.py`

 * *Files identical despite different names*

### Comparing `oelint_adv-5.3.2/tests/test_user_interface.py` & `oelint_adv-5.4.0/tests/test_user_interface.py`

 * *Files identical despite different names*


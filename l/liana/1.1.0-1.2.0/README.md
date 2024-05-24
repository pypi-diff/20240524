# Comparing `tmp/liana-1.1.0.tar.gz` & `tmp/liana-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liana-1.1.0.tar", max compression
+gzip compressed data, was "liana-1.2.0.tar", max compression
```

## Comparing `liana-1.1.0.tar` & `liana-1.2.0.tar`

### file list

```diff
@@ -1,96 +1,99 @@
--rw-r--r--   0        0        0    35149 2022-09-22 13:22:13.706956 liana-1.1.0/LICENSE
--rw-r--r--   0        0        0     2667 2024-03-25 09:18:41.388773 liana-1.1.0/README.md
--rw-r--r--   0        0        0      411 2024-04-12 09:05:15.061801 liana-1.1.0/liana/__init__.py
--rw-r--r--   0        0        0     2108 2024-02-25 13:50:51.564250 liana-1.1.0/liana/_constants.py
--rw-r--r--   0        0        0     9200 2024-04-12 09:05:15.061801 liana-1.1.0/liana/_docs.py
--rw-r--r--   0        0        0      984 2024-04-05 08:51:49.271659 liana-1.1.0/liana/_logging.py
--rw-r--r--   0        0        0     1969 2024-04-12 09:05:15.061801 liana-1.1.0/liana/method/__init__.py
--rw-r--r--   0        0        0       96 2024-01-02 14:41:52.277014 liana-1.1.0/liana/method/_pipe_utils/__init__.py
--rw-r--r--   0        0        0     5158 2023-11-06 12:56:19.933679 liana-1.1.0/liana/method/_pipe_utils/_aggregate.py
--rw-r--r--   0        0        0     1619 2024-04-12 09:05:15.061801 liana-1.1.0/liana/method/_pipe_utils/_common.py
--rw-r--r--   0        0        0     4478 2024-01-02 14:41:49.557050 liana-1.1.0/liana/method/_pipe_utils/_get_mean_perms.py
--rw-r--r--   0        0        0     9190 2024-04-12 09:05:15.061801 liana-1.1.0/liana/method/_pipe_utils/_pre.py
--rw-r--r--   0        0        0       60 2023-11-06 12:56:19.937679 liana-1.1.0/liana/method/fun/__init__.py
--rw-r--r--   0        0        0    10524 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/fun/_causalnet.py
--rw-r--r--   0        0        0     9782 2024-01-04 07:36:04.092801 liana-1.1.0/liana/method/sc/_Method.py
--rw-r--r--   0        0        0      336 2024-02-25 13:50:51.568250 liana-1.1.0/liana/method/sc/__init__.py
--rw-r--r--   0        0        0     1915 2024-01-02 14:41:49.557050 liana-1.1.0/liana/method/sc/_cellchat.py
--rw-r--r--   0        0        0     1897 2024-01-02 14:41:49.557050 liana-1.1.0/liana/method/sc/_cellphonedb.py
--rw-r--r--   0        0        0     1638 2023-11-06 12:56:19.937679 liana-1.1.0/liana/method/sc/_connectome.py
--rw-r--r--   0        0        0     1558 2023-12-05 07:31:15.866959 liana-1.1.0/liana/method/sc/_geometric_mean.py
--rw-r--r--   0        0        0    19466 2024-02-25 13:50:51.568250 liana-1.1.0/liana/method/sc/_liana_pipe.py
--rw-r--r--   0        0        0     1181 2023-11-07 09:15:10.387722 liana-1.1.0/liana/method/sc/_logfc.py
--rw-r--r--   0        0        0     1376 2024-02-25 13:50:51.568250 liana-1.1.0/liana/method/sc/_natmi.py
--rw-r--r--   0        0        0     6864 2024-01-02 14:41:49.557050 liana-1.1.0/liana/method/sc/_rank_aggregate.py
--rw-r--r--   0        0        0     1059 2024-02-25 13:50:51.568250 liana-1.1.0/liana/method/sc/_scseqcomm.py
--rw-r--r--   0        0        0     1499 2023-09-24 13:38:26.386870 liana-1.1.0/liana/method/sc/_singlecellsignalr.py
--rw-r--r--   0        0        0      284 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_bivariate/__init__.py
--rw-r--r--   0        0        0     4698 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_bivariate/_global_functions.py
--rw-r--r--   0        0        0    12256 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_bivariate/_local_functions.py
--rw-r--r--   0        0        0    15729 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_bivariate/_spatial_bivariate.py
--rw-r--r--   0        0        0    15023 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_misty/_Misty.py
--rw-r--r--   0        0        0        0 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_misty/__init__.py
--rw-r--r--   0        0        0    10823 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_misty/_misty_constructs.py
--rw-r--r--   0        0        0     3621 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_misty/_single_view_models.py
--rw-r--r--   0        0        0     1682 2024-04-12 09:05:15.065801 liana-1.1.0/liana/method/sp/_utils.py
--rw-r--r--   0        0        0      267 2024-02-25 13:50:51.568250 liana-1.1.0/liana/multi/__init__.py
--rw-r--r--   0        0        0     4034 2024-04-12 09:05:15.065801 liana-1.1.0/liana/multi/_nmf.py
--rw-r--r--   0        0        0     7140 2024-04-12 09:05:15.065801 liana-1.1.0/liana/multi/df_to_lr.py
--rw-r--r--   0        0        0    14204 2024-04-12 09:05:15.065801 liana-1.1.0/liana/multi/to_mudata.py
--rw-r--r--   0        0        0     4286 2024-02-25 13:50:51.568250 liana-1.1.0/liana/multi/to_tensor_c2c.py
--rw-r--r--   0        0        0      196 2023-11-06 12:56:19.941680 liana-1.1.0/liana/plotting/__init__.py
--rw-r--r--   0        0        0     4026 2024-01-11 12:36:30.484599 liana-1.1.0/liana/plotting/_common.py
--rw-r--r--   0        0        0     1760 2023-11-07 09:15:10.391722 liana-1.1.0/liana/plotting/_connectivity_plot.py
--rw-r--r--   0        0        0     7243 2024-01-02 14:41:49.561050 liana-1.1.0/liana/plotting/_dotplot.py
--rw-r--r--   0        0        0     7170 2024-02-25 13:50:51.572250 liana-1.1.0/liana/plotting/_misty_plots.py
--rw-r--r--   0        0        0     4667 2024-02-25 13:50:51.572250 liana-1.1.0/liana/plotting/_tileplot.py
--rw-r--r--   0        0        0      303 2024-04-09 07:27:00.642648 liana-1.1.0/liana/resource/__init__.py
--rw-r--r--   0        0        0     4760 2024-02-25 13:50:51.572250 liana-1.1.0/liana/resource/_reassemble_complexes.py
--rw-r--r--   0        0        0     5542 2024-02-25 13:50:51.572250 liana-1.1.0/liana/resource/_resource_utils.py
--rw-r--r--   0        0        0     7732 2024-04-09 07:25:45.471128 liana-1.1.0/liana/resource/get_metalinks.py
--rwxr-xr-x   0        0        0  2004583 2024-01-03 12:47:37.202135 liana-1.1.0/liana/resource/omni_resource.csv
--rw-r--r--   0        0        0     2929 2024-02-25 13:50:51.572250 liana-1.1.0/liana/resource/select_resource.py
--rw-r--r--   0        0        0      301 2023-10-31 12:22:28.754376 liana-1.1.0/liana/testing/__init__.py
--rw-r--r--   0        0        0     2783 2024-04-12 09:05:15.081801 liana-1.1.0/liana/testing/_sample_anndata.py
--rw-r--r--   0        0        0      584 2023-11-06 12:56:19.941680 liana-1.1.0/liana/testing/_sample_dea.py
--rw-r--r--   0        0        0     1206 2024-04-12 09:05:15.081801 liana-1.1.0/liana/testing/_sample_lrs.py
--rw-r--r--   0        0        0      926 2023-11-06 12:56:19.941680 liana-1.1.0/liana/testing/_sample_misty.py
--rw-r--r--   0        0        0      380 2024-04-12 09:05:15.081801 liana-1.1.0/liana/testing/_sample_resource.py
--rw-r--r--   0        0        0     1726 2023-11-06 12:56:19.945680 liana-1.1.0/liana/testing/datasets.py
--rw-r--r--   0        0        0        0 2022-10-10 17:40:32.066002 liana-1.1.0/liana/tests/__init__.py
--rwxr-xr-x   0        0        0   188646 2024-02-25 13:50:51.576250 liana-1.1.0/liana/tests/data/aggregate_rank_rest.csv
--rwxr-xr-x   0        0        0   360667 2024-02-25 13:50:51.576250 liana-1.1.0/liana/tests/data/all_defaults.csv
--rwxr-xr-x   0        0        0  1240013 2024-02-25 13:50:51.588250 liana-1.1.0/liana/tests/data/not_defaults.csv
--rwxr-xr-x   0        0        0   627053 2023-10-13 08:35:25.822208 liana-1.1.0/liana/tests/data/synthetic.h5ad
--rw-r--r--   0        0        0 16830464 2024-04-12 09:08:03.093124 liana-1.1.0/liana/tests/metalinksdb.db
--rw-r--r--   0        0        0     9308 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_bivar.py
--rw-r--r--   0        0        0     2344 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_bivariate_funs.py
--rw-r--r--   0        0        0     2008 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_causalnet.py
--rw-r--r--   0        0        0     1550 2023-11-06 12:56:19.945680 liana-1.1.0/liana/tests/test_converters.py
--rw-r--r--   0        0        0     1151 2024-02-25 13:50:51.592250 liana-1.1.0/liana/tests/test_generate_lr.py
--rw-r--r--   0        0        0     2866 2024-01-02 14:41:49.581049 liana-1.1.0/liana/tests/test_get_mean_perms.py
--rw-r--r--   0        0        0     2023 2024-01-02 14:41:49.581049 liana-1.1.0/liana/tests/test_interpolate.py
--rw-r--r--   0        0        0     4637 2024-02-25 13:50:51.592250 liana-1.1.0/liana/tests/test_liana_pipe.py
--rw-r--r--   0        0        0     1312 2024-02-25 13:50:51.592250 liana-1.1.0/liana/tests/test_metalinksdb.py
--rw-r--r--   0        0        0     6851 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_misty.py
--rw-r--r--   0        0        0     1681 2024-01-02 14:41:49.581049 liana-1.1.0/liana/tests/test_misty_plots.py
--rw-r--r--   0        0        0     5973 2023-11-07 09:15:10.391722 liana-1.1.0/liana/tests/test_multi.py
--rw-r--r--   0        0        0     1754 2024-04-12 07:53:29.775783 liana-1.1.0/liana/tests/test_multi_dea.py
--rw-r--r--   0        0        0     1277 2024-02-25 13:50:51.596249 liana-1.1.0/liana/tests/test_multi_nmf.py
--rw-r--r--   0        0        0     2577 2024-01-02 14:41:49.581049 liana-1.1.0/liana/tests/test_plotting.py
--rw-r--r--   0        0        0     2061 2023-10-13 06:13:31.232542 liana-1.1.0/liana/tests/test_pre.py
--rw-r--r--   0        0        0     3202 2024-02-25 13:50:51.596249 liana-1.1.0/liana/tests/test_rank_aggregate.py
--rw-r--r--   0        0        0     8301 2024-02-25 13:50:51.596249 liana-1.1.0/liana/tests/test_sc_methods.py
--rw-r--r--   0        0        0     2359 2024-02-25 13:50:51.596249 liana-1.1.0/liana/tests/test_select_resource.py
--rw-r--r--   0        0        0     4527 2024-04-12 09:05:15.081801 liana-1.1.0/liana/tests/test_spatial_utils.py
--rw-r--r--   0        0        0      417 2024-01-02 14:41:49.581049 liana-1.1.0/liana/utils/__init__.py
--rw-r--r--   0        0        0     3611 2023-11-07 09:15:10.391722 liana-1.1.0/liana/utils/_getters.py
--rw-r--r--   0        0        0     2221 2024-01-02 14:41:49.581049 liana-1.1.0/liana/utils/interpolate_adata.py
--rw-r--r--   0        0        0     2258 2024-01-10 09:10:17.424395 liana-1.1.0/liana/utils/mdata_to_anndata.py
--rw-r--r--   0        0        0     1477 2024-01-10 09:10:12.848404 liana-1.1.0/liana/utils/obsm_to_adata.py
--rw-r--r--   0        0        0     2174 2024-04-12 09:05:15.081801 liana-1.1.0/liana/utils/query_bandwidth.py
--rw-r--r--   0        0        0     5619 2024-02-25 13:50:51.596249 liana-1.1.0/liana/utils/spatial_neighbors.py
--rw-r--r--   0        0        0     1341 2023-11-06 12:56:19.949680 liana-1.1.0/liana/utils/transform.py
--rw-r--r--   0        0        0     2070 2024-04-12 09:05:15.089801 liana-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 liana-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-22 13:22:13.706956 liana-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2667 2024-05-24 17:09:34.456540 liana-1.2.0/README.md
+-rw-r--r--   0        0        0      411 2024-05-24 17:09:34.772541 liana-1.2.0/liana/__init__.py
+-rw-r--r--   0        0        0     2108 2024-02-25 13:50:51.564250 liana-1.2.0/liana/_constants.py
+-rw-r--r--   0        0        0     9200 2024-04-12 09:05:15.061801 liana-1.2.0/liana/_docs.py
+-rw-r--r--   0        0        0      984 2024-04-05 08:51:49.271659 liana-1.2.0/liana/_logging.py
+-rw-r--r--   0        0        0     1969 2024-04-12 09:05:15.061801 liana-1.2.0/liana/method/__init__.py
+-rw-r--r--   0        0        0       96 2024-01-02 14:41:52.277014 liana-1.2.0/liana/method/_pipe_utils/__init__.py
+-rw-r--r--   0        0        0     5225 2024-05-24 17:09:34.772541 liana-1.2.0/liana/method/_pipe_utils/_aggregate.py
+-rw-r--r--   0        0        0     1619 2024-04-12 09:05:15.061801 liana-1.2.0/liana/method/_pipe_utils/_common.py
+-rw-r--r--   0        0        0     4478 2024-01-02 14:41:49.557050 liana-1.2.0/liana/method/_pipe_utils/_get_mean_perms.py
+-rw-r--r--   0        0        0     9190 2024-05-24 17:09:21.500526 liana-1.2.0/liana/method/_pipe_utils/_pre.py
+-rw-r--r--   0        0        0       60 2023-11-06 12:56:19.937679 liana-1.2.0/liana/method/fun/__init__.py
+-rw-r--r--   0        0        0    10524 2024-04-12 09:05:15.065801 liana-1.2.0/liana/method/fun/_causalnet.py
+-rw-r--r--   0        0        0     9782 2024-01-04 07:36:04.092801 liana-1.2.0/liana/method/sc/_Method.py
+-rw-r--r--   0        0        0      336 2024-02-25 13:50:51.568250 liana-1.2.0/liana/method/sc/__init__.py
+-rw-r--r--   0        0        0     1915 2024-01-02 14:41:49.557050 liana-1.2.0/liana/method/sc/_cellchat.py
+-rw-r--r--   0        0        0     1897 2024-01-02 14:41:49.557050 liana-1.2.0/liana/method/sc/_cellphonedb.py
+-rw-r--r--   0        0        0     1638 2023-11-06 12:56:19.937679 liana-1.2.0/liana/method/sc/_connectome.py
+-rw-r--r--   0        0        0     1558 2023-12-05 07:31:15.866959 liana-1.2.0/liana/method/sc/_geometric_mean.py
+-rw-r--r--   0        0        0    19466 2024-05-07 13:43:10.822157 liana-1.2.0/liana/method/sc/_liana_pipe.py
+-rw-r--r--   0        0        0     1181 2023-11-07 09:15:10.387722 liana-1.2.0/liana/method/sc/_logfc.py
+-rw-r--r--   0        0        0     1376 2024-02-25 13:50:51.568250 liana-1.2.0/liana/method/sc/_natmi.py
+-rw-r--r--   0        0        0     6864 2024-01-02 14:41:49.557050 liana-1.2.0/liana/method/sc/_rank_aggregate.py
+-rw-r--r--   0        0        0     1059 2024-02-25 13:50:51.568250 liana-1.2.0/liana/method/sc/_scseqcomm.py
+-rw-r--r--   0        0        0     1499 2023-09-24 13:38:26.386870 liana-1.2.0/liana/method/sc/_singlecellsignalr.py
+-rw-r--r--   0        0        0      284 2024-04-12 09:05:15.065801 liana-1.2.0/liana/method/sp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:05:15.065801 liana-1.2.0/liana/method/sp/_bivariate/__init__.py
+-rw-r--r--   0        0        0     4698 2024-04-12 09:05:15.065801 liana-1.2.0/liana/method/sp/_bivariate/_global_functions.py
+-rw-r--r--   0        0        0    12256 2024-04-12 09:05:15.065801 liana-1.2.0/liana/method/sp/_bivariate/_local_functions.py
+-rw-r--r--   0        0        0    15763 2024-05-24 17:09:34.772541 liana-1.2.0/liana/method/sp/_bivariate/_spatial_bivariate.py
+-rw-r--r--   0        0        0    15022 2024-05-24 17:09:34.772541 liana-1.2.0/liana/method/sp/_misty/_Misty.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:05:15.065801 liana-1.2.0/liana/method/sp/_misty/__init__.py
+-rw-r--r--   0        0        0    10823 2024-04-12 09:05:15.065801 liana-1.2.0/liana/method/sp/_misty/_misty_constructs.py
+-rw-r--r--   0        0        0     3621 2024-04-12 09:05:15.065801 liana-1.2.0/liana/method/sp/_misty/_single_view_models.py
+-rw-r--r--   0        0        0     1682 2024-04-12 09:05:15.065801 liana-1.2.0/liana/method/sp/_utils.py
+-rw-r--r--   0        0        0      267 2024-02-25 13:50:51.568250 liana-1.2.0/liana/multi/__init__.py
+-rw-r--r--   0        0        0     4034 2024-04-12 09:05:15.065801 liana-1.2.0/liana/multi/_nmf.py
+-rw-r--r--   0        0        0     7140 2024-04-12 09:05:15.065801 liana-1.2.0/liana/multi/df_to_lr.py
+-rw-r--r--   0        0        0    14204 2024-04-12 09:05:15.065801 liana-1.2.0/liana/multi/to_mudata.py
+-rw-r--r--   0        0        0     4286 2024-02-25 13:50:51.568250 liana-1.2.0/liana/multi/to_tensor_c2c.py
+-rw-r--r--   0        0        0      196 2023-11-06 12:56:19.941680 liana-1.2.0/liana/plotting/__init__.py
+-rw-r--r--   0        0        0     4026 2024-05-22 12:31:59.012534 liana-1.2.0/liana/plotting/_common.py
+-rw-r--r--   0        0        0     1760 2023-11-07 09:15:10.391722 liana-1.2.0/liana/plotting/_connectivity_plot.py
+-rw-r--r--   0        0        0     7243 2024-01-02 14:41:49.561050 liana-1.2.0/liana/plotting/_dotplot.py
+-rw-r--r--   0        0        0     7170 2024-02-25 13:50:51.572250 liana-1.2.0/liana/plotting/_misty_plots.py
+-rw-r--r--   0        0        0     4660 2024-05-24 17:09:34.772541 liana-1.2.0/liana/plotting/_tileplot.py
+-rw-r--r--   0        0        0      384 2024-05-24 17:09:34.772541 liana-1.2.0/liana/resource/__init__.py
+-rw-r--r--   0        0        0     7097 2024-05-24 17:09:34.772541 liana-1.2.0/liana/resource/_orthology.py
+-rw-r--r--   0        0        0     4760 2024-05-22 11:24:12.594910 liana-1.2.0/liana/resource/_reassemble_complexes.py
+-rw-r--r--   0        0        0     5542 2024-02-25 13:50:51.572250 liana-1.2.0/liana/resource/_resource_utils.py
+-rw-r--r--   0        0        0     7732 2024-05-22 11:33:20.086884 liana-1.2.0/liana/resource/get_metalinks.py
+-rwxr-xr-x   0        0        0  2004583 2024-01-03 12:47:37.202135 liana-1.2.0/liana/resource/omni_resource.csv
+-rw-r--r--   0        0        0     2929 2024-02-25 13:50:51.572250 liana-1.2.0/liana/resource/select_resource.py
+-rw-r--r--   0        0        0      301 2023-10-31 12:22:28.754376 liana-1.2.0/liana/testing/__init__.py
+-rw-r--r--   0        0        0     2783 2024-04-12 09:05:15.081801 liana-1.2.0/liana/testing/_sample_anndata.py
+-rw-r--r--   0        0        0      584 2023-11-06 12:56:19.941680 liana-1.2.0/liana/testing/_sample_dea.py
+-rw-r--r--   0        0        0     1206 2024-04-12 09:05:15.081801 liana-1.2.0/liana/testing/_sample_lrs.py
+-rw-r--r--   0        0        0      926 2023-11-06 12:56:19.941680 liana-1.2.0/liana/testing/_sample_misty.py
+-rw-r--r--   0        0        0      380 2024-04-12 09:05:15.081801 liana-1.2.0/liana/testing/_sample_resource.py
+-rw-r--r--   0        0        0     1726 2023-11-06 12:56:19.945680 liana-1.2.0/liana/testing/datasets.py
+-rw-r--r--   0        0        0        0 2022-10-10 17:40:32.066002 liana-1.2.0/liana/tests/__init__.py
+-rwxr-xr-x   0        0        0   188646 2024-02-25 13:50:51.576250 liana-1.2.0/liana/tests/data/aggregate_rank_rest.csv
+-rwxr-xr-x   0        0        0   360667 2024-02-25 13:50:51.576250 liana-1.2.0/liana/tests/data/all_defaults.csv
+-rwxr-xr-x   0        0        0  1240013 2024-02-25 13:50:51.588250 liana-1.2.0/liana/tests/data/not_defaults.csv
+-rwxr-xr-x   0        0        0   627053 2023-10-13 08:35:25.822208 liana-1.2.0/liana/tests/data/synthetic.h5ad
+-rw-r--r--   0        0        0  3454647 2024-05-22 12:31:02.836667 liana-1.2.0/liana/tests/human_mouse_hcop_fifteen_column.txt.gz
+-rw-r--r--   0        0        0 16830464 2024-04-12 09:08:03.093124 liana-1.2.0/liana/tests/metalinksdb.db
+-rw-r--r--   0        0        0     9308 2024-04-12 09:05:15.081801 liana-1.2.0/liana/tests/test_bivar.py
+-rw-r--r--   0        0        0     2344 2024-04-12 09:05:15.081801 liana-1.2.0/liana/tests/test_bivariate_funs.py
+-rw-r--r--   0        0        0     2008 2024-04-12 09:05:15.081801 liana-1.2.0/liana/tests/test_causalnet.py
+-rw-r--r--   0        0        0     1550 2023-11-06 12:56:19.945680 liana-1.2.0/liana/tests/test_converters.py
+-rw-r--r--   0        0        0     1151 2024-02-25 13:50:51.592250 liana-1.2.0/liana/tests/test_generate_lr.py
+-rw-r--r--   0        0        0     2866 2024-01-02 14:41:49.581049 liana-1.2.0/liana/tests/test_get_mean_perms.py
+-rw-r--r--   0        0        0     2023 2024-01-02 14:41:49.581049 liana-1.2.0/liana/tests/test_interpolate.py
+-rw-r--r--   0        0        0     4637 2024-02-25 13:50:51.592250 liana-1.2.0/liana/tests/test_liana_pipe.py
+-rw-r--r--   0        0        0     1312 2024-02-25 13:50:51.592250 liana-1.2.0/liana/tests/test_metalinksdb.py
+-rw-r--r--   0        0        0     6851 2024-04-12 09:05:15.081801 liana-1.2.0/liana/tests/test_misty.py
+-rw-r--r--   0        0        0     1681 2024-01-02 14:41:49.581049 liana-1.2.0/liana/tests/test_misty_plots.py
+-rw-r--r--   0        0        0     5973 2023-11-07 09:15:10.391722 liana-1.2.0/liana/tests/test_multi.py
+-rw-r--r--   0        0        0     1754 2024-04-12 07:53:29.775783 liana-1.2.0/liana/tests/test_multi_dea.py
+-rw-r--r--   0        0        0     1277 2024-02-25 13:50:51.596249 liana-1.2.0/liana/tests/test_multi_nmf.py
+-rw-r--r--   0        0        0     2183 2024-05-24 17:09:34.772541 liana-1.2.0/liana/tests/test_orthology.py
+-rw-r--r--   0        0        0     2577 2024-01-02 14:41:49.581049 liana-1.2.0/liana/tests/test_plotting.py
+-rw-r--r--   0        0        0     2061 2023-10-13 06:13:31.232542 liana-1.2.0/liana/tests/test_pre.py
+-rw-r--r--   0        0        0     3321 2024-05-24 17:09:34.776541 liana-1.2.0/liana/tests/test_rank_aggregate.py
+-rw-r--r--   0        0        0     8301 2024-02-25 13:50:51.596249 liana-1.2.0/liana/tests/test_sc_methods.py
+-rw-r--r--   0        0        0     2359 2024-02-25 13:50:51.596249 liana-1.2.0/liana/tests/test_select_resource.py
+-rw-r--r--   0        0        0     4527 2024-04-12 09:05:15.081801 liana-1.2.0/liana/tests/test_spatial_utils.py
+-rw-r--r--   0        0        0      417 2024-05-22 11:23:49.478953 liana-1.2.0/liana/utils/__init__.py
+-rw-r--r--   0        0        0     3611 2023-11-07 09:15:10.391722 liana-1.2.0/liana/utils/_getters.py
+-rw-r--r--   0        0        0     2221 2024-01-02 14:41:49.581049 liana-1.2.0/liana/utils/interpolate_adata.py
+-rw-r--r--   0        0        0     2258 2024-01-10 09:10:17.424395 liana-1.2.0/liana/utils/mdata_to_anndata.py
+-rw-r--r--   0        0        0     1477 2024-01-10 09:10:12.848404 liana-1.2.0/liana/utils/obsm_to_adata.py
+-rw-r--r--   0        0        0     2174 2024-04-12 09:05:15.081801 liana-1.2.0/liana/utils/query_bandwidth.py
+-rw-r--r--   0        0        0     5619 2024-02-25 13:50:51.596249 liana-1.2.0/liana/utils/spatial_neighbors.py
+-rw-r--r--   0        0        0     1341 2023-11-06 12:56:19.949680 liana-1.2.0/liana/utils/transform.py
+-rw-r--r--   0        0        0     2070 2024-05-24 17:09:34.776541 liana-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 liana-1.2.0/PKG-INFO
```

### Comparing `liana-1.1.0/LICENSE` & `liana-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/README.md` & `liana-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 <img src="https://raw.githubusercontent.com/saezlab/liana-py/main/docs/source/_static/abstract.png" width="700" align="center">
 
 ## Development & Contributions
 
 We welcome suggestions, ideas, and contributions! Please use do not hesitate to contact us, or use the issues or the [LIANA+ Development project](https://github.com/orgs/saezlab/projects/16) to make suggestions.
 
-## Tutorials
-A set of extensive tutorials can be found in the [LIANA+ documentation](https://liana-py.readthedocs.io/en/latest/).
+## Vignettes
+A set of extensive vignettes can be found in the [LIANA+ documentation](https://liana-py.readthedocs.io/en/latest/).
 
 ## API
 For further information please check LIANA's [API documentation](https://liana-py.readthedocs.io/en/latest/api.html).
 
 
 ## Cite LIANA+:
```

### Comparing `liana-1.1.0/liana/_constants.py` & `liana-1.2.0/liana/_constants.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/_docs.py` & `liana-1.2.0/liana/_docs.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/_logging.py` & `liana-1.2.0/liana/_logging.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/__init__.py` & `liana-1.2.0/liana/method/__init__.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/_pipe_utils/_aggregate.py` & `liana-1.2.0/liana/method/_pipe_utils/_aggregate.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
         a list with results for all methods
     consensus
         ConsensusClass instance used to generate the lr results
     _key_cols
         should represent unique LRs columns by which to join
     aggregate_method
         method by which we aggregate the ranks. Options are ['rra', 'mean'],
-        where 'rra' corresponds to the RRA method, 'mean' is just the mean of the ranks.
+        where 'rra' corresponds to the RRA method;
+        while 'mean' is just the mean of the ranks divided by the number of interactions
     _consensus_opts
         consensus ranks to be obtained
 
     Returns
     -------
     A long pd.DataFrame with ranked LRs
     """
@@ -99,15 +100,15 @@
     # get only the relevant ranks as a mat (joins order the keys)
     scores = list({specs[s][0] for s in specs})
     rmat = lr_res[scores].values
 
     if aggregate_method == 'rra':
         return _robust_rank_aggregate(rmat)
     elif aggregate_method == 'mean':
-        return np.mean(rmat, axis=1)
+        return np.mean(rmat, axis=1) / rmat.shape[0]
 
 
 def _corr_beta_pvals(p, k) -> np.array:
     """
     Correct beta p-values
 
     Parameters
```

### Comparing `liana-1.1.0/liana/method/_pipe_utils/_common.py` & `liana-1.2.0/liana/method/_pipe_utils/_common.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/_pipe_utils/_get_mean_perms.py` & `liana-1.2.0/liana/method/_pipe_utils/_get_mean_perms.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/_pipe_utils/_pre.py` & `liana-1.2.0/liana/method/_pipe_utils/_pre.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/fun/_causalnet.py` & `liana-1.2.0/liana/method/fun/_causalnet.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_Method.py` & `liana-1.2.0/liana/method/sc/_Method.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_cellchat.py` & `liana-1.2.0/liana/method/sc/_cellchat.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_cellphonedb.py` & `liana-1.2.0/liana/method/sc/_cellphonedb.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_connectome.py` & `liana-1.2.0/liana/method/sc/_connectome.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_geometric_mean.py` & `liana-1.2.0/liana/method/sc/_geometric_mean.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_liana_pipe.py` & `liana-1.2.0/liana/method/sc/_liana_pipe.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_logfc.py` & `liana-1.2.0/liana/method/sc/_logfc.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_natmi.py` & `liana-1.2.0/liana/method/sc/_natmi.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_rank_aggregate.py` & `liana-1.2.0/liana/method/sc/_rank_aggregate.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_scseqcomm.py` & `liana-1.2.0/liana/method/sc/_scseqcomm.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sc/_singlecellsignalr.py` & `liana-1.2.0/liana/method/sc/_singlecellsignalr.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sp/_bivariate/_global_functions.py` & `liana-1.2.0/liana/method/sp/_bivariate/_global_functions.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sp/_bivariate/_local_functions.py` & `liana-1.2.0/liana/method/sp/_bivariate/_local_functions.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sp/_bivariate/_spatial_bivariate.py` & `liana-1.2.0/liana/method/sp/_bivariate/_spatial_bivariate.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,19 +117,19 @@
         If `inplace` is `False`, the results are returned.
 
         """
 
         if n_perms is not None:
             if not isinstance(n_perms, int) or n_perms < 0:
                 raise ValueError("n_perms must be None, 0 for analytical or > 0 for permutation")
-        if (n_perms == 0) and ((local_name != "morans") or (global_name=='morans')):
-            raise ValueError("An analytical solution is currently available only for Moran's R")
         if global_name is not None:
             if isinstance(global_name, str):
                 global_name = [global_name]
+        if (n_perms == 0) and ((local_name not in ["morans", None]) or ~np.isin(global_name, ["morans", None]).any()):
+            raise ValueError("An analytical solution is currently available only for Moran's R")
 
             global_funs = GlobalFunction.instances.keys()
             for g_fun in global_funs:
                 if g_fun not in global_funs:
                     raise ValueError(f"Invalid global function: {g_fun}. Must be in {global_funs}")
 
         if local_name is not None:
```

### Comparing `liana-1.1.0/liana/method/sp/_misty/_Misty.py` & `liana-1.2.0/liana/method/sp/_misty/_Misty.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class MistyData(MuData):
     """MistyData Class used to construct multi-view objects"""
     @d.dedent
     def __init__(self,
                  data:(dict | MuData),
                  obs:(pd.DataFrame | None)=None,
-                 spatial_key: str=K.spatial_key,
+                 spatial_key:str=K.spatial_key,
                  enforce_obs:bool=True,
                  **kwargs):
         """
         Construct a MistyData object from a dictionary of views (anndatas).
 
         Parameters
         ----------
```

### Comparing `liana-1.1.0/liana/method/sp/_misty/_misty_constructs.py` & `liana-1.2.0/liana/method/sp/_misty/_misty_constructs.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sp/_misty/_single_view_models.py` & `liana-1.2.0/liana/method/sp/_misty/_single_view_models.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/method/sp/_utils.py` & `liana-1.2.0/liana/method/sp/_utils.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/multi/_nmf.py` & `liana-1.2.0/liana/multi/_nmf.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/multi/df_to_lr.py` & `liana-1.2.0/liana/multi/df_to_lr.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/multi/to_mudata.py` & `liana-1.2.0/liana/multi/to_mudata.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/multi/to_tensor_c2c.py` & `liana-1.2.0/liana/multi/to_tensor_c2c.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/plotting/_common.py` & `liana-1.2.0/liana/plotting/_common.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/plotting/_connectivity_plot.py` & `liana-1.2.0/liana/plotting/_connectivity_plot.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/plotting/_dotplot.py` & `liana-1.2.0/liana/plotting/_dotplot.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/plotting/_misty_plots.py` & `liana-1.2.0/liana/plotting/_misty_plots.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/plotting/_tileplot.py` & `liana-1.2.0/liana/plotting/_tileplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     if label_fun is not None:
         liana_res[label] = liana_res[label].apply(label_fun)
 
     p = (
         p9.ggplot(liana_res, p9.aes(x='cell_type', y='interaction', fill=fill)) +
         p9.geom_tile() +
         p9.geom_text(p9.aes(label=label), size=label_size, color='white') +
-        p9.facet_grid(facets='~ type', scales='free') +
+        p9.facet_grid('~ type', scales='free') +
         p9.theme_bw(base_size=14) +
         p9.theme(
             axis_text_x=p9.element_text(angle=90),
             figure_size=figure_size,
             strip_background=p9.element_rect(colour="black", fill="#fdfff4"),
         ) +
         p9.scale_fill_cmap(cmap) +
```

### Comparing `liana-1.1.0/liana/resource/_reassemble_complexes.py` & `liana-1.2.0/liana/resource/_reassemble_complexes.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/resource/_resource_utils.py` & `liana-1.2.0/liana/resource/_resource_utils.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/resource/get_metalinks.py` & `liana-1.2.0/liana/resource/get_metalinks.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/resource/omni_resource.csv` & `liana-1.2.0/liana/resource/omni_resource.csv`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/resource/select_resource.py` & `liana-1.2.0/liana/resource/select_resource.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/testing/_sample_anndata.py` & `liana-1.2.0/liana/testing/_sample_anndata.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/testing/_sample_dea.py` & `liana-1.2.0/liana/testing/_sample_dea.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/testing/_sample_lrs.py` & `liana-1.2.0/liana/testing/_sample_lrs.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/testing/_sample_misty.py` & `liana-1.2.0/liana/testing/_sample_misty.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/testing/datasets.py` & `liana-1.2.0/liana/testing/datasets.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/data/aggregate_rank_rest.csv` & `liana-1.2.0/liana/tests/data/aggregate_rank_rest.csv`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/data/all_defaults.csv` & `liana-1.2.0/liana/tests/data/all_defaults.csv`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/data/not_defaults.csv` & `liana-1.2.0/liana/tests/data/not_defaults.csv`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/data/synthetic.h5ad` & `liana-1.2.0/liana/tests/data/synthetic.h5ad`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/metalinksdb.db` & `liana-1.2.0/liana/tests/metalinksdb.db`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_bivar.py` & `liana-1.2.0/liana/tests/test_bivar.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_bivariate_funs.py` & `liana-1.2.0/liana/tests/test_bivariate_funs.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_causalnet.py` & `liana-1.2.0/liana/tests/test_causalnet.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_converters.py` & `liana-1.2.0/liana/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_generate_lr.py` & `liana-1.2.0/liana/tests/test_generate_lr.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_get_mean_perms.py` & `liana-1.2.0/liana/tests/test_get_mean_perms.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_interpolate.py` & `liana-1.2.0/liana/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_liana_pipe.py` & `liana-1.2.0/liana/tests/test_liana_pipe.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_metalinksdb.py` & `liana-1.2.0/liana/tests/test_metalinksdb.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_misty.py` & `liana-1.2.0/liana/tests/test_misty.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_misty_plots.py` & `liana-1.2.0/liana/tests/test_misty_plots.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_multi.py` & `liana-1.2.0/liana/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_multi_dea.py` & `liana-1.2.0/liana/tests/test_multi_dea.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_multi_nmf.py` & `liana-1.2.0/liana/tests/test_multi_nmf.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_plotting.py` & `liana-1.2.0/liana/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_pre.py` & `liana-1.2.0/liana/tests/test_pre.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_rank_aggregate.py` & `liana-1.2.0/liana/tests/test_rank_aggregate.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 def test_consensus_meta():
     assert isinstance(rank_aggregate, AggregateClass)
     assert rank_aggregate.magnitude == 'magnitude_rank'
     assert rank_aggregate.specificity == 'specificity_rank'
     assert rank_aggregate.method_name == 'Rank_Aggregate'
 
-
 def test_aggregate_specs():
     specificity_specs = {'CellPhoneDB': ('cellphone_pvals', True),
                          'Connectome': ('scaled_weight', False),
                          'log2FC': ('lr_logfc', False),
                          'NATMI': ('spec_weight', False),
                     }
     TestCase().assertDictEqual(rank_aggregate.specificity_specs, specificity_specs)
@@ -42,15 +41,20 @@
 def test_aggregate_res():
     lr_res = rank_aggregate(adata, groupby='bulk_labels', use_raw=True, n_perms=2, inplace=False)
     lr_exp = read_csv(test_path.joinpath(path.join("data", "aggregate_rank_rest.csv")), index_col=0)
     assert_frame_equal(lr_res, lr_exp, check_dtype=False, check_exact=False, rtol=1e-4)
 
 
 def test_aggregate_all():
-    rank_aggregate(adata, groupby='bulk_labels', use_raw=True, return_all_lrs=True, key_added='all_res')
+    rank_aggregate(adata,
+                   groupby='bulk_labels',
+                   aggregate_method='mean',
+                   use_raw=True,
+                   return_all_lrs=True,
+                   key_added='all_res')
     assert adata.uns['all_res'].shape == (4200, 13)
 
 
 def test_aggregate_by_sample():
 
     rank_aggregate.by_sample(adata, groupby='bulk_labels', use_raw=True, return_all_lrs=True, sample_key='sample', key_added='liana_by_sample')
     lr_by_sample = adata.uns['liana_by_sample']
```

### Comparing `liana-1.1.0/liana/tests/test_sc_methods.py` & `liana-1.2.0/liana/tests/test_sc_methods.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_select_resource.py` & `liana-1.2.0/liana/tests/test_select_resource.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/tests/test_spatial_utils.py` & `liana-1.2.0/liana/tests/test_spatial_utils.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/utils/_getters.py` & `liana-1.2.0/liana/utils/_getters.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/utils/interpolate_adata.py` & `liana-1.2.0/liana/utils/interpolate_adata.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/utils/mdata_to_anndata.py` & `liana-1.2.0/liana/utils/mdata_to_anndata.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/utils/obsm_to_adata.py` & `liana-1.2.0/liana/utils/obsm_to_adata.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/utils/query_bandwidth.py` & `liana-1.2.0/liana/utils/query_bandwidth.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/utils/spatial_neighbors.py` & `liana-1.2.0/liana/utils/spatial_neighbors.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/liana/utils/transform.py` & `liana-1.2.0/liana/utils/transform.py`

 * *Files identical despite different names*

### Comparing `liana-1.1.0/pyproject.toml` & `liana-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liana"
-version = "1.1.0"
+version = "1.2.0"
 description = "LIANA+: a one-stop-shop framework for cell-cell communication"
 authors = ["Daniel Dimitrov <daniel.dimitrov@uni-heidelberg.de>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
```

### Comparing `liana-1.1.0/PKG-INFO` & `liana-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liana
-Version: 1.1.0
+Version: 1.2.0
 Summary: LIANA+: a one-stop-shop framework for cell-cell communication
 Home-page: https://liana-py.readthedocs.io
 License: GPLv3
 Author: Daniel Dimitrov
 Author-email: daniel.dimitrov@uni-heidelberg.de
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -60,16 +60,16 @@
 
 <img src="https://raw.githubusercontent.com/saezlab/liana-py/main/docs/source/_static/abstract.png" width="700" align="center">
 
 ## Development & Contributions
 
 We welcome suggestions, ideas, and contributions! Please use do not hesitate to contact us, or use the issues or the [LIANA+ Development project](https://github.com/orgs/saezlab/projects/16) to make suggestions.
 
-## Tutorials
-A set of extensive tutorials can be found in the [LIANA+ documentation](https://liana-py.readthedocs.io/en/latest/).
+## Vignettes
+A set of extensive vignettes can be found in the [LIANA+ documentation](https://liana-py.readthedocs.io/en/latest/).
 
 ## API
 For further information please check LIANA's [API documentation](https://liana-py.readthedocs.io/en/latest/api.html).
 
 
 ## Cite LIANA+:
```


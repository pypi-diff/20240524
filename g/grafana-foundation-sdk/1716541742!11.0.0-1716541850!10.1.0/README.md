# Comparing `tmp/grafana_foundation_sdk-1716541742!11.0.0.tar.gz` & `tmp/grafana_foundation_sdk-1716541850!10.1.0.tar.gz`

## Comparing `grafana_foundation_sdk-1716541742!11.0.0.tar` & `grafana_foundation_sdk-1716541850!10.1.0.tar`

### file list

```diff
@@ -1,103 +1,109 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/accesspolicy.py
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/alerting.py
--rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/annotationslist.py
--rw-r--r--   0        0        0    27561 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/azuremonitor.py
--rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/barchart.py
--rw-r--r--   0        0        0    22315 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/bargauge.py
--rw-r--r--   0        0        0    50009 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/candlestick.py
--rw-r--r--   0        0        0    20481 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/canvas.py
--rw-r--r--   0        0        0    29243 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/cloudwatch.py
--rw-r--r--   0        0        0    49538 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/common.py
--rw-r--r--   0        0        0    72631 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/dashboard.py
--rw-r--r--   0        0        0    21861 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/dashboardlist.py
--rw-r--r--   0        0        0    18861 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/datagrid.py
--rw-r--r--   0        0        0    19038 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/debug.py
--rw-r--r--   0        0        0    63305 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/elasticsearch.py
--rw-r--r--   0        0        0    49166 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/expr.py
--rw-r--r--   0        0        0    21279 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/gauge.py
--rw-r--r--   0        0        0    20204 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/geomap.py
--rw-r--r--   0        0        0    19800 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/grafanapyroscope.py
--rw-r--r--   0        0        0    30297 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/heatmap.py
--rw-r--r--   0        0        0    34584 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/histogram.py
--rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/librarypanel.py
--rw-r--r--   0        0        0    21476 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/logs.py
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/loki.py
--rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/news.py
--rw-r--r--   0        0        0    19063 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/nodegraph.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/parca.py
--rw-r--r--   0        0        0    21960 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/piechart.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/preferences.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/prometheus.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/publicdashboard.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/role.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/rolebinding.py
--rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/stat.py
--rw-r--r--   0        0        0    24178 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/statetimeline.py
--rw-r--r--   0        0        0    23895 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/statushistory.py
--rw-r--r--   0        0        0    28817 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/table.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/team.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/tempo.py
--rw-r--r--   0        0        0    18787 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/testdata.py
--rw-r--r--   0        0        0    19310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/text.py
--rw-r--r--   0        0        0    48021 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/timeseries.py
--rw-r--r--   0        0        0    47390 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/trend.py
--rw-r--r--   0        0        0    37141 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/xychart.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/cog/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/cog/builder.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/cog/encoder.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/cog/plugins.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/cog/runtime.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/cog/variants.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/__init__.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/accesspolicy.py
--rw-r--r--   0        0        0    26784 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/alerting.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/annotationslist.py
--rw-r--r--   0        0        0    40649 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/azuremonitor.py
--rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/barchart.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/bargauge.py
--rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/candlestick.py
--rw-r--r--   0        0        0    15808 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/canvas.py
--rw-r--r--   0        0        0    39640 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/cloudwatch.py
--rw-r--r--   0        0        0    87730 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/common.py
--rw-r--r--   0        0        0    86957 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/dashboard.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/dashboardlist.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/datagrid.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/debug.py
--rw-r--r--   0        0        0    91710 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/elasticsearch.py
--rw-r--r--   0        0        0    64441 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/expr.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/gauge.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/geomap.py
--rw-r--r--   0        0        0    27529 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/grafanapyroscope.py
--rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/heatmap.py
--rw-r--r--   0        0        0     8475 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/histogram.py
--rw-r--r--   0        0        0    16344 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/librarypanel.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/logs.py
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/loki.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/news.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/nodegraph.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/parca.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/piechart.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/preferences.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/prometheus.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/publicdashboard.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/role.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/rolebinding.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/stat.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/statetimeline.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/statushistory.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/table.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/team.py
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/tempo.py
--rw-r--r--   0        0        0    28219 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/testdata.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/text.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/timeseries.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/trend.py
--rw-r--r--   0        0        0    18310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/xychart.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/LICENSE.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/README.md
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/pyproject.toml
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541742!11.0.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/accesspolicy.py
+-rw-r--r--   0        0        0    18535 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/alertgroups.py
+-rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/alerting.py
+-rw-r--r--   0        0        0    20414 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/annotationslist.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/azuremonitor.py
+-rw-r--r--   0        0        0    37625 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/barchart.py
+-rw-r--r--   0        0        0    20170 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/bargauge.py
+-rw-r--r--   0        0        0    47608 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/candlestick.py
+-rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/canvas.py
+-rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/cloudwatch.py
+-rw-r--r--   0        0        0    48574 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/common.py
+-rw-r--r--   0        0        0    76169 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/dashboard.py
+-rw-r--r--   0        0        0    20296 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/dashboardlist.py
+-rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/datagrid.py
+-rw-r--r--   0        0        0    17906 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/debug.py
+-rw-r--r--   0        0        0    63427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/elasticsearch.py
+-rw-r--r--   0        0        0    49166 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/expr.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/folder.py
+-rw-r--r--   0        0        0    19181 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/gauge.py
+-rw-r--r--   0        0        0    19072 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/geomap.py
+-rw-r--r--   0        0        0    22904 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/grafanapyroscope.py
+-rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/heatmap.py
+-rw-r--r--   0        0        0    31190 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/histogram.py
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/librarypanel.py
+-rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/logs.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/loki.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/news.py
+-rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/nodegraph.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/parca.py
+-rw-r--r--   0        0        0    20828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/piechart.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/playlist.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/preferences.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/prometheus.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/publicdashboard.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/role.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/rolebinding.py
+-rw-r--r--   0        0        0    19784 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/stat.py
+-rw-r--r--   0        0        0    23046 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/statetimeline.py
+-rw-r--r--   0        0        0    22763 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/statushistory.py
+-rw-r--r--   0        0        0    19916 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/table.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/team.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/tempo.py
+-rw-r--r--   0        0        0    12183 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/testdata.py
+-rw-r--r--   0        0        0    18178 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/text.py
+-rw-r--r--   0        0        0    45683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/timeseries.py
+-rw-r--r--   0        0        0    45406 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/trend.py
+-rw-r--r--   0        0        0    35041 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/xychart.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/cog/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/cog/builder.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/cog/encoder.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/cog/plugins.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/cog/runtime.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/cog/variants.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/__init__.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/accesspolicy.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/alertgroups.py
+-rw-r--r--   0        0        0    27377 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/alerting.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/annotationslist.py
+-rw-r--r--   0        0        0    39886 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/azuremonitor.py
+-rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/barchart.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/bargauge.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/candlestick.py
+-rw-r--r--   0        0        0    13569 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/canvas.py
+-rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/cloudwatch.py
+-rw-r--r--   0        0        0    84497 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/common.py
+-rw-r--r--   0        0        0    87863 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/dashboard.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/dashboardlist.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/datagrid.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/debug.py
+-rw-r--r--   0        0        0    91828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/elasticsearch.py
+-rw-r--r--   0        0        0    64441 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/expr.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/folder.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/gauge.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/geomap.py
+-rw-r--r--   0        0        0    32298 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/grafanapyroscope.py
+-rw-r--r--   0        0        0    20031 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/heatmap.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/histogram.py
+-rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/librarypanel.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/logs.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/loki.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/news.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/nodegraph.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/parca.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/piechart.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/playlist.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/preferences.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/prometheus.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/publicdashboard.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/role.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/rolebinding.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/stat.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/statetimeline.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/statushistory.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/table.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/team.py
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/tempo.py
+-rw-r--r--   0        0        0    20919 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/testdata.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/text.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/timeseries.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/trend.py
+-rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/xychart.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/LICENSE.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/README.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1716541850!10.1.0/PKG-INFO
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/accesspolicy.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/alerting.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/alerting.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,30 +53,117 @@
     def template(self, template: str) -> typing.Self:        
         self._internal.template = template
     
         return self
     
 
 class TimeInterval(cogbuilder.Builder[alerting.TimeInterval]):    
+    """
+    TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    within the interval.
+    """
+    
     _internal: alerting.TimeInterval
 
     def __init__(self):
         self._internal = alerting.TimeInterval()
 
     def build(self) -> alerting.TimeInterval:
         return self._internal    
     
-    def name(self, name: str) -> typing.Self:        
-        self._internal.name = name
+    def days_of_month(self, days_of_month: list[str]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.days_of_month = days_of_month
+    
+        return self
+    
+    def location(self, location: str) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.location = location
+    
+        return self
+    
+    def months(self, months: list[str]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.months = months
+    
+        return self
+    
+    def times(self, times: list[cogbuilder.Builder[alerting.TimeRange]]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        times_resources = [r1.build() for r1 in times]
+        self._internal.times = times_resources
+    
+        return self
+    
+    def weekdays(self, weekdays: list[str]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.weekdays = weekdays
+    
+        return self
+    
+    def years(self, years: list[str]) -> typing.Self:    
+        """
+        TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+        within the interval.
+        """
+            
+        self._internal.years = years
+    
+        return self
+    
+
+class TimeRange(cogbuilder.Builder[alerting.TimeRange]):    
+    """
+    Redefining this to avoid an import cycle
+    """
+    
+    _internal: alerting.TimeRange
+
+    def __init__(self):
+        self._internal = alerting.TimeRange()
+
+    def build(self) -> alerting.TimeRange:
+        return self._internal    
+    
+    def from_val(self, from_val: str) -> typing.Self:    
+        """
+        Redefining this to avoid an import cycle
+        """
+            
+        self._internal.from_val = from_val
     
         return self
     
-    def time_intervals(self, time_intervals: list[cogbuilder.Builder[alerting.TimeInterval]]) -> typing.Self:        
-        time_intervals_resources = [r1.build() for r1 in time_intervals]
-        self._internal.time_intervals = time_intervals_resources
+    def to(self, to: str) -> typing.Self:    
+        """
+        Redefining this to avoid an import cycle
+        """
+            
+        self._internal.to = to
     
         return self
     
 
 class RuleGroup(cogbuilder.Builder[alerting.RuleGroup]):    
     _internal: alerting.RuleGroup
 
@@ -198,20 +285,14 @@
         return self
     
     def no_data_state(self, no_data_state: typing.Literal["Alerting", "NoData", "OK"]) -> typing.Self:        
         self._internal.no_data_state = no_data_state
     
         return self
     
-    def notification_settings(self, notification_settings: cogbuilder.Builder[alerting.NotificationSettings]) -> typing.Self:        
-        notification_settings_resource = notification_settings.build()
-        self._internal.notification_settings = notification_settings_resource
-    
-        return self
-    
     def org_id(self, org_id: int) -> typing.Self:        
         self._internal.org_id = org_id
     
         return self
     
     def provenance(self, provenance: alerting.Provenance) -> typing.Self:        
         self._internal.provenance = provenance
@@ -233,68 +314,24 @@
         if not len(title) <= 190:
             raise ValueError("len(title) must be <= 190")
         self._internal.title = title
     
         return self
     
     def uid(self, uid: str) -> typing.Self:        
-        if not len(uid) >= 1:
-            raise ValueError("len(uid) must be >= 1")
-        if not len(uid) <= 40:
-            raise ValueError("len(uid) must be <= 40")
         self._internal.uid = uid
     
         return self
     
     def updated(self, updated: str) -> typing.Self:        
         self._internal.updated = updated
     
         return self
     
 
-class NotificationSettings(cogbuilder.Builder[alerting.NotificationSettings]):    
-    _internal: alerting.NotificationSettings
-
-    def __init__(self):
-        self._internal = alerting.NotificationSettings()
-
-    def build(self) -> alerting.NotificationSettings:
-        return self._internal    
-    
-    def group_by(self, group_by: list[str]) -> typing.Self:        
-        self._internal.group_by = group_by
-    
-        return self
-    
-    def group_interval(self, group_interval: str) -> typing.Self:        
-        self._internal.group_interval = group_interval
-    
-        return self
-    
-    def group_wait(self, group_wait: str) -> typing.Self:        
-        self._internal.group_wait = group_wait
-    
-        return self
-    
-    def mute_time_intervals(self, mute_time_intervals: list[str]) -> typing.Self:        
-        self._internal.mute_time_intervals = mute_time_intervals
-    
-        return self
-    
-    def receiver(self, receiver: str) -> typing.Self:        
-        self._internal.receiver = receiver
-    
-        return self
-    
-    def repeat_interval(self, repeat_interval: str) -> typing.Self:        
-        self._internal.repeat_interval = repeat_interval
-    
-        return self
-    
-
 class Query(cogbuilder.Builder[alerting.Query]):    
     _internal: alerting.Query
 
     def __init__(self, ref_id: typing.Optional[str]):
         self._internal = alerting.Query()        
         self._internal.ref_id = ref_id
 
@@ -394,18 +431,14 @@
     
     def uid(self, uid: str) -> typing.Self:    
         """
         EmbeddedContactPoint is the contact point type that is used
         by grafanas embedded alertmanager implementation.
         """
             
-        if not len(uid) >= 1:
-            raise ValueError("len(uid) must be >= 1")
-        if not len(uid) <= 40:
-            raise ValueError("len(uid) must be <= 40")
         self._internal.uid = uid
     
         return self
     
 
 class NotificationPolicy(cogbuilder.Builder[alerting.NotificationPolicy]):    
     """
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/annotationslist.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/annotationslist.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,24 +153,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -237,50 +227,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/azuremonitor.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/azuremonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -365,35 +367,26 @@
         Array of resource URIs to be queried.
         """
             
         self._internal.resources = resources
     
         return self
     
-    def dashboard_time(self, dashboard_time: bool) -> typing.Self:    
-        """
-        If set to true the dashboard time range will be used as a filter for the query. Otherwise the query time ranges will be used. Defaults to false.
-        """
-            
-        self._internal.dashboard_time = dashboard_time
-    
-        return self
-    
-    def time_column(self, time_column: str) -> typing.Self:    
+    def intersect_time(self, intersect_time: bool) -> typing.Self:    
         """
-        If dashboardTime is set to true this value dictates which column the time filter will be applied to. Defaults to the first tables timeSpan column, the first datetime column found, or TimeGenerated
+        If set to true the intersection of time ranges specified in the query and Grafana will be used. Otherwise the query time ranges will be used. Defaults to false
         """
             
-        self._internal.time_column = time_column
+        self._internal.intersect_time = intersect_time
     
         return self
     
     def workspace(self, workspace: str) -> typing.Self:    
         """
-        Workspace ID. This was removed in Grafana 8, but remains for backwards compat.
+        Workspace ID. This was removed in Grafana 8, but remains for backwards compat
         """
             
         self._internal.workspace = workspace
     
         return self
     
     def resource(self, resource: str) -> typing.Self:    
@@ -401,23 +394,14 @@
         @deprecated Use resources instead
         """
             
         self._internal.resource = resource
     
         return self
     
-    def intersect_time(self, intersect_time: bool) -> typing.Self:    
-        """
-        @deprecated Use dashboardTime instead
-        """
-            
-        self._internal.intersect_time = intersect_time
-    
-        return self
-    
 
 class AzureTracesQuery(cogbuilder.Builder[azuremonitor.AzureTracesQuery]):    
     """
     Application Insights Traces sub-query properties
     """
     
     _internal: azuremonitor.AzureTracesQuery
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/barchart.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/barchart.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -817,28 +780,14 @@
             self._internal.field_config.defaults.custom = barchart.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, barchart.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = barchart.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, barchart.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
-    
-        return self
-    
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -865,21 +814,21 @@
             self._internal.field_config.defaults.custom = barchart.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, barchart.FieldConfig)
         thresholds_style_resource = thresholds_style.build()
         self._internal.field_config.defaults.custom.thresholds_style = thresholds_style_resource
     
         return self
     
-    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = barchart.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, barchart.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/bargauge.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
+from ..models import logs
 from ..models import common
-from ..models import bargauge
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "bargauge"
+        self._internal.type_val = "logs"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -454,97 +417,71 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def display_mode(self, display_mode: common.BarGaugeDisplayMode) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.display_mode = display_mode
-    
-        return self
-    
-    def value_mode(self, value_mode: common.BarGaugeValueMode) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.value_mode = value_mode
-    
-        return self
-    
-    def name_placement(self, name_placement: common.BarGaugeNamePlacement) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.name_placement = name_placement
-    
-        return self
-    
-    def show_unfilled(self, show_unfilled: bool) -> typing.Self:        
+    def show_labels(self, show_labels: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.show_unfilled = show_unfilled
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.show_labels = show_labels
     
         return self
     
-    def sizing(self, sizing: common.BarGaugeSizing) -> typing.Self:        
+    def show_common_labels(self, show_common_labels: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.sizing = sizing
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.show_common_labels = show_common_labels
     
         return self
     
-    def min_viz_width(self, min_viz_width: int) -> typing.Self:        
+    def show_time(self, show_time: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.min_viz_width = min_viz_width
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.show_time = show_time
     
         return self
     
-    def min_viz_height(self, min_viz_height: int) -> typing.Self:        
+    def wrap_log_message(self, wrap_log_message: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.min_viz_height = min_viz_height
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.wrap_log_message = wrap_log_message
     
         return self
     
-    def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
+    def prettify_log_message(self, prettify_log_message: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        reduce_options_resource = reduce_options.build()
-        self._internal.options.reduce_options = reduce_options_resource
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.prettify_log_message = prettify_log_message
     
         return self
     
-    def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
+    def enable_log_details(self, enable_log_details: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        text_resource = text.build()
-        self._internal.options.text = text_resource
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.enable_log_details = enable_log_details
     
         return self
     
-    def max_viz_height(self, max_viz_height: int) -> typing.Self:        
+    def sort_order(self, sort_order: common.LogsSortOrder) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.max_viz_height = max_viz_height
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.sort_order = sort_order
     
         return self
     
-    def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
+    def dedup_strategy(self, dedup_strategy: common.LogsDedupStrategy) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.orientation = orientation
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.dedup_strategy = dedup_strategy
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/candlestick.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/candlestick.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -523,23 +486,14 @@
             self._internal.options = candlestick.Options()
         assert isinstance(self._internal.options, candlestick.Options)
         legend_resource = legend.build()
         self._internal.options.legend = legend_resource
     
         return self
     
-    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = candlestick.Options()
-        assert isinstance(self._internal.options, candlestick.Options)
-        tooltip_resource = tooltip.build()
-        self._internal.options.tooltip = tooltip_resource
-    
-        return self
-    
     def include_all_fields(self, include_all_fields: bool) -> typing.Self:    
         """
         When enabled, all fields will be sent to the graph
         """
             
         if self._internal.options is None:
             self._internal.options = candlestick.Options()
@@ -827,28 +781,14 @@
             self._internal.field_config.defaults.custom = candlestick.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, candlestick.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = candlestick.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, candlestick.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
-    
-        return self
-    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -961,25 +901,25 @@
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = candlestick.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, candlestick.FieldConfig)
         self._internal.field_config.defaults.custom.point_symbol = point_symbol
     
         return self
     
-    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = candlestick.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, candlestick.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/canvas.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import canvas
+from ..models import table
+from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "canvas"
+        self._internal.type_val = "table"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -153,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -237,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -453,68 +417,81 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def inline_editing(self, inline_editing: bool) -> typing.Self:    
+    def frame_index(self, frame_index: float) -> typing.Self:    
+        """
+        Represents the index of the selected frame
+        """
+            
+        if self._internal.options is None:
+            self._internal.options = table.Options()
+        assert isinstance(self._internal.options, table.Options)
+        self._internal.options.frame_index = frame_index
+    
+        return self
+    
+    def show_header(self, show_header: bool) -> typing.Self:    
         """
-        Enable inline editing
+        Controls whether the panel should show the header
         """
             
         if self._internal.options is None:
-            self._internal.options = canvas.Options()
-        assert isinstance(self._internal.options, canvas.Options)
-        self._internal.options.inline_editing = inline_editing
+            self._internal.options = table.Options()
+        assert isinstance(self._internal.options, table.Options)
+        self._internal.options.show_header = show_header
     
         return self
     
-    def show_advanced_types(self, show_advanced_types: bool) -> typing.Self:    
+    def show_type_icons(self, show_type_icons: bool) -> typing.Self:    
         """
-        Show all available element types
+        Controls whether the header should show icons for the column types
         """
             
         if self._internal.options is None:
-            self._internal.options = canvas.Options()
-        assert isinstance(self._internal.options, canvas.Options)
-        self._internal.options.show_advanced_types = show_advanced_types
+            self._internal.options = table.Options()
+        assert isinstance(self._internal.options, table.Options)
+        self._internal.options.show_type_icons = show_type_icons
     
         return self
     
-    def pan_zoom(self, pan_zoom: bool) -> typing.Self:    
+    def sort_by(self, sort_by: list[cogbuilder.Builder[common.TableSortByFieldState]]) -> typing.Self:    
         """
-        Enable pan and zoom
+        Used to control row sorting
         """
             
         if self._internal.options is None:
-            self._internal.options = canvas.Options()
-        assert isinstance(self._internal.options, canvas.Options)
-        self._internal.options.pan_zoom = pan_zoom
+            self._internal.options = table.Options()
+        assert isinstance(self._internal.options, table.Options)
+        sort_by_resources = [r1.build() for r1 in sort_by]
+        self._internal.options.sort_by = sort_by_resources
     
         return self
     
-    def infinite_pan(self, infinite_pan: bool) -> typing.Self:    
+    def footer(self, footer: cogbuilder.Builder[common.TableFooterOptions]) -> typing.Self:    
         """
-        Enable infinite pan
+        Controls footer options
         """
             
         if self._internal.options is None:
-            self._internal.options = canvas.Options()
-        assert isinstance(self._internal.options, canvas.Options)
-        self._internal.options.infinite_pan = infinite_pan
+            self._internal.options = table.Options()
+        assert isinstance(self._internal.options, table.Options)
+        footer_resource = footer.build()
+        self._internal.options.footer = footer_resource
     
         return self
     
-    def root(self, root: canvas.CanvasOptionsRoot) -> typing.Self:    
+    def cell_height(self, cell_height: common.TableCellHeight) -> typing.Self:    
         """
-        The root element of canvas (frame), where all canvas elements are nested
-        TODO: Figure out how to define a default value for this
+        Controls the height of the rows
         """
             
         if self._internal.options is None:
-            self._internal.options = canvas.Options()
-        assert isinstance(self._internal.options, canvas.Options)
-        self._internal.options.root = root
+            self._internal.options = table.Options()
+        assert isinstance(self._internal.options, table.Options)
+        self._internal.options.cell_height = cell_height
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/cloudwatch.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/cloudwatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,15 +191,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -630,15 +632,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -774,15 +778,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/common.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -616,19 +618,14 @@
         return self
     
     def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
         self._internal.axis_centered_zero = axis_centered_zero
     
         return self
     
-    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
-        self._internal.axis_border_show = axis_border_show
-    
-        return self
-    
 
 class HideSeriesConfig(cogbuilder.Builder[common.HideSeriesConfig]):    
     """
     TODO docs
     """
     
     _internal: common.HideSeriesConfig
@@ -728,15 +725,15 @@
 
     def __init__(self):
         self._internal = common.GraphThresholdsStyleConfig()
 
     def build(self) -> common.GraphThresholdsStyleConfig:
         return self._internal    
     
-    def mode(self, mode: common.GraphThresholdsStyleMode) -> typing.Self:        
+    def mode(self, mode: common.GraphTresholdsStyleMode) -> typing.Self:        
         self._internal.mode = mode
     
         return self
     
 
 class SingleStatBaseOptions(cogbuilder.Builder[common.SingleStatBaseOptions]):    
     """
@@ -1042,19 +1039,14 @@
     
     def scale_distribution(self, scale_distribution: cogbuilder.Builder[common.ScaleDistributionConfig]) -> typing.Self:        
         scale_distribution_resource = scale_distribution.build()
         self._internal.scale_distribution = scale_distribution_resource
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
-        self._internal.axis_centered_zero = axis_centered_zero
-    
-        return self
-    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         self._internal.bar_alignment = bar_alignment
     
         return self
     
     def bar_width_factor(self, bar_width_factor: float) -> typing.Self:        
         self._internal.bar_width_factor = bar_width_factor
@@ -1095,16 +1087,16 @@
         return self
     
     def point_symbol(self, point_symbol: str) -> typing.Self:        
         self._internal.point_symbol = point_symbol
     
         return self
     
-    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
-        self._internal.axis_border_show = axis_border_show
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        self._internal.axis_centered_zero = axis_centered_zero
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         self._internal.bar_max_width = bar_max_width
     
         return self
@@ -1193,24 +1185,14 @@
         return self
     
     def sort(self, sort: common.SortOrder) -> typing.Self:        
         self._internal.sort = sort
     
         return self
     
-    def max_width(self, max_width: float) -> typing.Self:        
-        self._internal.max_width = max_width
-    
-        return self
-    
-    def max_height(self, max_height: float) -> typing.Self:        
-        self._internal.max_height = max_height
-    
-        return self
-    
 
 class TableSortByFieldState(cogbuilder.Builder[common.TableSortByFieldState]):    
     """
     Sort by field state
     """
     
     _internal: common.TableSortByFieldState
@@ -1421,19 +1403,14 @@
     
     def scale_distribution(self, scale_distribution: cogbuilder.Builder[common.ScaleDistributionConfig]) -> typing.Self:        
         scale_distribution_resource = scale_distribution.build()
         self._internal.scale_distribution = scale_distribution_resource
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
-        self._internal.axis_centered_zero = axis_centered_zero
-    
-        return self
-    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         self._internal.bar_alignment = bar_alignment
     
         return self
     
     def bar_width_factor(self, bar_width_factor: float) -> typing.Self:        
         self._internal.bar_width_factor = bar_width_factor
@@ -1448,19 +1425,14 @@
     
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
         hide_from_resource = hide_from.build()
         self._internal.hide_from = hide_from_resource
     
         return self
     
-    def hide_value(self, hide_value: bool) -> typing.Self:        
-        self._internal.hide_value = hide_value
-    
-        return self
-    
     def transform(self, transform: common.GraphTransform) -> typing.Self:        
         self._internal.transform = transform
     
         return self
     
     def span_nulls(self, span_nulls: typing.Union[bool, float]) -> typing.Self:    
         """
@@ -1479,16 +1451,16 @@
         return self
     
     def point_symbol(self, point_symbol: str) -> typing.Self:        
         self._internal.point_symbol = point_symbol
     
         return self
     
-    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
-        self._internal.axis_border_show = axis_border_show
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        self._internal.axis_centered_zero = axis_centered_zero
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         self._internal.bar_max_width = bar_max_width
     
         return self
@@ -1509,19 +1481,14 @@
         return self._internal    
     
     def mode(self, mode: common.TableCellBackgroundDisplayMode) -> typing.Self:        
         self._internal.mode = mode
     
         return self
     
-    def apply_to_row(self, apply_to_row: bool) -> typing.Self:        
-        self._internal.apply_to_row = apply_to_row
-    
-        return self
-    
 
 class DataSourceRef(cogbuilder.Builder[common.DataSourceRef]):    
     _internal: common.DataSourceRef
 
     def __init__(self):
         self._internal = common.DataSourceRef()
 
@@ -1723,14 +1690,14 @@
     def filterable(self, filterable: bool) -> typing.Self:        
         self._internal.filterable = filterable
     
         return self
     
     def hide_header(self, hide_header: bool) -> typing.Self:    
         """
-        Hides any header for a column, useful for columns that show some static content or buttons.
+        Hides any header for a column, usefull for columns that show some static content or buttons.
         """
             
         self._internal.hide_header = hide_header
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/dashboard.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,24 @@
         Tags associated with dashboard.
         """
             
         self._internal.tags = tags
     
         return self
     
+    def style(self, style: typing.Literal["light", "dark"]) -> typing.Self:    
+        """
+        Theme of dashboard.
+        Default value: dark.
+        """
+            
+        self._internal.style = style
+    
+        return self
+    
     def timezone(self, timezone: str) -> typing.Self:    
         """
         Timezone of dashboard. Accepted values are IANA TZDB zone ID or "browser" or "utc".
         """
             
         self._internal.timezone = timezone
     
@@ -134,15 +144,15 @@
         if self._internal.time is None:
             self._internal.time = dashboard.DashboardDashboardTime()
         assert isinstance(self._internal.time, dashboard.DashboardDashboardTime)
         self._internal.time.to = to
     
         return self
     
-    def timepicker(self, timepicker: cogbuilder.Builder[dashboard.TimePickerConfig]) -> typing.Self:    
+    def timepicker(self, timepicker: cogbuilder.Builder[dashboard.TimePicker]) -> typing.Self:    
         """
         Configuration of the time picker shown at the top of a dashboard.
         """
             
         timepicker_resource = timepicker.build()
         self._internal.timepicker = timepicker_resource
     
@@ -175,15 +185,15 @@
         Day when the week starts. Expressed by the name of the day in lowercase, e.g. "monday".
         """
             
         self._internal.week_start = week_start
     
         return self
     
-    def refresh(self, refresh: str) -> typing.Self:    
+    def refresh(self, refresh: typing.Union[str, typing.Literal[False]]) -> typing.Self:    
         """
         Refresh rate of dashboard. Represented via interval string, e.g. "5s", "1m", "1h", "1d".
         """
             
         self._internal.refresh = refresh
     
         return self
@@ -535,23 +545,14 @@
         TODO -- this should not exist here, it is based on the --grafana-- datasource
         """
             
         self._internal.type_val = type_val
     
         return self
     
-    def built_in(self, built_in: float) -> typing.Self:    
-        """
-        Set to 1 for the standard annotation query all dashboards have by default.
-        """
-            
-        self._internal.built_in = built_in
-    
-        return self
-    
 
 class DashboardLink(cogbuilder.Builder[dashboard.DashboardLink]):    
     """
     Links with references to other dashboards or external resources
     """
     
     _internal: dashboard.DashboardLink
@@ -823,65 +824,14 @@
     def options(self, options: cogbuilder.Builder[dashboard.DashboardSpecialValueMapOptions]) -> typing.Self:        
         options_resource = options.build()
         self._internal.options = options_resource
     
         return self
     
 
-class TimePicker(cogbuilder.Builder[dashboard.TimePickerConfig]):    
-    """
-    Time picker configuration
-    It defines the default config for the time picker and the refresh picker for the specific dashboard.
-    """
-    
-    _internal: dashboard.TimePickerConfig
-
-    def __init__(self):
-        self._internal = dashboard.TimePickerConfig()
-
-    def build(self) -> dashboard.TimePickerConfig:
-        return self._internal    
-    
-    def hidden(self, hidden: bool) -> typing.Self:    
-        """
-        Whether timepicker is visible or not.
-        """
-            
-        self._internal.hidden = hidden
-    
-        return self
-    
-    def refresh_intervals(self, refresh_intervals: list[str]) -> typing.Self:    
-        """
-        Interval options available in the refresh picker dropdown.
-        """
-            
-        self._internal.refresh_intervals = refresh_intervals
-    
-        return self
-    
-    def time_options(self, time_options: list[str]) -> typing.Self:    
-        """
-        Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
-        """
-            
-        self._internal.time_options = time_options
-    
-        return self
-    
-    def now_delay(self, now_delay: str) -> typing.Self:    
-        """
-        Override the now time by entering a time delay. Use this option to accommodate known delays in data aggregation to avoid null values.
-        """
-            
-        self._internal.now_delay = now_delay
-    
-        return self
-    
-
 class Snapshot(cogbuilder.Builder[dashboard.Snapshot]):    
     """
     A dashboard snapshot shares an interactive dashboard publicly.
     It is a read-only version of a dashboard, and is not editable.
     It is possible to create a snapshot of a snapshot.
     Grafana strips away all sensitive information from the dashboard.
     Sensitive information stripped: queries (metric, template,annotation) and panel links.
@@ -927,23 +877,14 @@
         external url, if snapshot was shared in external grafana instance
         """
             
         self._internal.external_url = external_url
     
         return self
     
-    def original_url(self, original_url: str) -> typing.Self:    
-        """
-        original url, url of the dashboard that was snapshotted
-        """
-            
-        self._internal.original_url = original_url
-    
-        return self
-    
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the snapshot
         """
             
         self._internal.id_val = id_val
     
@@ -1160,24 +1101,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -1244,50 +1175,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -1535,14 +1439,95 @@
         """
             
         self._internal.repeat = repeat
     
         return self
     
 
+class GraphPanel(cogbuilder.Builder[dashboard.GraphPanel]):    
+    """
+    Support for legacy graph panel.
+    @deprecated this a deprecated panel type
+    """
+    
+    _internal: dashboard.GraphPanel
+
+    def __init__(self):
+        self._internal = dashboard.GraphPanel()        
+        self._internal.type_val = "graph"
+
+    def build(self) -> dashboard.GraphPanel:
+        return self._internal    
+    
+    def legend(self, legend: cogbuilder.Builder[dashboard.DashboardGraphPanelLegend]) -> typing.Self:    
+        """
+        @deprecated this is part of deprecated graph panel
+        """
+            
+        legend_resource = legend.build()
+        self._internal.legend = legend_resource
+    
+        return self
+    
+
+class TimePicker(cogbuilder.Builder[dashboard.TimePicker]):    
+    _internal: dashboard.TimePicker
+
+    def __init__(self):
+        self._internal = dashboard.TimePicker()
+
+    def build(self) -> dashboard.TimePicker:
+        return self._internal    
+    
+    def hidden(self, hidden: bool) -> typing.Self:    
+        """
+        Whether timepicker is visible or not.
+        """
+            
+        self._internal.hidden = hidden
+    
+        return self
+    
+    def refresh_intervals(self, refresh_intervals: list[str]) -> typing.Self:    
+        """
+        Interval options available in the refresh picker dropdown.
+        """
+            
+        self._internal.refresh_intervals = refresh_intervals
+    
+        return self
+    
+    def collapse(self, collapse: bool) -> typing.Self:    
+        """
+        Whether timepicker is collapsed or not. Has no effect on provisioned dashboard.
+        """
+            
+        self._internal.collapse = collapse
+    
+        return self
+    
+    def enable(self, enable: bool) -> typing.Self:    
+        """
+        Whether timepicker is enabled or not. Has no effect on provisioned dashboard.
+        """
+            
+        self._internal.enable = enable
+    
+        return self
+    
+    def time_options(self, time_options: list[str]) -> typing.Self:    
+        """
+        Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
+        """
+            
+        self._internal.time_options = time_options
+    
+        return self
+    
+
 class DashboardDashboardTemplating(cogbuilder.Builder[dashboard.DashboardDashboardTemplating]):    
     _internal: dashboard.DashboardDashboardTemplating
 
     def __init__(self):
         self._internal = dashboard.DashboardDashboardTemplating()
 
     def build(self) -> dashboard.DashboardDashboardTemplating:
@@ -1668,14 +1653,39 @@
     
     def properties(self, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:        
         self._internal.properties = properties
     
         return self
     
 
+class DashboardGraphPanelLegend(cogbuilder.Builder[dashboard.DashboardGraphPanelLegend]):    
+    _internal: dashboard.DashboardGraphPanelLegend
+
+    def __init__(self):
+        self._internal = dashboard.DashboardGraphPanelLegend()
+
+    def build(self) -> dashboard.DashboardGraphPanelLegend:
+        return self._internal    
+    
+    def show(self, show: bool) -> typing.Self:        
+        self._internal.show = show
+    
+        return self
+    
+    def sort(self, sort: str) -> typing.Self:        
+        self._internal.sort = sort
+    
+        return self
+    
+    def sort_desc(self, sort_desc: bool) -> typing.Self:        
+        self._internal.sort_desc = sort_desc
+    
+        return self
+    
+
 class QueryVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
 
@@ -1683,14 +1693,23 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.QUERY
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
+    def id_val(self, id_val: str) -> typing.Self:    
+        """
+        Unique numeric identifier for the variable.
+        """
+            
+        self._internal.id_val = id_val
+    
+        return self
+    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -1737,14 +1756,23 @@
         Data source used to fetch values for a variable. It can be defined but `null`.
         """
             
         self._internal.datasource = datasource
     
         return self
     
+    def all_format(self, all_format: str) -> typing.Self:    
+        """
+        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
+        """
+            
+        self._internal.all_format = all_format
+    
+        return self
+    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
     
@@ -1826,14 +1854,23 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.ADHOC
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
+    def id_val(self, id_val: str) -> typing.Self:    
+        """
+        Unique numeric identifier for the variable.
+        """
+            
+        self._internal.id_val = id_val
+    
+        return self
+    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -1871,14 +1908,23 @@
         Data source used to fetch values for a variable. It can be defined but `null`.
         """
             
         self._internal.datasource = datasource
     
         return self
     
+    def all_format(self, all_format: str) -> typing.Self:    
+        """
+        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
+        """
+            
+        self._internal.all_format = all_format
+    
+        return self
+    
 
 class ConstantVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
@@ -1887,14 +1933,23 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.CONSTANT
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
+    def id_val(self, id_val: str) -> typing.Self:    
+        """
+        Unique numeric identifier for the variable.
+        """
+            
+        self._internal.id_val = id_val
+    
+        return self
+    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -1923,14 +1978,23 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
+    def all_format(self, all_format: str) -> typing.Self:    
+        """
+        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
+        """
+            
+        self._internal.all_format = all_format
+    
+        return self
+    
 
 class DatasourceVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
@@ -1939,14 +2003,23 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.DATASOURCE
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
+    def id_val(self, id_val: str) -> typing.Self:    
+        """
+        Unique numeric identifier for the variable.
+        """
+            
+        self._internal.id_val = id_val
+    
+        return self
+    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -1984,14 +2057,23 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
+    def all_format(self, all_format: str) -> typing.Self:    
+        """
+        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
+        """
+            
+        self._internal.all_format = all_format
+    
+        return self
+    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
     
@@ -2046,14 +2128,23 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.INTERVAL
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
+    def id_val(self, id_val: str) -> typing.Self:    
+        """
+        Unique numeric identifier for the variable.
+        """
+            
+        self._internal.id_val = id_val
+    
+        return self
+    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -2091,14 +2182,23 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
+    def all_format(self, all_format: str) -> typing.Self:    
+        """
+        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
+        """
+            
+        self._internal.all_format = all_format
+    
+        return self
+    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
     
@@ -2125,14 +2225,23 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.TEXTBOX
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
+    def id_val(self, id_val: str) -> typing.Self:    
+        """
+        Unique numeric identifier for the variable.
+        """
+            
+        self._internal.id_val = id_val
+    
+        return self
+    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -2170,14 +2279,23 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
+    def all_format(self, all_format: str) -> typing.Self:    
+        """
+        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
+        """
+            
+        self._internal.all_format = all_format
+    
+        return self
+    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
     
@@ -2204,14 +2322,23 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.CUSTOM
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
+    def id_val(self, id_val: str) -> typing.Self:    
+        """
+        Unique numeric identifier for the variable.
+        """
+            
+        self._internal.id_val = id_val
+    
+        return self
+    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -2249,14 +2376,23 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
+    def all_format(self, all_format: str) -> typing.Self:    
+        """
+        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
+        """
+            
+        self._internal.all_format = all_format
+    
+        return self
+    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/dashboardlist.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/bargauge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import dashboardlist
+from ..models import common
+from ..models import bargauge
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "dashlist"
+        self._internal.type_val = "bargauge"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -153,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -237,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -453,91 +417,73 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def keep_time(self, keep_time: bool) -> typing.Self:        
+    def display_mode(self, display_mode: common.BarGaugeDisplayMode) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.keep_time = keep_time
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.display_mode = display_mode
     
         return self
     
-    def include_vars(self, include_vars: bool) -> typing.Self:        
+    def value_mode(self, value_mode: common.BarGaugeValueMode) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.include_vars = include_vars
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.value_mode = value_mode
     
         return self
     
-    def show_starred(self, show_starred: bool) -> typing.Self:        
+    def show_unfilled(self, show_unfilled: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.show_starred = show_starred
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.show_unfilled = show_unfilled
     
         return self
     
-    def show_recently_viewed(self, show_recently_viewed: bool) -> typing.Self:        
+    def min_viz_width(self, min_viz_width: int) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.show_recently_viewed = show_recently_viewed
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.min_viz_width = min_viz_width
     
         return self
     
-    def show_search(self, show_search: bool) -> typing.Self:        
+    def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.show_search = show_search
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        reduce_options_resource = reduce_options.build()
+        self._internal.options.reduce_options = reduce_options_resource
     
         return self
     
-    def show_headings(self, show_headings: bool) -> typing.Self:        
+    def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.show_headings = show_headings
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        text_resource = text.build()
+        self._internal.options.text = text_resource
     
         return self
     
-    def max_items(self, max_items: int) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.max_items = max_items
-    
-        return self
-    
-    def query(self, query: str) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.query = query
-    
-        return self
-    
-    def folder_id(self, folder_id: int) -> typing.Self:    
-        """
-        folderId is deprecated, and migrated to folderUid on panel init
-        """
-            
+    def min_viz_height(self, min_viz_height: int) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.folder_id = folder_id
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.min_viz_height = min_viz_height
     
         return self
     
-    def folder_uid(self, folder_uid: str) -> typing.Self:        
+    def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = dashboardlist.Options()
-        assert isinstance(self._internal.options, dashboardlist.Options)
-        self._internal.options.folder_uid = folder_uid
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.orientation = orientation
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/datagrid.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/datagrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,24 +153,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -237,50 +227,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/debug.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/news.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import debug
+from ..models import news
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "debug"
+        self._internal.type_val = "news"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -153,24 +153,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -237,50 +227,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -453,23 +416,27 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def mode(self, mode: debug.DebugMode) -> typing.Self:        
+    def feed_url(self, feed_url: str) -> typing.Self:    
+        """
+        empty/missing will default to grafana blog
+        """
+            
         if self._internal.options is None:
-            self._internal.options = debug.Options()
-        assert isinstance(self._internal.options, debug.Options)
-        self._internal.options.mode = mode
+            self._internal.options = news.Options()
+        assert isinstance(self._internal.options, news.Options)
+        self._internal.options.feed_url = feed_url
     
         return self
     
-    def counters(self, counters: debug.UpdateConfig) -> typing.Self:        
+    def show_image(self, show_image: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = debug.Options()
-        assert isinstance(self._internal.options, debug.Options)
-        self._internal.options.counters = counters
+            self._internal.options = news.Options()
+        assert isinstance(self._internal.options, news.Options)
+        self._internal.options.show_image = show_image
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/elasticsearch.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/elasticsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1437,15 +1437,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/expr.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/expr.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/gauge.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/piechart.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import gauge
+from ..models import piechart
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "gauge"
+        self._internal.type_val = "piechart"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -454,73 +417,81 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def show_threshold_labels(self, show_threshold_labels: bool) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        self._internal.options.show_threshold_labels = show_threshold_labels
-    
-        return self
-    
-    def show_threshold_markers(self, show_threshold_markers: bool) -> typing.Self:        
+    def pie_type(self, pie_type: piechart.PieChartType) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        self._internal.options.show_threshold_markers = show_threshold_markers
+            self._internal.options = piechart.Options()
+        assert isinstance(self._internal.options, piechart.Options)
+        self._internal.options.pie_type = pie_type
     
         return self
     
-    def sizing(self, sizing: common.BarGaugeSizing) -> typing.Self:        
+    def display_labels(self, display_labels: list[piechart.PieChartLabels]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        self._internal.options.sizing = sizing
+            self._internal.options = piechart.Options()
+        assert isinstance(self._internal.options, piechart.Options)
+        self._internal.options.display_labels = display_labels
     
         return self
     
-    def min_viz_width(self, min_viz_width: int) -> typing.Self:        
+    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        self._internal.options.min_viz_width = min_viz_width
+            self._internal.options = piechart.Options()
+        assert isinstance(self._internal.options, piechart.Options)
+        tooltip_resource = tooltip.build()
+        self._internal.options.tooltip = tooltip_resource
     
         return self
     
     def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
+            self._internal.options = piechart.Options()
+        assert isinstance(self._internal.options, piechart.Options)
         reduce_options_resource = reduce_options.build()
         self._internal.options.reduce_options = reduce_options_resource
     
         return self
     
     def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
+            self._internal.options = piechart.Options()
+        assert isinstance(self._internal.options, piechart.Options)
         text_resource = text.build()
         self._internal.options.text = text_resource
     
         return self
     
-    def min_viz_height(self, min_viz_height: int) -> typing.Self:        
+    def legend(self, legend: piechart.PieChartLegendOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        self._internal.options.min_viz_height = min_viz_height
+            self._internal.options = piechart.Options()
+        assert isinstance(self._internal.options, piechart.Options)
+        self._internal.options.legend = legend
     
         return self
     
     def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
+            self._internal.options = piechart.Options()
+        assert isinstance(self._internal.options, piechart.Options)
         self._internal.options.orientation = orientation
     
         return self
+    
+    def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = piechart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, piechart.FieldConfig)
+        hide_from_resource = hide_from.build()
+        self._internal.field_config.defaults.custom.hide_from = hide_from_resource
+    
+        return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/geomap.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/geomap.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -81,24 +83,14 @@
         """
             
         slo_query_resource = slo_query.build()
         self._internal.slo_query = slo_query_resource
     
         return self
     
-    def prom_ql_query(self, prom_ql_query: cogbuilder.Builder[googlecloudmonitoring.PromQLQuery]) -> typing.Self:    
-        """
-        PromQL sub-query properties.
-        """
-            
-        prom_ql_query_resource = prom_ql_query.build()
-        self._internal.prom_ql_query = prom_ql_query_resource
-    
-        return self
-    
     def datasource(self, datasource: object) -> typing.Self:    
         """
         For mixed data sources the selected datasource is on the query level.
         For non mixed scenarios this is undefined.
         TODO find a better way to do this ^ that's friendly to schema
         TODO this shouldn't be unknown but DataSourceRef | null
         """
@@ -189,14 +181,59 @@
         Data view, defaults to FULL.
         """
             
         self._internal.view = view
     
         return self
     
+    def secondary_cross_series_reducer(self, secondary_cross_series_reducer: str) -> typing.Self:    
+        """
+        Only present if a preprocessor is selected. Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
+        """
+            
+        self._internal.secondary_cross_series_reducer = secondary_cross_series_reducer
+    
+        return self
+    
+    def secondary_alignment_period(self, secondary_alignment_period: str) -> typing.Self:    
+        """
+        Only present if a preprocessor is selected. Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
+        """
+            
+        self._internal.secondary_alignment_period = secondary_alignment_period
+    
+        return self
+    
+    def secondary_per_series_aligner(self, secondary_per_series_aligner: str) -> typing.Self:    
+        """
+        Only present if a preprocessor is selected. Alignment function to be used. Defaults to ALIGN_MEAN.
+        """
+            
+        self._internal.secondary_per_series_aligner = secondary_per_series_aligner
+    
+        return self
+    
+    def secondary_group_bys(self, secondary_group_bys: list[str]) -> typing.Self:    
+        """
+        Only present if a preprocessor is selected. Array of labels to group data by.
+        """
+            
+        self._internal.secondary_group_bys = secondary_group_bys
+    
+        return self
+    
+    def preprocessor(self, preprocessor: googlecloudmonitoring.PreprocessorType) -> typing.Self:    
+        """
+        Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
+        """
+            
+        self._internal.preprocessor = preprocessor
+    
+        return self
+    
     def title(self, title: str) -> typing.Self:    
         """
         Annotation title.
         """
             
         self._internal.title = title
     
@@ -207,14 +244,91 @@
         Annotation text.
         """
             
         self._internal.text = text
     
         return self
     
+
+class AnnotationQuery(cogbuilder.Builder[googlecloudmonitoring.AnnotationQuery]):    
+    """
+    Annotation sub-query properties.
+    """
+    
+    _internal: googlecloudmonitoring.AnnotationQuery
+
+    def __init__(self):
+        self._internal = googlecloudmonitoring.AnnotationQuery()
+
+    def build(self) -> googlecloudmonitoring.AnnotationQuery:
+        return self._internal    
+    
+    def project_name(self, project_name: str) -> typing.Self:    
+        """
+        GCP project to execute the query against.
+        """
+            
+        self._internal.project_name = project_name
+    
+        return self
+    
+    def cross_series_reducer(self, cross_series_reducer: str) -> typing.Self:    
+        """
+        Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
+        """
+            
+        self._internal.cross_series_reducer = cross_series_reducer
+    
+        return self
+    
+    def alignment_period(self, alignment_period: str) -> typing.Self:    
+        """
+        Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
+        """
+            
+        self._internal.alignment_period = alignment_period
+    
+        return self
+    
+    def per_series_aligner(self, per_series_aligner: str) -> typing.Self:    
+        """
+        Alignment function to be used. Defaults to ALIGN_MEAN.
+        """
+            
+        self._internal.per_series_aligner = per_series_aligner
+    
+        return self
+    
+    def group_bys(self, group_bys: list[str]) -> typing.Self:    
+        """
+        Array of labels to group data by.
+        """
+            
+        self._internal.group_bys = group_bys
+    
+        return self
+    
+    def filters(self, filters: list[str]) -> typing.Self:    
+        """
+        Array of filters to query data by. Labels that can be filtered on are defined by the metric.
+        """
+            
+        self._internal.filters = filters
+    
+        return self
+    
+    def view(self, view: str) -> typing.Self:    
+        """
+        Data view, defaults to FULL.
+        """
+            
+        self._internal.view = view
+    
+        return self
+    
     def secondary_cross_series_reducer(self, secondary_cross_series_reducer: str) -> typing.Self:    
         """
         Only present if a preprocessor is selected. Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
         """
             
         self._internal.secondary_cross_series_reducer = secondary_cross_series_reducer
     
@@ -243,23 +357,41 @@
         Only present if a preprocessor is selected. Array of labels to group data by.
         """
             
         self._internal.secondary_group_bys = secondary_group_bys
     
         return self
     
+    def title(self, title: str) -> typing.Self:    
+        """
+        Annotation title.
+        """
+            
+        self._internal.title = title
+    
+        return self
+    
     def preprocessor(self, preprocessor: googlecloudmonitoring.PreprocessorType) -> typing.Self:    
         """
         Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
         """
             
         self._internal.preprocessor = preprocessor
     
         return self
     
+    def text(self, text: str) -> typing.Self:    
+        """
+        Annotation text.
+        """
+            
+        self._internal.text = text
+    
+        return self
+    
 
 class TimeSeriesQuery(cogbuilder.Builder[googlecloudmonitoring.TimeSeriesQuery]):    
     """
     Time Series sub-query properties.
     """
     
     _internal: googlecloudmonitoring.TimeSeriesQuery
@@ -398,55 +530,14 @@
         """
             
         self._internal.lookback_period = lookback_period
     
         return self
     
 
-class PromQLQuery(cogbuilder.Builder[googlecloudmonitoring.PromQLQuery]):    
-    """
-    PromQL sub-query properties.
-    """
-    
-    _internal: googlecloudmonitoring.PromQLQuery
-
-    def __init__(self):
-        self._internal = googlecloudmonitoring.PromQLQuery()
-
-    def build(self) -> googlecloudmonitoring.PromQLQuery:
-        return self._internal    
-    
-    def project_name(self, project_name: str) -> typing.Self:    
-        """
-        GCP project to execute the query against.
-        """
-            
-        self._internal.project_name = project_name
-    
-        return self
-    
-    def expr(self, expr: str) -> typing.Self:    
-        """
-        PromQL expression/query to be executed.
-        """
-            
-        self._internal.expr = expr
-    
-        return self
-    
-    def step(self, step: str) -> typing.Self:    
-        """
-        PromQL min step
-        """
-            
-        self._internal.step = step
-    
-        return self
-    
-
 class MetricQuery(cogbuilder.Builder[googlecloudmonitoring.MetricQuery]):    
     """
     @deprecated This type is for migration purposes only. Replaced by TimeSeriesList Metric sub-query properties.
     """
     
     _internal: googlecloudmonitoring.MetricQuery
 
@@ -570,15 +661,15 @@
         self._internal.graph_period = graph_period
     
         return self
     
 
 class LegacyCloudMonitoringAnnotationQuery(cogbuilder.Builder[googlecloudmonitoring.LegacyCloudMonitoringAnnotationQuery]):    
     """
-    @deprecated Use TimeSeriesList instead. Legacy annotation query properties for migration purposes.
+    @deprecated Use AnnotationQuery instead. Legacy annotation query properties for migration purposes.
     """
     
     _internal: googlecloudmonitoring.LegacyCloudMonitoringAnnotationQuery
 
     def __init__(self):
         self._internal = googlecloudmonitoring.LegacyCloudMonitoringAnnotationQuery()
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/grafanapyroscope.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/grafanapyroscope.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,23 +19,14 @@
         Specifies the query label selectors.
         """
             
         self._internal.label_selector = label_selector
     
         return self
     
-    def span_selector(self, span_selector: list[str]) -> typing.Self:    
-        """
-        Specifies the query span selectors.
-        """
-            
-        self._internal.span_selector = span_selector
-    
-        return self
-    
     def profile_type_id(self, profile_type_id: str) -> typing.Self:    
         """
         Specifies the type of profile to query.
         """
             
         self._internal.profile_type_id = profile_type_id
     
@@ -68,15 +59,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/heatmap.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/heatmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -616,48 +579,41 @@
         if self._internal.options.legend is None:
             self._internal.options.legend = heatmap.HeatmapLegend()
         assert isinstance(self._internal.options.legend, heatmap.HeatmapLegend)
         self._internal.options.legend.show = False
     
         return self
     
-    def mode(self, mode: common.TooltipDisplayMode) -> typing.Self:    
+    def show_tooltip(self) -> typing.Self:    
         """
-        Controls how the tooltip is shown
+        Controls if the tooltip is shown
         """
             
         if self._internal.options is None:
             self._internal.options = heatmap.Options()
         assert isinstance(self._internal.options, heatmap.Options)
         if self._internal.options.tooltip is None:
             self._internal.options.tooltip = heatmap.HeatmapTooltip()
         assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
-        self._internal.options.tooltip.mode = mode
+        self._internal.options.tooltip.show = True
     
         return self
     
-    def max_height(self, max_height: float) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = heatmap.Options()
-        assert isinstance(self._internal.options, heatmap.Options)
-        if self._internal.options.tooltip is None:
-            self._internal.options.tooltip = heatmap.HeatmapTooltip()
-        assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
-        self._internal.options.tooltip.max_height = max_height
-    
-        return self
-    
-    def max_width(self, max_width: float) -> typing.Self:        
+    def hide_tooltip(self) -> typing.Self:    
+        """
+        Controls if the tooltip is shown
+        """
+            
         if self._internal.options is None:
             self._internal.options = heatmap.Options()
         assert isinstance(self._internal.options, heatmap.Options)
         if self._internal.options.tooltip is None:
             self._internal.options.tooltip = heatmap.HeatmapTooltip()
         assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
-        self._internal.options.tooltip.max_width = max_width
+        self._internal.options.tooltip.show = False
     
         return self
     
     def show_y_histogram(self) -> typing.Self:    
         """
         Controls if the tooltip shows a histogram of the y-axis values
         """
@@ -683,29 +639,14 @@
         if self._internal.options.tooltip is None:
             self._internal.options.tooltip = heatmap.HeatmapTooltip()
         assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
         self._internal.options.tooltip.y_histogram = False
     
         return self
     
-    def show_color_scale(self, show_color_scale: bool) -> typing.Self:    
-        """
-        Controls if the tooltip shows a color scale in header
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = heatmap.Options()
-        assert isinstance(self._internal.options, heatmap.Options)
-        if self._internal.options.tooltip is None:
-            self._internal.options.tooltip = heatmap.HeatmapTooltip()
-        assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
-        self._internal.options.tooltip.show_color_scale = show_color_scale
-    
-        return self
-    
     def exemplars_color(self, color: str) -> typing.Self:    
         """
         Controls exemplar options
         """
             
         if self._internal.options is None:
             self._internal.options = heatmap.Options()
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/histogram.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/histogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -454,41 +417,27 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def bucket_count(self, bucket_count: int) -> typing.Self:    
-        """
-        Bucket count (approx)
-        """
-            
-        if not bucket_count > 0:
-            raise ValueError("bucket_count must be > 0")
-        if self._internal.options is None:
-            self._internal.options = histogram.Options()
-        assert isinstance(self._internal.options, histogram.Options)
-        self._internal.options.bucket_count = bucket_count
-    
-        return self
-    
     def bucket_size(self, bucket_size: int) -> typing.Self:    
         """
         Size of each bucket
         """
             
         if self._internal.options is None:
             self._internal.options = histogram.Options()
         assert isinstance(self._internal.options, histogram.Options)
         self._internal.options.bucket_size = bucket_size
     
         return self
     
-    def bucket_offset(self, bucket_offset: float) -> typing.Self:    
+    def bucket_offset(self, bucket_offset: int) -> typing.Self:    
         """
         Offset buckets by this amount
         """
             
         if self._internal.options is None:
             self._internal.options = histogram.Options()
         assert isinstance(self._internal.options, histogram.Options)
@@ -675,28 +624,14 @@
             self._internal.field_config.defaults.custom = histogram.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = histogram.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
-    
-        return self
-    
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -704,29 +639,14 @@
             self._internal.field_config.defaults.custom = histogram.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
         hide_from_resource = hide_from.build()
         self._internal.field_config.defaults.custom.hide_from = hide_from_resource
     
         return self
     
-    def stacking(self, stacking: cogbuilder.Builder[common.StackingConfig]) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = histogram.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
-        stacking_resource = stacking.build()
-        self._internal.field_config.defaults.custom.stacking = stacking_resource
-    
-        return self
-    
     def gradient_mode(self, gradient_mode: common.GraphGradientMode) -> typing.Self:    
         """
         Set the mode of the gradient fill. Fill gradient is based on the line color. To change the color, use the standard color scheme field option.
         Gradient appearance is influenced by the Fill opacity setting.
         """
             
         if self._internal.field_config is None:
@@ -738,21 +658,21 @@
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = histogram.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
         self._internal.field_config.defaults.custom.gradient_mode = gradient_mode
     
         return self
     
-    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = histogram.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/librarypanel.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/librarypanel.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,14 +202,23 @@
         The version of the plugin that is used for this panel. This is used to find the plugin to display the panel and to migrate old panel configs.
         """
             
         self._internal.plugin_version = plugin_version
     
         return self
     
+    def tags(self, tags: list[str]) -> typing.Self:    
+        """
+        Tags for the panel.
+        """
+            
+        self._internal.tags = tags
+    
+        return self
+    
     def targets(self, targets: list[cogbuilder.Builder[cogvariants.Dataquery]]) -> typing.Self:    
         """
         Depends on the panel plugin. See the plugin documentation for details.
         """
             
         targets_resources = [r1.build() for r1 in targets]
         self._internal.targets = targets_resources
@@ -277,21 +286,20 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
+    def repeat_panel_id(self, repeat_panel_id: int) -> typing.Self:    
         """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
+        Id of the repeating panel.
         """
             
-        self._internal.max_per_row = max_per_row
+        self._internal.repeat_panel_id = repeat_panel_id
     
         return self
     
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
@@ -347,41 +355,14 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def options(self, options: object) -> typing.Self:    
         """
         It depends on the panel plugin. They are specified by the Options field in panel plugin schemas.
         """
             
         self._internal.options = options
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/logs.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/statetimeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import logs
 from ..models import common
+from ..models import statetimeline
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "logs"
+        self._internal.type_val = "state-timeline"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -454,79 +417,130 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def show_labels(self, show_labels: bool) -> typing.Self:        
+    def show_value(self, show_value: common.VisibilityMode) -> typing.Self:    
+        """
+        Show timeline values on chart
+        """
+            
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.show_labels = show_labels
+            self._internal.options = statetimeline.Options()
+        assert isinstance(self._internal.options, statetimeline.Options)
+        self._internal.options.show_value = show_value
     
         return self
     
-    def show_common_labels(self, show_common_labels: bool) -> typing.Self:        
+    def row_height(self, row_height: float) -> typing.Self:    
+        """
+        Controls the row height
+        """
+            
+        if not row_height <= 1:
+            raise ValueError("row_height must be <= 1")
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.show_common_labels = show_common_labels
+            self._internal.options = statetimeline.Options()
+        assert isinstance(self._internal.options, statetimeline.Options)
+        self._internal.options.row_height = row_height
     
         return self
     
-    def show_time(self, show_time: bool) -> typing.Self:        
+    def merge_values(self, merge_values: bool) -> typing.Self:    
+        """
+        Merge equal consecutive values
+        """
+            
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.show_time = show_time
+            self._internal.options = statetimeline.Options()
+        assert isinstance(self._internal.options, statetimeline.Options)
+        self._internal.options.merge_values = merge_values
     
         return self
     
-    def show_log_context_toggle(self, show_log_context_toggle: bool) -> typing.Self:        
+    def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.show_log_context_toggle = show_log_context_toggle
+            self._internal.options = statetimeline.Options()
+        assert isinstance(self._internal.options, statetimeline.Options)
+        legend_resource = legend.build()
+        self._internal.options.legend = legend_resource
     
         return self
     
-    def wrap_log_message(self, wrap_log_message: bool) -> typing.Self:        
+    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.wrap_log_message = wrap_log_message
+            self._internal.options = statetimeline.Options()
+        assert isinstance(self._internal.options, statetimeline.Options)
+        tooltip_resource = tooltip.build()
+        self._internal.options.tooltip = tooltip_resource
     
         return self
     
-    def prettify_log_message(self, prettify_log_message: bool) -> typing.Self:        
+    def timezone(self, timezone: list[common.TimeZone]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.prettify_log_message = prettify_log_message
+            self._internal.options = statetimeline.Options()
+        assert isinstance(self._internal.options, statetimeline.Options)
+        self._internal.options.timezone = timezone
     
         return self
     
-    def enable_log_details(self, enable_log_details: bool) -> typing.Self:        
+    def align_value(self, align_value: common.TimelineValueAlignment) -> typing.Self:    
+        """
+        Controls value alignment on the timelines
+        """
+            
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.enable_log_details = enable_log_details
+            self._internal.options = statetimeline.Options()
+        assert isinstance(self._internal.options, statetimeline.Options)
+        self._internal.options.align_value = align_value
     
         return self
     
-    def sort_order(self, sort_order: common.LogsSortOrder) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.sort_order = sort_order
+    def line_width(self, line_width: int) -> typing.Self:        
+        if not line_width <= 10:
+            raise ValueError("line_width must be <= 10")
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
+        self._internal.field_config.defaults.custom.line_width = line_width
     
         return self
     
-    def dedup_strategy(self, dedup_strategy: common.LogsDedupStrategy) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.dedup_strategy = dedup_strategy
+    def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
+        hide_from_resource = hide_from.build()
+        self._internal.field_config.defaults.custom.hide_from = hide_from_resource
+    
+        return self
+    
+    def fill_opacity(self, fill_opacity: int) -> typing.Self:        
+        if not fill_opacity <= 100:
+            raise ValueError("fill_opacity must be <= 100")
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
+        self._internal.field_config.defaults.custom.fill_opacity = fill_opacity
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/loki.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/loki.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,15 +91,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/news.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/alertgroups.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import news
+from ..models import alertgroups
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "news"
+        self._internal.type_val = "alertGroups"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -153,24 +153,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -237,50 +227,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -453,27 +416,43 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def feed_url(self, feed_url: str) -> typing.Self:    
+    def labels(self, labels: str) -> typing.Self:    
         """
-        empty/missing will default to grafana blog
+        Comma-separated list of values used to filter alert results
         """
             
         if self._internal.options is None:
-            self._internal.options = news.Options()
-        assert isinstance(self._internal.options, news.Options)
-        self._internal.options.feed_url = feed_url
+            self._internal.options = alertgroups.Options()
+        assert isinstance(self._internal.options, alertgroups.Options)
+        self._internal.options.labels = labels
     
         return self
     
-    def show_image(self, show_image: bool) -> typing.Self:        
+    def alertmanager(self, alertmanager: str) -> typing.Self:    
+        """
+        Name of the alertmanager used as a source for alerts
+        """
+            
+        if self._internal.options is None:
+            self._internal.options = alertgroups.Options()
+        assert isinstance(self._internal.options, alertgroups.Options)
+        self._internal.options.alertmanager = alertmanager
+    
+        return self
+    
+    def expand_all(self, expand_all: bool) -> typing.Self:    
+        """
+        Expand all alert groups by default
+        """
+            
         if self._internal.options is None:
-            self._internal.options = news.Options()
-        assert isinstance(self._internal.options, news.Options)
-        self._internal.options.show_image = show_image
+            self._internal.options = alertgroups.Options()
+        assert isinstance(self._internal.options, alertgroups.Options)
+        self._internal.options.expand_all = expand_all
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/nodegraph.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/nodegraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,24 +153,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -237,50 +227,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/parca.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/parca.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,15 +41,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/piechart.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/statushistory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import piechart
+from ..models import statushistory
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "piechart"
+        self._internal.type_val = "status-history"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -454,81 +417,122 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def pie_type(self, pie_type: piechart.PieChartType) -> typing.Self:        
+    def row_height(self, row_height: float) -> typing.Self:    
+        """
+        Set the height of the rows
+        """
+            
+        if not row_height >= 0:
+            raise ValueError("row_height must be >= 0")
+        if not row_height <= 1:
+            raise ValueError("row_height must be <= 1")
         if self._internal.options is None:
-            self._internal.options = piechart.Options()
-        assert isinstance(self._internal.options, piechart.Options)
-        self._internal.options.pie_type = pie_type
+            self._internal.options = statushistory.Options()
+        assert isinstance(self._internal.options, statushistory.Options)
+        self._internal.options.row_height = row_height
     
         return self
     
-    def display_labels(self, display_labels: list[piechart.PieChartLabels]) -> typing.Self:        
+    def show_value(self, show_value: common.VisibilityMode) -> typing.Self:    
+        """
+        Show values on the columns
+        """
+            
         if self._internal.options is None:
-            self._internal.options = piechart.Options()
-        assert isinstance(self._internal.options, piechart.Options)
-        self._internal.options.display_labels = display_labels
+            self._internal.options = statushistory.Options()
+        assert isinstance(self._internal.options, statushistory.Options)
+        self._internal.options.show_value = show_value
     
         return self
     
-    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
+    def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = piechart.Options()
-        assert isinstance(self._internal.options, piechart.Options)
-        tooltip_resource = tooltip.build()
-        self._internal.options.tooltip = tooltip_resource
+            self._internal.options = statushistory.Options()
+        assert isinstance(self._internal.options, statushistory.Options)
+        legend_resource = legend.build()
+        self._internal.options.legend = legend_resource
     
         return self
     
-    def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
+    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = piechart.Options()
-        assert isinstance(self._internal.options, piechart.Options)
-        reduce_options_resource = reduce_options.build()
-        self._internal.options.reduce_options = reduce_options_resource
+            self._internal.options = statushistory.Options()
+        assert isinstance(self._internal.options, statushistory.Options)
+        tooltip_resource = tooltip.build()
+        self._internal.options.tooltip = tooltip_resource
     
         return self
     
-    def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
+    def timezone(self, timezone: list[common.TimeZone]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = piechart.Options()
-        assert isinstance(self._internal.options, piechart.Options)
-        text_resource = text.build()
-        self._internal.options.text = text_resource
+            self._internal.options = statushistory.Options()
+        assert isinstance(self._internal.options, statushistory.Options)
+        self._internal.options.timezone = timezone
     
         return self
     
-    def legend(self, legend: piechart.PieChartLegendOptions) -> typing.Self:        
+    def col_width(self, col_width: float) -> typing.Self:    
+        """
+        Controls the column width
+        """
+            
+        if not col_width <= 1:
+            raise ValueError("col_width must be <= 1")
         if self._internal.options is None:
-            self._internal.options = piechart.Options()
-        assert isinstance(self._internal.options, piechart.Options)
-        self._internal.options.legend = legend
+            self._internal.options = statushistory.Options()
+        assert isinstance(self._internal.options, statushistory.Options)
+        self._internal.options.col_width = col_width
     
         return self
     
-    def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = piechart.Options()
-        assert isinstance(self._internal.options, piechart.Options)
-        self._internal.options.orientation = orientation
+    def line_width(self, line_width: int) -> typing.Self:        
+        if not line_width <= 10:
+            raise ValueError("line_width must be <= 10")
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
+        self._internal.field_config.defaults.custom.line_width = line_width
     
         return self
     
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = piechart.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, piechart.FieldConfig)
+            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
         hide_from_resource = hide_from.build()
         self._internal.field_config.defaults.custom.hide_from = hide_from_resource
     
         return self
+    
+    def fill_opacity(self, fill_opacity: int) -> typing.Self:        
+        if not fill_opacity <= 100:
+            raise ValueError("fill_opacity must be <= 100")
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
+        self._internal.field_config.defaults.custom.fill_opacity = fill_opacity
+    
+        return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/preferences.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/preferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import preferences
 
 
 class Preferences(cogbuilder.Builder[preferences.Preferences]):    
-    """
-    Spec defines user, team or org Grafana preferences
-    swagger:model Preferences
-    """
-    
     _internal: preferences.Preferences
 
     def __init__(self):
         self._internal = preferences.Preferences()
 
     def build(self) -> preferences.Preferences:
         return self._internal
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/prometheus.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/prometheus.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,15 +96,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/publicdashboard.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/role.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/rolebinding.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/stat.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/stat.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -478,30 +441,14 @@
         if self._internal.options is None:
             self._internal.options = stat.Options()
         assert isinstance(self._internal.options, stat.Options)
         self._internal.options.justify_mode = justify_mode
     
         return self
     
-    def text_mode(self, text_mode: common.BigValueTextMode) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = stat.Options()
-        assert isinstance(self._internal.options, stat.Options)
-        self._internal.options.text_mode = text_mode
-    
-        return self
-    
-    def wide_layout(self, wide_layout: bool) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = stat.Options()
-        assert isinstance(self._internal.options, stat.Options)
-        self._internal.options.wide_layout = wide_layout
-    
-        return self
-    
     def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
         if self._internal.options is None:
             self._internal.options = stat.Options()
         assert isinstance(self._internal.options, stat.Options)
         reduce_options_resource = reduce_options.build()
         self._internal.options.reduce_options = reduce_options_resource
     
@@ -512,19 +459,19 @@
             self._internal.options = stat.Options()
         assert isinstance(self._internal.options, stat.Options)
         text_resource = text.build()
         self._internal.options.text = text_resource
     
         return self
     
-    def show_percent_change(self, show_percent_change: bool) -> typing.Self:        
+    def text_mode(self, text_mode: common.BigValueTextMode) -> typing.Self:        
         if self._internal.options is None:
             self._internal.options = stat.Options()
         assert isinstance(self._internal.options, stat.Options)
-        self._internal.options.show_percent_change = show_percent_change
+        self._internal.options.text_mode = text_mode
     
         return self
     
     def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
         if self._internal.options is None:
             self._internal.options = stat.Options()
         assert isinstance(self._internal.options, stat.Options)
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/statetimeline.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/debug.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import common
-from ..models import statetimeline
+from ..models import debug
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "state-timeline"
+        self._internal.type_val = "debug"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,24 +153,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +227,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -454,130 +416,23 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def show_value(self, show_value: common.VisibilityMode) -> typing.Self:    
-        """
-        Show timeline values on chart
-        """
-            
+    def mode(self, mode: debug.DebugMode) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
-        assert isinstance(self._internal.options, statetimeline.Options)
-        self._internal.options.show_value = show_value
+            self._internal.options = debug.Options()
+        assert isinstance(self._internal.options, debug.Options)
+        self._internal.options.mode = mode
     
         return self
     
-    def row_height(self, row_height: float) -> typing.Self:    
-        """
-        Controls the row height
-        """
-            
-        if not row_height <= 1:
-            raise ValueError("row_height must be <= 1")
+    def counters(self, counters: debug.UpdateConfig) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
-        assert isinstance(self._internal.options, statetimeline.Options)
-        self._internal.options.row_height = row_height
-    
-        return self
-    
-    def merge_values(self, merge_values: bool) -> typing.Self:    
-        """
-        Merge equal consecutive values
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
-        assert isinstance(self._internal.options, statetimeline.Options)
-        self._internal.options.merge_values = merge_values
-    
-        return self
-    
-    def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
-        assert isinstance(self._internal.options, statetimeline.Options)
-        legend_resource = legend.build()
-        self._internal.options.legend = legend_resource
-    
-        return self
-    
-    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
-        assert isinstance(self._internal.options, statetimeline.Options)
-        tooltip_resource = tooltip.build()
-        self._internal.options.tooltip = tooltip_resource
-    
-        return self
-    
-    def timezone(self, timezone: list[common.TimeZone]) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
-        assert isinstance(self._internal.options, statetimeline.Options)
-        self._internal.options.timezone = timezone
-    
-        return self
-    
-    def align_value(self, align_value: common.TimelineValueAlignment) -> typing.Self:    
-        """
-        Controls value alignment on the timelines
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = statetimeline.Options()
-        assert isinstance(self._internal.options, statetimeline.Options)
-        self._internal.options.align_value = align_value
-    
-        return self
-    
-    def line_width(self, line_width: int) -> typing.Self:        
-        if not line_width <= 10:
-            raise ValueError("line_width must be <= 10")
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
-        self._internal.field_config.defaults.custom.line_width = line_width
-    
-        return self
-    
-    def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
-        hide_from_resource = hide_from.build()
-        self._internal.field_config.defaults.custom.hide_from = hide_from_resource
-    
-        return self
-    
-    def fill_opacity(self, fill_opacity: int) -> typing.Self:        
-        if not fill_opacity <= 100:
-            raise ValueError("fill_opacity must be <= 100")
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statetimeline.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, statetimeline.FieldConfig)
-        self._internal.field_config.defaults.custom.fill_opacity = fill_opacity
+            self._internal.options = debug.Options()
+        assert isinstance(self._internal.options, debug.Options)
+        self._internal.options.counters = counters
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/statushistory.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/text.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import statushistory
-from ..models import common
+from ..models import text
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "status-history"
+        self._internal.type_val = "text"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,24 +153,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +227,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -454,122 +416,31 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def row_height(self, row_height: float) -> typing.Self:    
-        """
-        Set the height of the rows
-        """
-            
-        if not row_height >= 0:
-            raise ValueError("row_height must be >= 0")
-        if not row_height <= 1:
-            raise ValueError("row_height must be <= 1")
-        if self._internal.options is None:
-            self._internal.options = statushistory.Options()
-        assert isinstance(self._internal.options, statushistory.Options)
-        self._internal.options.row_height = row_height
-    
-        return self
-    
-    def show_value(self, show_value: common.VisibilityMode) -> typing.Self:    
-        """
-        Show values on the columns
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = statushistory.Options()
-        assert isinstance(self._internal.options, statushistory.Options)
-        self._internal.options.show_value = show_value
-    
-        return self
-    
-    def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
+    def mode(self, mode: text.TextMode) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = statushistory.Options()
-        assert isinstance(self._internal.options, statushistory.Options)
-        legend_resource = legend.build()
-        self._internal.options.legend = legend_resource
+            self._internal.options = text.Options()
+        assert isinstance(self._internal.options, text.Options)
+        self._internal.options.mode = mode
     
         return self
     
-    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
+    def code(self, code: text.CodeOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = statushistory.Options()
-        assert isinstance(self._internal.options, statushistory.Options)
-        tooltip_resource = tooltip.build()
-        self._internal.options.tooltip = tooltip_resource
+            self._internal.options = text.Options()
+        assert isinstance(self._internal.options, text.Options)
+        self._internal.options.code = code
     
         return self
     
-    def timezone(self, timezone: list[common.TimeZone]) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = statushistory.Options()
-        assert isinstance(self._internal.options, statushistory.Options)
-        self._internal.options.timezone = timezone
-    
-        return self
-    
-    def col_width(self, col_width: float) -> typing.Self:    
-        """
-        Controls the column width
-        """
-            
-        if not col_width <= 1:
-            raise ValueError("col_width must be <= 1")
+    def content(self, content: str) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = statushistory.Options()
-        assert isinstance(self._internal.options, statushistory.Options)
-        self._internal.options.col_width = col_width
-    
-        return self
-    
-    def line_width(self, line_width: int) -> typing.Self:        
-        if not line_width <= 10:
-            raise ValueError("line_width must be <= 10")
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
-        self._internal.field_config.defaults.custom.line_width = line_width
-    
-        return self
-    
-    def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
-        hide_from_resource = hide_from.build()
-        self._internal.field_config.defaults.custom.hide_from = hide_from_resource
-    
-        return self
-    
-    def fill_opacity(self, fill_opacity: int) -> typing.Self:        
-        if not fill_opacity <= 100:
-            raise ValueError("fill_opacity must be <= 100")
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = statushistory.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, statushistory.FieldConfig)
-        self._internal.field_config.defaults.custom.fill_opacity = fill_opacity
+            self._internal.options = text.Options()
+        assert isinstance(self._internal.options, text.Options)
+        self._internal.options.content = content
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/table.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/xychart.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import table
+from ..models import xychart
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "table"
+        self._internal.type_val = "xychart"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -454,219 +417,310 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def frame_index(self, frame_index: float) -> typing.Self:    
-        """
-        Represents the index of the selected frame
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        self._internal.options.frame_index = frame_index
+    def show(self, show: xychart.ScatterShow) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.show = show
     
         return self
     
-    def show_header(self, show_header: bool) -> typing.Self:    
-        """
-        Controls whether the panel should show the header
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        self._internal.options.show_header = show_header
+    def point_size(self, point_size: cogbuilder.Builder[common.ScaleDimensionConfig]) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        point_size_resource = point_size.build()
+        self._internal.field_config.defaults.custom.point_size = point_size_resource
     
         return self
     
-    def show_type_icons(self, show_type_icons: bool) -> typing.Self:    
-        """
-        Controls whether the header should show icons for the column types
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        self._internal.options.show_type_icons = show_type_icons
+    def point_color(self, point_color: cogbuilder.Builder[common.ColorDimensionConfig]) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        point_color_resource = point_color.build()
+        self._internal.field_config.defaults.custom.point_color = point_color_resource
     
         return self
     
-    def sort_by(self, sort_by: list[cogbuilder.Builder[common.TableSortByFieldState]]) -> typing.Self:    
-        """
-        Used to control row sorting
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        sort_by_resources = [r1.build() for r1 in sort_by]
-        self._internal.options.sort_by = sort_by_resources
+    def line_color(self, line_color: cogbuilder.Builder[common.ColorDimensionConfig]) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        line_color_resource = line_color.build()
+        self._internal.field_config.defaults.custom.line_color = line_color_resource
     
         return self
     
-    def footer(self, footer: cogbuilder.Builder[common.TableFooterOptions]) -> typing.Self:    
-        """
-        Controls footer options
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        footer_resource = footer.build()
-        self._internal.options.footer = footer_resource
+    def line_width(self, line_width: int) -> typing.Self:        
+        if not line_width >= 0:
+            raise ValueError("line_width must be >= 0")
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.line_width = line_width
     
         return self
     
-    def cell_height(self, cell_height: common.TableCellHeight) -> typing.Self:    
-        """
-        Controls the height of the rows
-        """
-            
-        if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        self._internal.options.cell_height = cell_height
+    def line_style(self, line_style: cogbuilder.Builder[common.LineStyle]) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        line_style_resource = line_style.build()
+        self._internal.field_config.defaults.custom.line_style = line_style_resource
     
         return self
     
-    def width(self, width: float) -> typing.Self:        
+    def label(self, label: common.VisibilityMode) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = table.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, table.FieldConfig)
-        self._internal.field_config.defaults.custom.width = width
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.label = label
     
         return self
     
-    def min_width(self, min_width: float) -> typing.Self:        
+    def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = table.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, table.FieldConfig)
-        self._internal.field_config.defaults.custom.min_width = min_width
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        hide_from_resource = hide_from.build()
+        self._internal.field_config.defaults.custom.hide_from = hide_from_resource
     
         return self
     
-    def align(self, align: common.FieldTextAlignment) -> typing.Self:        
+    def axis_placement(self, axis_placement: common.AxisPlacement) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = table.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, table.FieldConfig)
-        self._internal.field_config.defaults.custom.align = align
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_placement = axis_placement
     
         return self
     
-    def display_mode(self, display_mode: common.TableCellDisplayMode) -> typing.Self:    
-        """
-        This field is deprecated in favor of using cellOptions
-        """
-            
+    def axis_color_mode(self, axis_color_mode: common.AxisColorMode) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = table.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, table.FieldConfig)
-        self._internal.field_config.defaults.custom.display_mode = display_mode
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_color_mode = axis_color_mode
     
         return self
     
-    def cell_options(self, cell_options: common.TableCellOptions) -> typing.Self:        
+    def axis_label(self, axis_label: str) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = table.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, table.FieldConfig)
-        self._internal.field_config.defaults.custom.cell_options = cell_options
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_label = axis_label
     
         return self
     
-    def hidden(self, hidden: bool) -> typing.Self:    
-        """
-        ?? default is missing or false ??
-        """
-            
+    def axis_width(self, axis_width: float) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = table.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, table.FieldConfig)
-        self._internal.field_config.defaults.custom.hidden = hidden
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_width = axis_width
     
         return self
     
-    def inspect(self, inspect: bool) -> typing.Self:        
+    def axis_soft_min(self, axis_soft_min: float) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = table.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, table.FieldConfig)
-        self._internal.field_config.defaults.custom.inspect = inspect
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_soft_min = axis_soft_min
     
         return self
     
-    def filterable(self, filterable: bool) -> typing.Self:        
+    def axis_soft_max(self, axis_soft_max: float) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = table.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, table.FieldConfig)
-        self._internal.field_config.defaults.custom.filterable = filterable
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_soft_max = axis_soft_max
     
         return self
     
-    def hide_header(self, hide_header: bool) -> typing.Self:    
-        """
-        Hides any header for a column, useful for columns that show some static content or buttons.
-        """
-            
+    def axis_grid_show(self, axis_grid_show: bool) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_grid_show = axis_grid_show
+    
+        return self
+    
+    def scale_distribution(self, scale_distribution: cogbuilder.Builder[common.ScaleDistributionConfig]) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        scale_distribution_resource = scale_distribution.build()
+        self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
+    
+        return self
+    
+    def label_value(self, label_value: cogbuilder.Builder[common.TextDimensionConfig]) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = table.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, table.FieldConfig)
-        self._internal.field_config.defaults.custom.hide_header = hide_header
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        label_value_resource = label_value.build()
+        self._internal.field_config.defaults.custom.label_value = label_value_resource
+    
+        return self
+    
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+    
+        return self
+    
+    def series_mapping(self, series_mapping: xychart.SeriesMapping) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = xychart.Options()
+        assert isinstance(self._internal.options, xychart.Options)
+        self._internal.options.series_mapping = series_mapping
+    
+        return self
+    
+    def dims(self, dims: xychart.XYDimensionConfig) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = xychart.Options()
+        assert isinstance(self._internal.options, xychart.Options)
+        self._internal.options.dims = dims
+    
+        return self
+    
+    def legend(self, legend: cogbuilder.Builder[common.VizLegendOptions]) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = xychart.Options()
+        assert isinstance(self._internal.options, xychart.Options)
+        legend_resource = legend.build()
+        self._internal.options.legend = legend_resource
+    
+        return self
+    
+    def tooltip(self, tooltip: cogbuilder.Builder[common.VizTooltipOptions]) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = xychart.Options()
+        assert isinstance(self._internal.options, xychart.Options)
+        tooltip_resource = tooltip.build()
+        self._internal.options.tooltip = tooltip_resource
+    
+        return self
+    
+    def series(self, series: list[xychart.ScatterSeriesConfig]) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = xychart.Options()
+        assert isinstance(self._internal.options, xychart.Options)
+        self._internal.options.series = series
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/team.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/tempo.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/tempo.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,17 @@
             
         self._internal.ref_id = ref_id
     
         return self
     
     def hide(self, hide: bool) -> typing.Self:    
         """
-        If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+        true if query is disabled (ie should not be returned to the dashboard)
+        Note this does not always imply that the query should not be executed since
+        the results from a hidden query may be used as the input to other queries (SSE etc)
         """
             
         self._internal.hide = hide
     
         return self
     
     def query_type(self, query_type: str) -> typing.Self:    
@@ -94,17 +96,17 @@
         @deprecated Define the maximum duration to select traces. Use duration format, for example: 1.2s, 100ms
         """
             
         self._internal.max_duration = max_duration
     
         return self
     
-    def service_map_query(self, service_map_query: typing.Union[str, list[str]]) -> typing.Self:    
+    def service_map_query(self, service_map_query: str) -> typing.Self:    
         """
-        Filters to be included in a PromQL query to select data for the service graph. Example: {client="app",service="app"}. Providing multiple values will produce union of results for each filter, using PromQL OR operator internally.
+        Filters to be included in a PromQL query to select data for the service graph. Example: {client="app",service="app"}
         """
             
         self._internal.service_map_query = service_map_query
     
         return self
     
     def service_map_include_namespace(self, service_map_include_namespace: bool) -> typing.Self:    
@@ -121,57 +123,29 @@
         Defines the maximum number of traces that are returned from Tempo
         """
             
         self._internal.limit = limit
     
         return self
     
-    def spss(self, spss: int) -> typing.Self:    
-        """
-        Defines the maximum number of spans per spanset that are returned from Tempo
-        """
-            
-        self._internal.spss = spss
-    
-        return self
-    
-    def filters(self, filters: list[cogbuilder.Builder[tempo.TraceqlFilter]]) -> typing.Self:        
-        filters_resources = [r1.build() for r1 in filters]
-        self._internal.filters = filters_resources
-    
-        return self
-    
-    def group_by(self, group_by: list[cogbuilder.Builder[tempo.TraceqlFilter]]) -> typing.Self:    
-        """
-        Filters that are used to query the metrics summary
-        """
-            
-        group_by_resources = [r1.build() for r1 in group_by]
-        self._internal.group_by = group_by_resources
-    
-        return self
-    
     def datasource(self, datasource: object) -> typing.Self:    
         """
         For mixed data sources the selected datasource is on the query level.
         For non mixed scenarios this is undefined.
         TODO find a better way to do this ^ that's friendly to schema
         TODO this shouldn't be unknown but DataSourceRef | null
         """
             
         self._internal.datasource = datasource
     
         return self
     
-    def table_type(self, table_type: tempo.SearchTableType) -> typing.Self:    
-        """
-        The type of the table that is used to display the search results
-        """
-            
-        self._internal.table_type = table_type
+    def filters(self, filters: list[cogbuilder.Builder[tempo.TraceqlFilter]]) -> typing.Self:        
+        filters_resources = [r1.build() for r1 in filters]
+        self._internal.filters = filters_resources
     
         return self
     
 
 class TraceqlFilter(cogbuilder.Builder[tempo.TraceqlFilter]):    
     _internal: tempo.TraceqlFilter
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/text.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/canvas.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import text
+from ..models import canvas
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "text"
+        self._internal.type_val = "canvas"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -153,24 +153,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -237,50 +227,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -453,31 +416,44 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def mode(self, mode: text.TextMode) -> typing.Self:        
+    def inline_editing(self, inline_editing: bool) -> typing.Self:    
+        """
+        Enable inline editing
+        """
+            
         if self._internal.options is None:
-            self._internal.options = text.Options()
-        assert isinstance(self._internal.options, text.Options)
-        self._internal.options.mode = mode
+            self._internal.options = canvas.Options()
+        assert isinstance(self._internal.options, canvas.Options)
+        self._internal.options.inline_editing = inline_editing
     
         return self
     
-    def code(self, code: text.CodeOptions) -> typing.Self:        
+    def show_advanced_types(self, show_advanced_types: bool) -> typing.Self:    
+        """
+        Show all available element types
+        """
+            
         if self._internal.options is None:
-            self._internal.options = text.Options()
-        assert isinstance(self._internal.options, text.Options)
-        self._internal.options.code = code
+            self._internal.options = canvas.Options()
+        assert isinstance(self._internal.options, canvas.Options)
+        self._internal.options.show_advanced_types = show_advanced_types
     
         return self
     
-    def content(self, content: str) -> typing.Self:        
+    def root(self, root: canvas.CanvasOptionsRoot) -> typing.Self:    
+        """
+        The root element of canvas (frame), where all canvas elements are nested
+        TODO: Figure out how to define a default value for this
+        """
+            
         if self._internal.options is None:
-            self._internal.options = text.Options()
-        assert isinstance(self._internal.options, text.Options)
-        self._internal.options.content = content
+            self._internal.options = canvas.Options()
+        assert isinstance(self._internal.options, canvas.Options)
+        self._internal.options.root = root
     
         return self
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/timeseries.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -480,22 +443,14 @@
             self._internal.options = timeseries.Options()
         assert isinstance(self._internal.options, timeseries.Options)
         tooltip_resource = tooltip.build()
         self._internal.options.tooltip = tooltip_resource
     
         return self
     
-    def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = timeseries.Options()
-        assert isinstance(self._internal.options, timeseries.Options)
-        self._internal.options.orientation = orientation
-    
-        return self
-    
     def draw_style(self, draw_style: common.GraphDrawStyle) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -771,28 +726,14 @@
             self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
-    
-        return self
-    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -905,25 +846,25 @@
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         self._internal.field_config.defaults.custom.point_symbol = point_symbol
     
         return self
     
-    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/builders/trend.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/builders/trend.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,24 +154,14 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def max_per_row(self, max_per_row: float) -> typing.Self:    
-        """
-        Option for repeated panels that controls max items per row
-        Only relevant for horizontally repeated panels
-        """
-            
-        self._internal.max_per_row = max_per_row
-    
-        return self
-    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -238,50 +228,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
-    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
-        """
-        Controls if the timeFrom or timeShift overrides are shown in the panel header
-        """
-            
-        self._internal.hide_time_override = hide_time_override
-    
-        return self
-    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
         return self
     
-    def cache_timeout(self, cache_timeout: str) -> typing.Self:    
-        """
-        Sets panel queries cache timeout.
-        """
-            
-        self._internal.cache_timeout = cache_timeout
-    
-        return self
-    
-    def query_caching_ttl(self, query_caching_ttl: float) -> typing.Self:    
-        """
-        Overrides the data source configured time-to-live for a query cache item in milliseconds
-        """
-            
-        self._internal.query_caching_ttl = query_caching_ttl
-    
-        return self
-    
     def display_name(self, display_name: str) -> typing.Self:    
         """
         The display value for this field.  This supports template variables blank is auto
         """
             
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
@@ -767,28 +730,14 @@
             self._internal.field_config.defaults.custom = trend.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
-        if self._internal.field_config is None:
-            self._internal.field_config = dashboard.FieldConfigSource()
-        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
-        if self._internal.field_config.defaults is None:
-            self._internal.field_config.defaults = dashboard.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
-        if self._internal.field_config.defaults.custom is None:
-            self._internal.field_config.defaults.custom = trend.FieldConfig()
-        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
-    
-        return self
-    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -901,25 +850,25 @@
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = trend.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         self._internal.field_config.defaults.custom.point_symbol = point_symbol
     
         return self
     
-    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = trend.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/cog/plugins.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/cog/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-from ..models import canvas
-from ..models import dashboardlist
-from ..models import elasticsearch
-from ..models import heatmap
+from ..models import alertgroups
+from ..models import tempo
+from ..models import debug
+from ..models import grafanapyroscope
 from ..models import news
+from ..models import nodegraph
+from ..models import canvas
+from ..models import azuremonitor
+from ..models import candlestick
+from ..models import parca
+from ..models import trend
 from ..models import prometheus
-from ..models import statushistory
+from ..models import statetimeline
 from ..models import bargauge
 from ..models import datagrid
-from ..models import gauge
+from ..models import googlecloudmonitoring
 from ..models import logs
-from ..models import nodegraph
-from ..models import expr
-from ..models import stat
-from ..models import tempo
-from ..models import candlestick
-from ..models import cloudwatch
+from ..models import annotationslist
+from ..models import gauge
 from ..models import geomap
 from ..models import piechart
-from ..models import trend
-from ..models import barchart
+from ..models import elasticsearch
+from ..models import heatmap
 from ..models import histogram
-from ..models import annotationslist
-from ..models import azuremonitor
-from ..models import googlecloudmonitoring
-from ..models import parca
-from ..models import statetimeline
-from ..models import timeseries
-from ..models import grafanapyroscope
-from ..models import loki
+from ..models import table
+from ..models import cloudwatch
+from ..models import dashboardlist
 from ..models import text
+from ..models import timeseries
 from ..models import xychart
-from ..models import debug
-from ..models import table
+from ..models import expr
+from ..models import loki
+from ..models import stat
+from ..models import statushistory
+from ..models import barchart
+from ..models import testdata
 from . import runtime as cogruntime
 
 
 def register_default_plugins():
     # Panelcfg variants
+    cogruntime.register_panelcfg_variant(alertgroups.variant_config())
     cogruntime.register_panelcfg_variant(annotationslist.variant_config())
     cogruntime.register_panelcfg_variant(barchart.variant_config())
     cogruntime.register_panelcfg_variant(bargauge.variant_config())
     cogruntime.register_panelcfg_variant(candlestick.variant_config())
     cogruntime.register_panelcfg_variant(canvas.variant_config())
     cogruntime.register_panelcfg_variant(dashboardlist.variant_config())
     cogruntime.register_panelcfg_variant(datagrid.variant_config())
@@ -71,7 +74,8 @@
     cogruntime.register_dataquery_variant(expr.variant_config())
     cogruntime.register_dataquery_variant(googlecloudmonitoring.variant_config())
     cogruntime.register_dataquery_variant(grafanapyroscope.variant_config())
     cogruntime.register_dataquery_variant(loki.variant_config())
     cogruntime.register_dataquery_variant(parca.variant_config())
     cogruntime.register_dataquery_variant(prometheus.variant_config())
     cogruntime.register_dataquery_variant(tempo.variant_config())
+    cogruntime.register_dataquery_variant(testdata.variant_config())
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/cog/runtime.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/cog/runtime.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/accesspolicy.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/alerting.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/alerting.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Duration in seconds.
 Duration: typing.TypeAlias = int
 
 
 Json: typing.TypeAlias = object
 
 
-MatchRegexps: typing.TypeAlias = dict[str, str]
+MatchRegexps: typing.TypeAlias = dict[str, 'Regexp']
 
 
 MatchType: typing.TypeAlias = int
 
 
 class Matcher:
     name: typing.Optional[str]
@@ -90,21 +90,26 @@
             args["provenance"] = data["provenance"]
         if "template" in data:
             args["template"] = data["template"]        
 
         return cls(**args)
 
 
-ObjectMatcher: typing.TypeAlias = list[str]
+# Matchers is a slice of Matchers that is sortable, implements Stringer, and
+# provides a Matches method to match a LabelSet against all Matchers in the
+# slice. Note that some users of Matchers might require it to be sorted.
+ObjectMatchers: typing.TypeAlias = 'Matchers'
 
 
-ObjectMatchers: typing.TypeAlias = list['ObjectMatcher']
+Provenance: typing.TypeAlias = str
 
 
-Provenance: typing.TypeAlias = str
+# A Regexp is safe for concurrent use by multiple goroutines,
+# except for configuration methods, such as Longest.
+Regexp: typing.TypeAlias = object
 
 
 class RelativeTimeRange:
     """
     RelativeTimeRange is the per query start and end time
     for requests.
     """
@@ -138,38 +143,114 @@
         if "to" in data:
             args["to"] = data["to"]        
 
         return cls(**args)
 
 
 class TimeInterval:
-    name: typing.Optional[str]
-    time_intervals: typing.Optional[list['TimeInterval']]
+    """
+    TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    within the interval.
+    """
 
-    def __init__(self, name: typing.Optional[str] = None, time_intervals: typing.Optional[list['TimeInterval']] = None):
-        self.name = name
-        self.time_intervals = time_intervals
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    days_of_month: typing.Optional[list[str]]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    location: typing.Optional[str]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    months: typing.Optional[list[str]]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    times: typing.Optional[list['TimeRange']]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    weekdays: typing.Optional[list[str]]
+    # TimeInterval describes intervals of time. ContainsTime will tell you if a golang time is contained
+    # within the interval.
+    years: typing.Optional[list[str]]
+
+    def __init__(self, days_of_month: typing.Optional[list[str]] = None, location: typing.Optional[str] = None, months: typing.Optional[list[str]] = None, times: typing.Optional[list['TimeRange']] = None, weekdays: typing.Optional[list[str]] = None, years: typing.Optional[list[str]] = None):
+        self.days_of_month = days_of_month
+        self.location = location
+        self.months = months
+        self.times = times
+        self.weekdays = weekdays
+        self.years = years
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
-        if self.name is not None:
-            payload["name"] = self.name
-        if self.time_intervals is not None:
-            payload["time_intervals"] = self.time_intervals
+        if self.days_of_month is not None:
+            payload["days_of_month"] = self.days_of_month
+        if self.location is not None:
+            payload["location"] = self.location
+        if self.months is not None:
+            payload["months"] = self.months
+        if self.times is not None:
+            payload["times"] = self.times
+        if self.weekdays is not None:
+            payload["weekdays"] = self.weekdays
+        if self.years is not None:
+            payload["years"] = self.years
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "name" in data:
-            args["name"] = data["name"]
-        if "time_intervals" in data:
-            args["time_intervals"] = data["time_intervals"]        
+        if "days_of_month" in data:
+            args["days_of_month"] = data["days_of_month"]
+        if "location" in data:
+            args["location"] = data["location"]
+        if "months" in data:
+            args["months"] = data["months"]
+        if "times" in data:
+            args["times"] = data["times"]
+        if "weekdays" in data:
+            args["weekdays"] = data["weekdays"]
+        if "years" in data:
+            args["years"] = data["years"]        
+
+        return cls(**args)
+
+
+class TimeRange:
+    """
+    Redefining this to avoid an import cycle
+    """
+
+    # Redefining this to avoid an import cycle
+    from_val: typing.Optional[str]
+    # Redefining this to avoid an import cycle
+    to: typing.Optional[str]
+
+    def __init__(self, from_val: typing.Optional[str] = None, to: typing.Optional[str] = None):
+        self.from_val = from_val
+        self.to = to
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+        }
+        if self.from_val is not None:
+            payload["from"] = self.from_val
+        if self.to is not None:
+            payload["to"] = self.to
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "from" in data:
+            args["from_val"] = data["from"]
+        if "to" in data:
+            args["to"] = data["to"]        
 
         return cls(**args)
 
 
 class RuleGroup:
     folder_uid: typing.Optional[str]
     # The interval, in seconds, at which all rules in the group are evaluated.
@@ -222,34 +303,32 @@
     # The amount of time, in seconds, for which the rule must be breached for the rule to be considered to be Firing.
     # Before this time has elapsed, the rule is only considered to be Pending.
     for_val: str
     id_val: typing.Optional[int]
     is_paused: typing.Optional[bool]
     labels: typing.Optional[dict[str, str]]
     no_data_state: typing.Literal["Alerting", "NoData", "OK"]
-    notification_settings: typing.Optional['NotificationSettings']
     org_id: int
     provenance: typing.Optional['Provenance']
     rule_group: str
     title: str
     uid: typing.Optional[str]
     updated: typing.Optional[str]
 
-    def __init__(self, annotations: typing.Optional[dict[str, str]] = None, condition: str = "", data: typing.Optional[list['Query']] = None, exec_err_state: typing.Optional[typing.Literal["OK", "Alerting", "Error"]] = None, folder_uid: str = "", for_val: str = "", id_val: typing.Optional[int] = None, is_paused: typing.Optional[bool] = None, labels: typing.Optional[dict[str, str]] = None, no_data_state: typing.Optional[typing.Literal["Alerting", "NoData", "OK"]] = None, notification_settings: typing.Optional['NotificationSettings'] = None, org_id: int = 0, provenance: typing.Optional['Provenance'] = None, rule_group: str = "", title: str = "", uid: typing.Optional[str] = None, updated: typing.Optional[str] = None):
+    def __init__(self, annotations: typing.Optional[dict[str, str]] = None, condition: str = "", data: typing.Optional[list['Query']] = None, exec_err_state: typing.Optional[typing.Literal["OK", "Alerting", "Error"]] = None, folder_uid: str = "", for_val: str = "", id_val: typing.Optional[int] = None, is_paused: typing.Optional[bool] = None, labels: typing.Optional[dict[str, str]] = None, no_data_state: typing.Optional[typing.Literal["Alerting", "NoData", "OK"]] = None, org_id: int = 0, provenance: typing.Optional['Provenance'] = None, rule_group: str = "", title: str = "", uid: typing.Optional[str] = None, updated: typing.Optional[str] = None):
         self.annotations = annotations
         self.condition = condition
         self.data = data if data is not None else []
         self.exec_err_state = exec_err_state if exec_err_state is not None else "OK"
         self.folder_uid = folder_uid
         self.for_val = for_val
         self.id_val = id_val
         self.is_paused = is_paused
         self.labels = labels
         self.no_data_state = no_data_state if no_data_state is not None else "Alerting"
-        self.notification_settings = notification_settings
         self.org_id = org_id
         self.provenance = provenance
         self.rule_group = rule_group
         self.title = title
         self.uid = uid
         self.updated = updated
 
@@ -269,16 +348,14 @@
             payload["annotations"] = self.annotations
         if self.id_val is not None:
             payload["id"] = self.id_val
         if self.is_paused is not None:
             payload["isPaused"] = self.is_paused
         if self.labels is not None:
             payload["labels"] = self.labels
-        if self.notification_settings is not None:
-            payload["notification_settings"] = self.notification_settings
         if self.provenance is not None:
             payload["provenance"] = self.provenance
         if self.uid is not None:
             payload["uid"] = self.uid
         if self.updated is not None:
             payload["updated"] = self.updated
         return payload
@@ -303,16 +380,14 @@
             args["id_val"] = data["id"]
         if "isPaused" in data:
             args["is_paused"] = data["isPaused"]
         if "labels" in data:
             args["labels"] = data["labels"]
         if "noDataState" in data:
             args["no_data_state"] = data["noDataState"]
-        if "notification_settings" in data:
-            args["notification_settings"] = NotificationSettings.from_json(data["notification_settings"])
         if "orgID" in data:
             args["org_id"] = data["orgID"]
         if "provenance" in data:
             args["provenance"] = data["provenance"]
         if "ruleGroup" in data:
             args["rule_group"] = data["ruleGroup"]
         if "title" in data:
@@ -321,66 +396,14 @@
             args["uid"] = data["uid"]
         if "updated" in data:
             args["updated"] = data["updated"]        
 
         return cls(**args)
 
 
-class NotificationSettings:
-    group_by: typing.Optional[list[str]]
-    group_interval: typing.Optional[str]
-    group_wait: typing.Optional[str]
-    mute_time_intervals: typing.Optional[list[str]]
-    receiver: str
-    repeat_interval: typing.Optional[str]
-
-    def __init__(self, group_by: typing.Optional[list[str]] = None, group_interval: typing.Optional[str] = None, group_wait: typing.Optional[str] = None, mute_time_intervals: typing.Optional[list[str]] = None, receiver: str = "", repeat_interval: typing.Optional[str] = None):
-        self.group_by = group_by if group_by is not None else ["alertname", "grafana_folder"]
-        self.group_interval = group_interval
-        self.group_wait = group_wait
-        self.mute_time_intervals = mute_time_intervals
-        self.receiver = receiver
-        self.repeat_interval = repeat_interval
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "receiver": self.receiver,
-        }
-        if self.group_by is not None:
-            payload["group_by"] = self.group_by
-        if self.group_interval is not None:
-            payload["group_interval"] = self.group_interval
-        if self.group_wait is not None:
-            payload["group_wait"] = self.group_wait
-        if self.mute_time_intervals is not None:
-            payload["mute_time_intervals"] = self.mute_time_intervals
-        if self.repeat_interval is not None:
-            payload["repeat_interval"] = self.repeat_interval
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "group_by" in data:
-            args["group_by"] = data["group_by"]
-        if "group_interval" in data:
-            args["group_interval"] = data["group_interval"]
-        if "group_wait" in data:
-            args["group_wait"] = data["group_wait"]
-        if "mute_time_intervals" in data:
-            args["mute_time_intervals"] = data["mute_time_intervals"]
-        if "receiver" in data:
-            args["receiver"] = data["receiver"]
-        if "repeat_interval" in data:
-            args["repeat_interval"] = data["repeat_interval"]        
-
-        return cls(**args)
-
-
 class Query:
     datasource_uid: typing.Optional[str]
     model: typing.Optional[cogvariants.Dataquery]
     query_type: typing.Optional[str]
     ref_id: typing.Optional[str]
     relative_time_range: typing.Optional['RelativeTimeRange']
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/annotationslist.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/azuremonitor.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/azuremonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 
 class AzureMonitorQuery(cogvariants.Dataquery):
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # Azure subscription containing the resource(s) to be queried.
     subscription: typing.Optional[str]
     # Subscriptions to be queried via Azure Resource Graph.
@@ -310,76 +312,62 @@
 
     # KQL query to be executed.
     query: typing.Optional[str]
     # Specifies the format results should be returned as.
     result_format: typing.Optional['ResultFormat']
     # Array of resource URIs to be queried.
     resources: typing.Optional[list[str]]
-    # If set to true the dashboard time range will be used as a filter for the query. Otherwise the query time ranges will be used. Defaults to false.
-    dashboard_time: typing.Optional[bool]
-    # If dashboardTime is set to true this value dictates which column the time filter will be applied to. Defaults to the first tables timeSpan column, the first datetime column found, or TimeGenerated
-    time_column: typing.Optional[str]
-    # Workspace ID. This was removed in Grafana 8, but remains for backwards compat.
+    # If set to true the intersection of time ranges specified in the query and Grafana will be used. Otherwise the query time ranges will be used. Defaults to false
+    intersect_time: typing.Optional[bool]
+    # Workspace ID. This was removed in Grafana 8, but remains for backwards compat
     workspace: typing.Optional[str]
     # @deprecated Use resources instead
     resource: typing.Optional[str]
-    # @deprecated Use dashboardTime instead
-    intersect_time: typing.Optional[bool]
 
-    def __init__(self, query: typing.Optional[str] = None, result_format: typing.Optional['ResultFormat'] = None, resources: typing.Optional[list[str]] = None, dashboard_time: typing.Optional[bool] = None, time_column: typing.Optional[str] = None, workspace: typing.Optional[str] = None, resource: typing.Optional[str] = None, intersect_time: typing.Optional[bool] = None):
+    def __init__(self, query: typing.Optional[str] = None, result_format: typing.Optional['ResultFormat'] = None, resources: typing.Optional[list[str]] = None, intersect_time: typing.Optional[bool] = None, workspace: typing.Optional[str] = None, resource: typing.Optional[str] = None):
         self.query = query
         self.result_format = result_format
         self.resources = resources
-        self.dashboard_time = dashboard_time
-        self.time_column = time_column
+        self.intersect_time = intersect_time
         self.workspace = workspace
         self.resource = resource
-        self.intersect_time = intersect_time
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.query is not None:
             payload["query"] = self.query
         if self.result_format is not None:
             payload["resultFormat"] = self.result_format
         if self.resources is not None:
             payload["resources"] = self.resources
-        if self.dashboard_time is not None:
-            payload["dashboardTime"] = self.dashboard_time
-        if self.time_column is not None:
-            payload["timeColumn"] = self.time_column
+        if self.intersect_time is not None:
+            payload["intersectTime"] = self.intersect_time
         if self.workspace is not None:
             payload["workspace"] = self.workspace
         if self.resource is not None:
             payload["resource"] = self.resource
-        if self.intersect_time is not None:
-            payload["intersectTime"] = self.intersect_time
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "query" in data:
             args["query"] = data["query"]
         if "resultFormat" in data:
             args["result_format"] = data["resultFormat"]
         if "resources" in data:
             args["resources"] = data["resources"]
-        if "dashboardTime" in data:
-            args["dashboard_time"] = data["dashboardTime"]
-        if "timeColumn" in data:
-            args["time_column"] = data["timeColumn"]
+        if "intersectTime" in data:
+            args["intersect_time"] = data["intersectTime"]
         if "workspace" in data:
             args["workspace"] = data["workspace"]
         if "resource" in data:
-            args["resource"] = data["resource"]
-        if "intersectTime" in data:
-            args["intersect_time"] = data["intersectTime"]        
+            args["resource"] = data["resource"]        
 
         return cls(**args)
 
 
 class AzureTracesQuery:
     """
     Application Insights Traces sub-query properties
@@ -478,15 +466,14 @@
         return cls(**args)
 
 
 class ResultFormat(enum.StrEnum):
     TABLE = "table"
     TIME_SERIES = "time_series"
     TRACE = "trace"
-    LOGS = "logs"
 
 
 class AzureResourceGraphQuery:
     # Azure Resource Graph KQL query to be executed.
     query: typing.Optional[str]
     # Specifies the format results should be returned as. Defaults to table.
     result_format: typing.Optional[str]
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/barchart.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/barchart.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,36 +128,34 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
-    axis_centered_zero: typing.Optional[bool]
     hide_from: typing.Optional[common.HideSeriesConfig]
     # Threshold rendering
     thresholds_style: typing.Optional[common.GraphThresholdsStyleConfig]
-    axis_border_show: typing.Optional[bool]
+    axis_centered_zero: typing.Optional[bool]
 
-    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, thresholds_style: typing.Optional[common.GraphThresholdsStyleConfig] = None, axis_border_show: typing.Optional[bool] = None):
+    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, thresholds_style: typing.Optional[common.GraphThresholdsStyleConfig] = None, axis_centered_zero: typing.Optional[bool] = None):
         self.line_width = line_width
         self.fill_opacity = fill_opacity
         self.gradient_mode = gradient_mode if gradient_mode is not None else common.GraphGradientMode.NONE
         self.axis_placement = axis_placement
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
-        self.axis_centered_zero = axis_centered_zero
         self.hide_from = hide_from
         self.thresholds_style = thresholds_style
-        self.axis_border_show = axis_border_show
+        self.axis_centered_zero = axis_centered_zero
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.line_width is not None:
             payload["lineWidth"] = self.line_width
         if self.fill_opacity is not None:
@@ -176,22 +174,20 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.hide_from is not None:
             payload["hideFrom"] = self.hide_from
         if self.thresholds_style is not None:
             payload["thresholdsStyle"] = self.thresholds_style
-        if self.axis_border_show is not None:
-            payload["axisBorderShow"] = self.axis_border_show
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "lineWidth" in data:
@@ -212,22 +208,20 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "hideFrom" in data:
             args["hide_from"] = common.HideSeriesConfig.from_json(data["hideFrom"])
         if "thresholdsStyle" in data:
             args["thresholds_style"] = common.GraphThresholdsStyleConfig.from_json(data["thresholdsStyle"])
-        if "axisBorderShow" in data:
-            args["axis_border_show"] = data["axisBorderShow"]        
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/bargauge.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/bargauge.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,78 +4,63 @@
 import typing
 from ..cog import runtime as cogruntime
 
 
 class Options:
     display_mode: common.BarGaugeDisplayMode
     value_mode: common.BarGaugeValueMode
-    name_placement: common.BarGaugeNamePlacement
     show_unfilled: bool
-    sizing: common.BarGaugeSizing
     min_viz_width: int
-    min_viz_height: int
     reduce_options: common.ReduceDataOptions
     text: typing.Optional[common.VizTextDisplayOptions]
-    max_viz_height: int
+    min_viz_height: int
     orientation: common.VizOrientation
 
-    def __init__(self, display_mode: typing.Optional[common.BarGaugeDisplayMode] = None, value_mode: typing.Optional[common.BarGaugeValueMode] = None, name_placement: typing.Optional[common.BarGaugeNamePlacement] = None, show_unfilled: bool = True, sizing: typing.Optional[common.BarGaugeSizing] = None, min_viz_width: int = 8, min_viz_height: int = 16, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, max_viz_height: int = 300, orientation: typing.Optional[common.VizOrientation] = None):
+    def __init__(self, display_mode: typing.Optional[common.BarGaugeDisplayMode] = None, value_mode: typing.Optional[common.BarGaugeValueMode] = None, show_unfilled: bool = True, min_viz_width: int = 0, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, min_viz_height: int = 10, orientation: typing.Optional[common.VizOrientation] = None):
         self.display_mode = display_mode if display_mode is not None else common.BarGaugeDisplayMode.GRADIENT
         self.value_mode = value_mode if value_mode is not None else common.BarGaugeValueMode.COLOR
-        self.name_placement = name_placement if name_placement is not None else common.BarGaugeNamePlacement.AUTO
         self.show_unfilled = show_unfilled
-        self.sizing = sizing if sizing is not None else common.BarGaugeSizing.AUTO
         self.min_viz_width = min_viz_width
-        self.min_viz_height = min_viz_height
         self.reduce_options = reduce_options if reduce_options is not None else common.ReduceDataOptions()
         self.text = text
-        self.max_viz_height = max_viz_height
+        self.min_viz_height = min_viz_height
         self.orientation = orientation if orientation is not None else common.VizOrientation.AUTO
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "displayMode": self.display_mode,
             "valueMode": self.value_mode,
-            "namePlacement": self.name_placement,
             "showUnfilled": self.show_unfilled,
-            "sizing": self.sizing,
             "minVizWidth": self.min_viz_width,
-            "minVizHeight": self.min_viz_height,
             "reduceOptions": self.reduce_options,
-            "maxVizHeight": self.max_viz_height,
+            "minVizHeight": self.min_viz_height,
             "orientation": self.orientation,
         }
         if self.text is not None:
             payload["text"] = self.text
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "displayMode" in data:
             args["display_mode"] = data["displayMode"]
         if "valueMode" in data:
             args["value_mode"] = data["valueMode"]
-        if "namePlacement" in data:
-            args["name_placement"] = data["namePlacement"]
         if "showUnfilled" in data:
             args["show_unfilled"] = data["showUnfilled"]
-        if "sizing" in data:
-            args["sizing"] = data["sizing"]
         if "minVizWidth" in data:
             args["min_viz_width"] = data["minVizWidth"]
-        if "minVizHeight" in data:
-            args["min_viz_height"] = data["minVizHeight"]
         if "reduceOptions" in data:
             args["reduce_options"] = common.ReduceDataOptions.from_json(data["reduceOptions"])
         if "text" in data:
             args["text"] = common.VizTextDisplayOptions.from_json(data["text"])
-        if "maxVizHeight" in data:
-            args["max_viz_height"] = data["maxVizHeight"]
+        if "minVizHeight" in data:
+            args["min_viz_height"] = data["minVizHeight"]
         if "orientation" in data:
             args["orientation"] = data["orientation"]        
 
         return cls(**args)
 
 
 def variant_config():
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/candlestick.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/candlestick.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,37 +114,34 @@
     # Sets the color strategy for the candlesticks
     color_strategy: 'ColorStrategy'
     # Map fields to appropriate dimension
     fields: 'CandlestickFieldMap'
     # Set which colors are used when the price movement is up or down
     colors: 'CandlestickColors'
     legend: common.VizLegendOptions
-    tooltip: common.VizTooltipOptions
     # When enabled, all fields will be sent to the graph
     include_all_fields: typing.Optional[bool]
 
-    def __init__(self, mode: typing.Optional['VizDisplayMode'] = None, candle_style: typing.Optional['CandleStyle'] = None, color_strategy: typing.Optional['ColorStrategy'] = None, fields: typing.Optional['CandlestickFieldMap'] = None, colors: typing.Optional['CandlestickColors'] = None, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, include_all_fields: typing.Optional[bool] = False):
+    def __init__(self, mode: typing.Optional['VizDisplayMode'] = None, candle_style: typing.Optional['CandleStyle'] = None, color_strategy: typing.Optional['ColorStrategy'] = None, fields: typing.Optional['CandlestickFieldMap'] = None, colors: typing.Optional['CandlestickColors'] = None, legend: typing.Optional[common.VizLegendOptions] = None, include_all_fields: typing.Optional[bool] = False):
         self.mode = mode if mode is not None else VizDisplayMode.CANDLES_VOLUME
         self.candle_style = candle_style if candle_style is not None else CandleStyle.CANDLES
         self.color_strategy = color_strategy if color_strategy is not None else ColorStrategy.OPEN_CLOSE
         self.fields = fields if fields is not None else CandlestickFieldMap()
         self.colors = colors if colors is not None else CandlestickColors(down="red", flat="gray", up="green")
         self.legend = legend if legend is not None else common.VizLegendOptions()
-        self.tooltip = tooltip if tooltip is not None else common.VizTooltipOptions()
         self.include_all_fields = include_all_fields
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "mode": self.mode,
             "candleStyle": self.candle_style,
             "colorStrategy": self.color_strategy,
             "fields": self.fields,
             "colors": self.colors,
             "legend": self.legend,
-            "tooltip": self.tooltip,
         }
         if self.include_all_fields is not None:
             payload["includeAllFields"] = self.include_all_fields
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
@@ -158,16 +155,14 @@
             args["color_strategy"] = data["colorStrategy"]
         if "fields" in data:
             args["fields"] = CandlestickFieldMap.from_json(data["fields"])
         if "colors" in data:
             args["colors"] = CandlestickColors.from_json(data["colors"])
         if "legend" in data:
             args["legend"] = common.VizLegendOptions.from_json(data["legend"])
-        if "tooltip" in data:
-            args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])
         if "includeAllFields" in data:
             args["include_all_fields"] = data["includeAllFields"]        
 
         return cls(**args)
 
 
 FieldConfig: typing.TypeAlias = common.GraphFieldConfig
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/canvas.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,24 +54,22 @@
 class Placement:
     top: typing.Optional[float]
     left: typing.Optional[float]
     right: typing.Optional[float]
     bottom: typing.Optional[float]
     width: typing.Optional[float]
     height: typing.Optional[float]
-    rotation: typing.Optional[float]
 
-    def __init__(self, top: typing.Optional[float] = None, left: typing.Optional[float] = None, right: typing.Optional[float] = None, bottom: typing.Optional[float] = None, width: typing.Optional[float] = None, height: typing.Optional[float] = None, rotation: typing.Optional[float] = None):
+    def __init__(self, top: typing.Optional[float] = None, left: typing.Optional[float] = None, right: typing.Optional[float] = None, bottom: typing.Optional[float] = None, width: typing.Optional[float] = None, height: typing.Optional[float] = None):
         self.top = top
         self.left = left
         self.right = right
         self.bottom = bottom
         self.width = width
         self.height = height
-        self.rotation = rotation
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.top is not None:
             payload["top"] = self.top
         if self.left is not None:
@@ -80,16 +78,14 @@
             payload["right"] = self.right
         if self.bottom is not None:
             payload["bottom"] = self.bottom
         if self.width is not None:
             payload["width"] = self.width
         if self.height is not None:
             payload["height"] = self.height
-        if self.rotation is not None:
-            payload["rotation"] = self.rotation
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "top" in data:
@@ -99,17 +95,15 @@
         if "right" in data:
             args["right"] = data["right"]
         if "bottom" in data:
             args["bottom"] = data["bottom"]
         if "width" in data:
             args["width"] = data["width"]
         if "height" in data:
-            args["height"] = data["height"]
-        if "rotation" in data:
-            args["rotation"] = data["rotation"]        
+            args["height"] = data["height"]        
 
         return cls(**args)
 
 
 class BackgroundImageSize(enum.StrEnum):
     ORIGINAL = "original"
     CONTAIN = "contain"
@@ -152,52 +146,40 @@
 
         return cls(**args)
 
 
 class LineConfig:
     color: typing.Optional[common.ColorDimensionConfig]
     width: typing.Optional[float]
-    radius: typing.Optional[float]
 
-    def __init__(self, color: typing.Optional[common.ColorDimensionConfig] = None, width: typing.Optional[float] = None, radius: typing.Optional[float] = None):
+    def __init__(self, color: typing.Optional[common.ColorDimensionConfig] = None, width: typing.Optional[float] = None):
         self.color = color
         self.width = width
-        self.radius = radius
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.color is not None:
             payload["color"] = self.color
         if self.width is not None:
             payload["width"] = self.width
-        if self.radius is not None:
-            payload["radius"] = self.radius
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "color" in data:
             args["color"] = common.ColorDimensionConfig.from_json(data["color"])
         if "width" in data:
-            args["width"] = data["width"]
-        if "radius" in data:
-            args["radius"] = data["radius"]        
+            args["width"] = data["width"]        
 
         return cls(**args)
 
 
-class HttpRequestMethod(enum.StrEnum):
-    GET = "GET"
-    POST = "POST"
-    PUT = "PUT"
-
-
 class ConnectionCoordinates:
     x: float
     y: float
 
     def __init__(self, x: float = 0, y: float = 0):
         self.x = x
         self.y = y
@@ -228,47 +210,35 @@
 class CanvasConnection:
     source: 'ConnectionCoordinates'
     target: 'ConnectionCoordinates'
     target_name: typing.Optional[str]
     path: 'ConnectionPath'
     color: typing.Optional[common.ColorDimensionConfig]
     size: typing.Optional[common.ScaleDimensionConfig]
-    vertices: typing.Optional[list['ConnectionCoordinates']]
-    source_original: typing.Optional['ConnectionCoordinates']
-    target_original: typing.Optional['ConnectionCoordinates']
 
-    def __init__(self, source: typing.Optional['ConnectionCoordinates'] = None, target: typing.Optional['ConnectionCoordinates'] = None, target_name: typing.Optional[str] = None, path: typing.Optional['ConnectionPath'] = None, color: typing.Optional[common.ColorDimensionConfig] = None, size: typing.Optional[common.ScaleDimensionConfig] = None, vertices: typing.Optional[list['ConnectionCoordinates']] = None, source_original: typing.Optional['ConnectionCoordinates'] = None, target_original: typing.Optional['ConnectionCoordinates'] = None):
+    def __init__(self, source: typing.Optional['ConnectionCoordinates'] = None, target: typing.Optional['ConnectionCoordinates'] = None, target_name: typing.Optional[str] = None, path: typing.Optional['ConnectionPath'] = None, color: typing.Optional[common.ColorDimensionConfig] = None, size: typing.Optional[common.ScaleDimensionConfig] = None):
         self.source = source if source is not None else ConnectionCoordinates()
         self.target = target if target is not None else ConnectionCoordinates()
         self.target_name = target_name
         self.path = path if path is not None else ConnectionPath.STRAIGHT
         self.color = color
         self.size = size
-        self.vertices = vertices
-        self.source_original = source_original
-        self.target_original = target_original
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "source": self.source,
             "target": self.target,
             "path": self.path,
         }
         if self.target_name is not None:
             payload["targetName"] = self.target_name
         if self.color is not None:
             payload["color"] = self.color
         if self.size is not None:
             payload["size"] = self.size
-        if self.vertices is not None:
-            payload["vertices"] = self.vertices
-        if self.source_original is not None:
-            payload["sourceOriginal"] = self.source_original
-        if self.target_original is not None:
-            payload["targetOriginal"] = self.target_original
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "source" in data:
@@ -278,21 +248,15 @@
         if "targetName" in data:
             args["target_name"] = data["targetName"]
         if "path" in data:
             args["path"] = data["path"]
         if "color" in data:
             args["color"] = common.ColorDimensionConfig.from_json(data["color"])
         if "size" in data:
-            args["size"] = common.ScaleDimensionConfig.from_json(data["size"])
-        if "vertices" in data:
-            args["vertices"] = data["vertices"]
-        if "sourceOriginal" in data:
-            args["source_original"] = ConnectionCoordinates.from_json(data["sourceOriginal"])
-        if "targetOriginal" in data:
-            args["target_original"] = ConnectionCoordinates.from_json(data["targetOriginal"])        
+            args["size"] = common.ScaleDimensionConfig.from_json(data["size"])        
 
         return cls(**args)
 
 
 class CanvasElementOptions:
     name: str
     type_val: str
@@ -358,51 +322,39 @@
 
 
 class Options:
     # Enable inline editing
     inline_editing: bool
     # Show all available element types
     show_advanced_types: bool
-    # Enable pan and zoom
-    pan_zoom: bool
-    # Enable infinite pan
-    infinite_pan: bool
     # The root element of canvas (frame), where all canvas elements are nested
     # TODO: Figure out how to define a default value for this
     root: 'CanvasOptionsRoot'
 
-    def __init__(self, inline_editing: bool = True, show_advanced_types: bool = True, pan_zoom: bool = True, infinite_pan: bool = True, root: typing.Optional['CanvasOptionsRoot'] = None):
+    def __init__(self, inline_editing: bool = True, show_advanced_types: bool = True, root: typing.Optional['CanvasOptionsRoot'] = None):
         self.inline_editing = inline_editing
         self.show_advanced_types = show_advanced_types
-        self.pan_zoom = pan_zoom
-        self.infinite_pan = infinite_pan
         self.root = root if root is not None else CanvasOptionsRoot()
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "inlineEditing": self.inline_editing,
             "showAdvancedTypes": self.show_advanced_types,
-            "panZoom": self.pan_zoom,
-            "infinitePan": self.infinite_pan,
             "root": self.root,
         }
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "inlineEditing" in data:
             args["inline_editing"] = data["inlineEditing"]
         if "showAdvancedTypes" in data:
             args["show_advanced_types"] = data["showAdvancedTypes"]
-        if "panZoom" in data:
-            args["pan_zoom"] = data["panZoom"]
-        if "infinitePan" in data:
-            args["infinite_pan"] = data["infinitePan"]
         if "root" in data:
             args["root"] = CanvasOptionsRoot.from_json(data["root"])        
 
         return cls(**args)
 
 
 class CanvasOptionsRoot:
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/cloudwatch.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/cloudwatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,17 @@
     expression: typing.Optional[str]
     # When the metric query type is `metricQueryType` is set to `Query`, this field is used to specify the query string.
     sql_expression: typing.Optional[str]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # AWS region to query for the metric
     region: str
     # A namespace is a container for CloudWatch metrics. Metrics in different namespaces are isolated from each other, so that metrics from different applications are not mistakenly aggregated into the same statistics. For example, Amazon EC2 uses the AWS/EC2 namespace.
@@ -328,15 +330,15 @@
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "select" in data:
             args["select"] = QueryEditorFunctionExpression.from_json(data["select"])
         if "from" in data:
-            decoding_map: dict[str, typing.Union[typing.Type[QueryEditorPropertyExpression], typing.Type[QueryEditorFunctionExpression]]] = {"property": QueryEditorPropertyExpression, "function": QueryEditorFunctionExpression}
+            decoding_map: dict[str, typing.Union[typing.Type[QueryEditorFunctionExpression], typing.Type[QueryEditorPropertyExpression]]] = {"function": QueryEditorFunctionExpression, "property": QueryEditorPropertyExpression}
             args["from_val"] = decoding_map[data["from"]["type"]].from_json(data["from"])
         if "where" in data:
             args["where"] = QueryEditorArrayExpression.from_json(data["where"])
         if "groupBy" in data:
             args["group_by"] = QueryEditorArrayExpression.from_json(data["groupBy"])
         if "orderBy" in data:
             args["order_by"] = QueryEditorFunctionExpression.from_json(data["orderBy"])
@@ -614,15 +616,17 @@
     stats_groups: typing.Optional[list[str]]
     # Log groups to query
     log_groups: typing.Optional[list['LogGroup']]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # @deprecated use logGroups
     log_group_names: typing.Optional[list[str]]
     # For mixed data sources the selected datasource is on the query level.
@@ -757,15 +761,17 @@
     # e.g. `arn:aws:sns:us-east-1:123456789012:my-app-` would match `arn:aws:sns:us-east-1:123456789012:my-app-action`
     # but not match `arn:aws:sns:us-east-1:123456789012:your-app-action`
     action_prefix: typing.Optional[str]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # AWS region to query for the metric
     region: str
     # A namespace is a container for CloudWatch metrics. Metrics in different namespaces are isolated from each other, so that metrics from different applications are not mistakenly aggregated into the same statistics. For example, Amazon EC2 uses the AWS/EC2 namespace.
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/common.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,11 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-import enum
 import typing
-
-
-class DataTopic(enum.StrEnum):
-    """
-    A topic is attached to DataFrame metadata in query results.
-    This specifies where the data should be used.
-    """
-
-    SERIES = "series"
-    ANNOTATIONS = "annotations"
-    ALERT_STATES = "alertStates"
+import enum
 
 
 class DataSourceJsonData:
     """
     TODO docs
     """
 
@@ -73,15 +62,17 @@
     properties for the given context.
     """
 
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
@@ -836,27 +827,25 @@
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional['ScaleDistributionConfig']
     axis_centered_zero: typing.Optional[bool]
-    axis_border_show: typing.Optional[bool]
 
-    def __init__(self, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, axis_centered_zero: typing.Optional[bool] = None, axis_border_show: typing.Optional[bool] = None):
+    def __init__(self, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, axis_centered_zero: typing.Optional[bool] = None):
         self.axis_placement = axis_placement
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
         self.axis_centered_zero = axis_centered_zero
-        self.axis_border_show = axis_border_show
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.axis_placement is not None:
             payload["axisPlacement"] = self.axis_placement
         if self.axis_color_mode is not None:
@@ -871,16 +860,14 @@
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
         if self.axis_centered_zero is not None:
             payload["axisCenteredZero"] = self.axis_centered_zero
-        if self.axis_border_show is not None:
-            payload["axisBorderShow"] = self.axis_border_show
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "axisPlacement" in data:
@@ -896,17 +883,15 @@
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = ScaleDistributionConfig.from_json(data["scaleDistribution"])
         if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
-        if "axisBorderShow" in data:
-            args["axis_border_show"] = data["axisBorderShow"]        
+            args["axis_centered_zero"] = data["axisCenteredZero"]        
 
         return cls(**args)
 
 
 class HideSeriesConfig:
     """
     TODO docs
@@ -1026,15 +1011,15 @@
         
         if "hideFrom" in data:
             args["hide_from"] = HideSeriesConfig.from_json(data["hideFrom"])        
 
         return cls(**args)
 
 
-class GraphThresholdsStyleMode(enum.StrEnum):
+class GraphTresholdsStyleMode(enum.StrEnum):
     """
     TODO docs
     """
 
     OFF = "off"
     LINE = "line"
     DASHED = "dashed"
@@ -1045,18 +1030,18 @@
 
 
 class GraphThresholdsStyleConfig:
     """
     TODO docs
     """
 
-    mode: 'GraphThresholdsStyleMode'
+    mode: 'GraphTresholdsStyleMode'
 
-    def __init__(self, mode: typing.Optional['GraphThresholdsStyleMode'] = None):
-        self.mode = mode if mode is not None else GraphThresholdsStyleMode.OFF
+    def __init__(self, mode: typing.Optional['GraphTresholdsStyleMode'] = None):
+        self.mode = mode if mode is not None else GraphTresholdsStyleMode.OFF
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "mode": self.mode,
         }
         return payload
 
@@ -1431,31 +1416,30 @@
     axis_color_mode: typing.Optional['AxisColorMode']
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional['ScaleDistributionConfig']
-    axis_centered_zero: typing.Optional[bool]
     bar_alignment: typing.Optional['BarAlignment']
     bar_width_factor: typing.Optional[float]
     stacking: typing.Optional['StackingConfig']
     hide_from: typing.Optional['HideSeriesConfig']
     transform: typing.Optional['GraphTransform']
     # Indicate if null values should be treated as gaps or connected.
     # When the value is a number, it represents the maximum delta in the
     # X axis that should be considered connected.  For timeseries, this is milliseconds
     span_nulls: typing.Optional[typing.Union[bool, float]]
     fill_below_to: typing.Optional[str]
     point_symbol: typing.Optional[str]
-    axis_border_show: typing.Optional[bool]
+    axis_centered_zero: typing.Optional[bool]
     bar_max_width: typing.Optional[float]
     insert_nulls: typing.Optional[typing.Union[bool, int]]
 
-    def __init__(self, draw_style: typing.Optional['GraphDrawStyle'] = None, gradient_mode: typing.Optional['GraphGradientMode'] = None, thresholds_style: typing.Optional['GraphThresholdsStyleConfig'] = None, line_color: typing.Optional[str] = None, line_width: typing.Optional[float] = None, line_interpolation: typing.Optional['LineInterpolation'] = None, line_style: typing.Optional['LineStyle'] = None, fill_color: typing.Optional[str] = None, fill_opacity: typing.Optional[float] = None, show_points: typing.Optional['VisibilityMode'] = None, point_size: typing.Optional[float] = None, point_color: typing.Optional[str] = None, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, axis_centered_zero: typing.Optional[bool] = None, bar_alignment: typing.Optional['BarAlignment'] = None, bar_width_factor: typing.Optional[float] = None, stacking: typing.Optional['StackingConfig'] = None, hide_from: typing.Optional['HideSeriesConfig'] = None, transform: typing.Optional['GraphTransform'] = None, span_nulls: typing.Optional[typing.Union[bool, float]] = None, fill_below_to: typing.Optional[str] = None, point_symbol: typing.Optional[str] = None, axis_border_show: typing.Optional[bool] = None, bar_max_width: typing.Optional[float] = None, insert_nulls: typing.Optional[typing.Union[bool, int]] = None):
+    def __init__(self, draw_style: typing.Optional['GraphDrawStyle'] = None, gradient_mode: typing.Optional['GraphGradientMode'] = None, thresholds_style: typing.Optional['GraphThresholdsStyleConfig'] = None, line_color: typing.Optional[str] = None, line_width: typing.Optional[float] = None, line_interpolation: typing.Optional['LineInterpolation'] = None, line_style: typing.Optional['LineStyle'] = None, fill_color: typing.Optional[str] = None, fill_opacity: typing.Optional[float] = None, show_points: typing.Optional['VisibilityMode'] = None, point_size: typing.Optional[float] = None, point_color: typing.Optional[str] = None, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, bar_alignment: typing.Optional['BarAlignment'] = None, bar_width_factor: typing.Optional[float] = None, stacking: typing.Optional['StackingConfig'] = None, hide_from: typing.Optional['HideSeriesConfig'] = None, transform: typing.Optional['GraphTransform'] = None, span_nulls: typing.Optional[typing.Union[bool, float]] = None, fill_below_to: typing.Optional[str] = None, point_symbol: typing.Optional[str] = None, axis_centered_zero: typing.Optional[bool] = None, bar_max_width: typing.Optional[float] = None, insert_nulls: typing.Optional[typing.Union[bool, int]] = None):
         self.draw_style = draw_style
         self.gradient_mode = gradient_mode
         self.thresholds_style = thresholds_style
         self.line_color = line_color
         self.line_width = line_width
         self.line_interpolation = line_interpolation
         self.line_style = line_style
@@ -1468,24 +1452,23 @@
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
-        self.axis_centered_zero = axis_centered_zero
         self.bar_alignment = bar_alignment
         self.bar_width_factor = bar_width_factor
         self.stacking = stacking
         self.hide_from = hide_from
         self.transform = transform
         self.span_nulls = span_nulls
         self.fill_below_to = fill_below_to
         self.point_symbol = point_symbol
-        self.axis_border_show = axis_border_show
+        self.axis_centered_zero = axis_centered_zero
         self.bar_max_width = bar_max_width
         self.insert_nulls = insert_nulls
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.draw_style is not None:
@@ -1524,16 +1507,14 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.bar_alignment is not None:
             payload["barAlignment"] = self.bar_alignment
         if self.bar_width_factor is not None:
             payload["barWidthFactor"] = self.bar_width_factor
         if self.stacking is not None:
             payload["stacking"] = self.stacking
         if self.hide_from is not None:
@@ -1542,16 +1523,16 @@
             payload["transform"] = self.transform
         if self.span_nulls is not None:
             payload["spanNulls"] = self.span_nulls
         if self.fill_below_to is not None:
             payload["fillBelowTo"] = self.fill_below_to
         if self.point_symbol is not None:
             payload["pointSymbol"] = self.point_symbol
-        if self.axis_border_show is not None:
-            payload["axisBorderShow"] = self.axis_border_show
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.bar_max_width is not None:
             payload["barMaxWidth"] = self.bar_max_width
         if self.insert_nulls is not None:
             payload["insertNulls"] = self.insert_nulls
         return payload
 
     @classmethod
@@ -1594,16 +1575,14 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = ScaleDistributionConfig.from_json(data["scaleDistribution"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "barAlignment" in data:
             args["bar_alignment"] = data["barAlignment"]
         if "barWidthFactor" in data:
             args["bar_width_factor"] = data["barWidthFactor"]
         if "stacking" in data:
             args["stacking"] = StackingConfig.from_json(data["stacking"])
         if "hideFrom" in data:
@@ -1612,16 +1591,16 @@
             args["transform"] = data["transform"]
         if "spanNulls" in data:
             args["span_nulls"] = data["spanNulls"]
         if "fillBelowTo" in data:
             args["fill_below_to"] = data["fillBelowTo"]
         if "pointSymbol" in data:
             args["point_symbol"] = data["pointSymbol"]
-        if "axisBorderShow" in data:
-            args["axis_border_show"] = data["axisBorderShow"]
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "barMaxWidth" in data:
             args["bar_max_width"] = data["barMaxWidth"]
         if "insertNulls" in data:
             args["insert_nulls"] = data["insertNulls"]        
 
         return cls(**args)
 
@@ -1714,72 +1693,41 @@
     """
 
     COLOR = "color"
     TEXT = "text"
     HIDDEN = "hidden"
 
 
-class BarGaugeNamePlacement(enum.StrEnum):
-    """
-    Allows for the bar gauge name to be placed explicitly
-    """
-
-    AUTO = "auto"
-    TOP = "top"
-    LEFT = "left"
-
-
-class BarGaugeSizing(enum.StrEnum):
-    """
-    Allows for the bar gauge size to be set explicitly
-    """
-
-    AUTO = "auto"
-    MANUAL = "manual"
-
-
 class VizTooltipOptions:
     """
     TODO docs
     """
 
     mode: 'TooltipDisplayMode'
     sort: 'SortOrder'
-    max_width: typing.Optional[float]
-    max_height: typing.Optional[float]
 
-    def __init__(self, mode: typing.Optional['TooltipDisplayMode'] = None, sort: typing.Optional['SortOrder'] = None, max_width: typing.Optional[float] = None, max_height: typing.Optional[float] = None):
+    def __init__(self, mode: typing.Optional['TooltipDisplayMode'] = None, sort: typing.Optional['SortOrder'] = None):
         self.mode = mode if mode is not None else TooltipDisplayMode.SINGLE
         self.sort = sort if sort is not None else SortOrder.ASCENDING
-        self.max_width = max_width
-        self.max_height = max_height
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "mode": self.mode,
             "sort": self.sort,
         }
-        if self.max_width is not None:
-            payload["maxWidth"] = self.max_width
-        if self.max_height is not None:
-            payload["maxHeight"] = self.max_height
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "mode" in data:
             args["mode"] = data["mode"]
         if "sort" in data:
-            args["sort"] = data["sort"]
-        if "maxWidth" in data:
-            args["max_width"] = data["maxWidth"]
-        if "maxHeight" in data:
-            args["max_height"] = data["maxHeight"]        
+            args["sort"] = data["sort"]        
 
         return cls(**args)
 
 
 Labels: typing.TypeAlias = dict[str, str]
 
 
@@ -1798,15 +1746,14 @@
     GRADIENT_GAUGE = "gradient-gauge"
     LCD_GAUGE = "lcd-gauge"
     JSON_VIEW = "json-view"
     BASIC_GAUGE = "basic"
     IMAGE = "image"
     GAUGE = "gauge"
     SPARKLINE = "sparkline"
-    DATA_LINKS = "data-links"
     CUSTOM = "custom"
 
 
 class TableCellBackgroundDisplayMode(enum.StrEnum):
     """
     Display mode to the "Colored Background" display
     mode for table cells. Either displays a solid color (basic mode)
@@ -1985,36 +1932,14 @@
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         return cls(**args)
 
 
-class TableDataLinksCellOptions:
-    """
-    Show data links in the cell
-    """
-
-    type_val: typing.Literal["data-links"]
-
-    def __init__(self, ):
-        self.type_val = "data-links"
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "type": self.type_val,
-        }
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        return cls(**args)
-
-
 class TableBarGaugeCellOptions:
     """
     Gauge cell options
     """
 
     type_val: typing.Literal["gauge"]
     mode: typing.Optional['BarGaugeDisplayMode']
@@ -2069,31 +1994,29 @@
     axis_color_mode: typing.Optional['AxisColorMode']
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional['ScaleDistributionConfig']
-    axis_centered_zero: typing.Optional[bool]
     bar_alignment: typing.Optional['BarAlignment']
     bar_width_factor: typing.Optional[float]
     stacking: typing.Optional['StackingConfig']
     hide_from: typing.Optional['HideSeriesConfig']
-    hide_value: typing.Optional[bool]
     transform: typing.Optional['GraphTransform']
     # Indicate if null values should be treated as gaps or connected.
     # When the value is a number, it represents the maximum delta in the
     # X axis that should be considered connected.  For timeseries, this is milliseconds
     span_nulls: typing.Optional[typing.Union[bool, float]]
     fill_below_to: typing.Optional[str]
     point_symbol: typing.Optional[str]
-    axis_border_show: typing.Optional[bool]
+    axis_centered_zero: typing.Optional[bool]
     bar_max_width: typing.Optional[float]
 
-    def __init__(self, draw_style: typing.Optional['GraphDrawStyle'] = None, gradient_mode: typing.Optional['GraphGradientMode'] = None, thresholds_style: typing.Optional['GraphThresholdsStyleConfig'] = None, line_color: typing.Optional[str] = None, line_width: typing.Optional[float] = None, line_interpolation: typing.Optional['LineInterpolation'] = None, line_style: typing.Optional['LineStyle'] = None, fill_color: typing.Optional[str] = None, fill_opacity: typing.Optional[float] = None, show_points: typing.Optional['VisibilityMode'] = None, point_size: typing.Optional[float] = None, point_color: typing.Optional[str] = None, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, axis_centered_zero: typing.Optional[bool] = None, bar_alignment: typing.Optional['BarAlignment'] = None, bar_width_factor: typing.Optional[float] = None, stacking: typing.Optional['StackingConfig'] = None, hide_from: typing.Optional['HideSeriesConfig'] = None, hide_value: typing.Optional[bool] = None, transform: typing.Optional['GraphTransform'] = None, span_nulls: typing.Optional[typing.Union[bool, float]] = None, fill_below_to: typing.Optional[str] = None, point_symbol: typing.Optional[str] = None, axis_border_show: typing.Optional[bool] = None, bar_max_width: typing.Optional[float] = None):
+    def __init__(self, draw_style: typing.Optional['GraphDrawStyle'] = None, gradient_mode: typing.Optional['GraphGradientMode'] = None, thresholds_style: typing.Optional['GraphThresholdsStyleConfig'] = None, line_color: typing.Optional[str] = None, line_width: typing.Optional[float] = None, line_interpolation: typing.Optional['LineInterpolation'] = None, line_style: typing.Optional['LineStyle'] = None, fill_color: typing.Optional[str] = None, fill_opacity: typing.Optional[float] = None, show_points: typing.Optional['VisibilityMode'] = None, point_size: typing.Optional[float] = None, point_color: typing.Optional[str] = None, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, bar_alignment: typing.Optional['BarAlignment'] = None, bar_width_factor: typing.Optional[float] = None, stacking: typing.Optional['StackingConfig'] = None, hide_from: typing.Optional['HideSeriesConfig'] = None, transform: typing.Optional['GraphTransform'] = None, span_nulls: typing.Optional[typing.Union[bool, float]] = None, fill_below_to: typing.Optional[str] = None, point_symbol: typing.Optional[str] = None, axis_centered_zero: typing.Optional[bool] = None, bar_max_width: typing.Optional[float] = None):
         self.type_val = "sparkline"
         self.draw_style = draw_style
         self.gradient_mode = gradient_mode
         self.thresholds_style = thresholds_style
         self.line_color = line_color
         self.line_width = line_width
         self.line_interpolation = line_interpolation
@@ -2107,25 +2030,23 @@
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
-        self.axis_centered_zero = axis_centered_zero
         self.bar_alignment = bar_alignment
         self.bar_width_factor = bar_width_factor
         self.stacking = stacking
         self.hide_from = hide_from
-        self.hide_value = hide_value
         self.transform = transform
         self.span_nulls = span_nulls
         self.fill_below_to = fill_below_to
         self.point_symbol = point_symbol
-        self.axis_border_show = axis_border_show
+        self.axis_centered_zero = axis_centered_zero
         self.bar_max_width = bar_max_width
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
         }
         if self.draw_style is not None:
@@ -2164,36 +2085,32 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.bar_alignment is not None:
             payload["barAlignment"] = self.bar_alignment
         if self.bar_width_factor is not None:
             payload["barWidthFactor"] = self.bar_width_factor
         if self.stacking is not None:
             payload["stacking"] = self.stacking
         if self.hide_from is not None:
             payload["hideFrom"] = self.hide_from
-        if self.hide_value is not None:
-            payload["hideValue"] = self.hide_value
         if self.transform is not None:
             payload["transform"] = self.transform
         if self.span_nulls is not None:
             payload["spanNulls"] = self.span_nulls
         if self.fill_below_to is not None:
             payload["fillBelowTo"] = self.fill_below_to
         if self.point_symbol is not None:
             payload["pointSymbol"] = self.point_symbol
-        if self.axis_border_show is not None:
-            payload["axisBorderShow"] = self.axis_border_show
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.bar_max_width is not None:
             payload["barMaxWidth"] = self.bar_max_width
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
@@ -2234,74 +2151,64 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = ScaleDistributionConfig.from_json(data["scaleDistribution"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "barAlignment" in data:
             args["bar_alignment"] = data["barAlignment"]
         if "barWidthFactor" in data:
             args["bar_width_factor"] = data["barWidthFactor"]
         if "stacking" in data:
             args["stacking"] = StackingConfig.from_json(data["stacking"])
         if "hideFrom" in data:
             args["hide_from"] = HideSeriesConfig.from_json(data["hideFrom"])
-        if "hideValue" in data:
-            args["hide_value"] = data["hideValue"]
         if "transform" in data:
             args["transform"] = data["transform"]
         if "spanNulls" in data:
             args["span_nulls"] = data["spanNulls"]
         if "fillBelowTo" in data:
             args["fill_below_to"] = data["fillBelowTo"]
         if "pointSymbol" in data:
             args["point_symbol"] = data["pointSymbol"]
-        if "axisBorderShow" in data:
-            args["axis_border_show"] = data["axisBorderShow"]
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "barMaxWidth" in data:
             args["bar_max_width"] = data["barMaxWidth"]        
 
         return cls(**args)
 
 
 class TableColoredBackgroundCellOptions:
     """
     Colored background cell options
     """
 
     type_val: typing.Literal["color-background"]
     mode: typing.Optional['TableCellBackgroundDisplayMode']
-    apply_to_row: typing.Optional[bool]
 
-    def __init__(self, mode: typing.Optional['TableCellBackgroundDisplayMode'] = None, apply_to_row: typing.Optional[bool] = None):
+    def __init__(self, mode: typing.Optional['TableCellBackgroundDisplayMode'] = None):
         self.type_val = "color-background"
         self.mode = mode
-        self.apply_to_row = apply_to_row
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
         }
         if self.mode is not None:
             payload["mode"] = self.mode
-        if self.apply_to_row is not None:
-            payload["applyToRow"] = self.apply_to_row
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "mode" in data:
-            args["mode"] = data["mode"]
-        if "applyToRow" in data:
-            args["apply_to_row"] = data["applyToRow"]        
+            args["mode"] = data["mode"]        
 
         return cls(**args)
 
 
 class TableCellHeight(enum.StrEnum):
     """
     Height of a table cell
@@ -2310,15 +2217,15 @@
     SM = "sm"
     MD = "md"
     LG = "lg"
 
 
 # Table cell options. Each cell has a display mode
 # and other potential options for that display.
-TableCellOptions: typing.TypeAlias = typing.Union['TableAutoCellOptions', 'TableSparklineCellOptions', 'TableBarGaugeCellOptions', 'TableColoredBackgroundCellOptions', 'TableColorTextCellOptions', 'TableImageCellOptions', 'TableDataLinksCellOptions', 'TableJsonViewCellOptions']
+TableCellOptions: typing.TypeAlias = typing.Union['TableAutoCellOptions', 'TableSparklineCellOptions', 'TableBarGaugeCellOptions', 'TableColoredBackgroundCellOptions', 'TableColorTextCellOptions', 'TableImageCellOptions', 'TableJsonViewCellOptions']
 
 
 # Use UTC/GMT timezone
 TimeZoneUtc: typing.Literal["utc"] = "utc"
 
 
 # Use the timezone defined by end user web browser
@@ -2543,15 +2450,15 @@
     # This field is deprecated in favor of using cellOptions
     display_mode: typing.Optional['TableCellDisplayMode']
     cell_options: typing.Optional['TableCellOptions']
     # ?? default is missing or false ??
     hidden: typing.Optional[bool]
     inspect: bool
     filterable: typing.Optional[bool]
-    # Hides any header for a column, useful for columns that show some static content or buttons.
+    # Hides any header for a column, usefull for columns that show some static content or buttons.
     hide_header: typing.Optional[bool]
 
     def __init__(self, width: typing.Optional[float] = None, min_width: typing.Optional[float] = None, align: typing.Optional['FieldTextAlignment'] = None, display_mode: typing.Optional['TableCellDisplayMode'] = None, cell_options: typing.Optional['TableCellOptions'] = None, hidden: typing.Optional[bool] = None, inspect: bool = False, filterable: typing.Optional[bool] = None, hide_header: typing.Optional[bool] = None):
         self.width = width
         self.min_width = min_width
         self.align = align if align is not None else FieldTextAlignment.AUTO
         self.display_mode = display_mode
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/dashboard.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,36 +19,39 @@
     # This property should only be used in dashboards defined by plugins.  It is a quick check
     # to see if the version has changed since the last time.
     revision: typing.Optional[int]
     # ID of a dashboard imported from the https://grafana.com/grafana/dashboards/ portal
     gnet_id: typing.Optional[str]
     # Tags associated with dashboard.
     tags: typing.Optional[list[str]]
+    # Theme of dashboard.
+    # Default value: dark.
+    style: typing.Literal["light", "dark"]
     # Timezone of dashboard. Accepted values are IANA TZDB zone ID or "browser" or "utc".
     timezone: typing.Optional[str]
     # Whether a dashboard is editable or not.
-    editable: typing.Optional[bool]
+    editable: bool
     # Configuration of dashboard cursor sync behavior.
     # Accepted values are 0 (sync turned off), 1 (shared crosshair), 2 (shared crosshair and tooltip).
-    graph_tooltip: typing.Optional['DashboardCursorSync']
+    graph_tooltip: 'DashboardCursorSync'
     # Time range for dashboard.
     # Accepted values are relative time strings like {from: 'now-6h', to: 'now'} or absolute time strings like {from: '2020-07-10T08:00:00.000Z', to: '2020-07-10T14:00:00.000Z'}.
     time: typing.Optional['DashboardDashboardTime']
     # Configuration of the time picker shown at the top of a dashboard.
-    timepicker: typing.Optional['TimePickerConfig']
+    timepicker: typing.Optional['TimePicker']
     # The month that the fiscal year starts on.  0 = January, 11 = December
     fiscal_year_start_month: typing.Optional[int]
     # When set to true, the dashboard will redraw panels at an interval matching the pixel width.
     # This will keep data "moving left" regardless of the query refresh rate. This setting helps
     # avoid dashboards presenting stale live data
     live_now: typing.Optional[bool]
     # Day when the week starts. Expressed by the name of the day in lowercase, e.g. "monday".
     week_start: typing.Optional[str]
     # Refresh rate of dashboard. Represented via interval string, e.g. "5s", "1m", "1h", "1d".
-    refresh: typing.Optional[str]
+    refresh: typing.Optional[typing.Union[str, typing.Literal[False]]]
     # Version of the JSON schema, incremented each time a Grafana update brings
     # changes to said schema.
     schema_version: int
     # Version of the dashboard, incremented each time the dashboard is updated.
     version: typing.Optional[int]
     # List of dashboard panels
     panels: typing.Optional[list[typing.Union['Panel', 'RowPanel']]]
@@ -60,22 +63,23 @@
     # See https://grafana.com/docs/grafana/latest/dashboards/build-dashboards/annotate-visualizations/
     annotations: 'AnnotationContainer'
     # Links with references to other dashboards or external websites.
     links: typing.Optional[list['DashboardLink']]
     # Snapshot options. They are present only if the dashboard is a snapshot.
     snapshot: typing.Optional['Snapshot']
 
-    def __init__(self, id_val: typing.Optional[int] = None, uid: typing.Optional[str] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, revision: typing.Optional[int] = None, gnet_id: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, timezone: typing.Optional[str] = "browser", editable: typing.Optional[bool] = True, graph_tooltip: typing.Optional['DashboardCursorSync'] = None, time: typing.Optional['DashboardDashboardTime'] = None, timepicker: typing.Optional['TimePickerConfig'] = None, fiscal_year_start_month: typing.Optional[int] = 0, live_now: typing.Optional[bool] = None, week_start: typing.Optional[str] = None, refresh: typing.Optional[str] = None, schema_version: int = 36, version: typing.Optional[int] = None, panels: typing.Optional[list[typing.Union['Panel', 'RowPanel']]] = None, templating: typing.Optional['DashboardDashboardTemplating'] = None, annotations: typing.Optional['AnnotationContainer'] = None, links: typing.Optional[list['DashboardLink']] = None, snapshot: typing.Optional['Snapshot'] = None):
+    def __init__(self, id_val: typing.Optional[int] = None, uid: typing.Optional[str] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, revision: typing.Optional[int] = None, gnet_id: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, style: typing.Optional[typing.Literal["light", "dark"]] = None, timezone: typing.Optional[str] = "browser", editable: bool = True, graph_tooltip: typing.Optional['DashboardCursorSync'] = None, time: typing.Optional['DashboardDashboardTime'] = None, timepicker: typing.Optional['TimePicker'] = None, fiscal_year_start_month: typing.Optional[int] = 0, live_now: typing.Optional[bool] = None, week_start: typing.Optional[str] = None, refresh: typing.Optional[typing.Union[str, typing.Literal[False]]] = None, schema_version: int = 36, version: typing.Optional[int] = None, panels: typing.Optional[list[typing.Union['Panel', 'RowPanel']]] = None, templating: typing.Optional['DashboardDashboardTemplating'] = None, annotations: typing.Optional['AnnotationContainer'] = None, links: typing.Optional[list['DashboardLink']] = None, snapshot: typing.Optional['Snapshot'] = None):
         self.id_val = id_val
         self.uid = uid
         self.title = title
         self.description = description
         self.revision = revision
         self.gnet_id = gnet_id
         self.tags = tags
+        self.style = style if style is not None else "dark"
         self.timezone = timezone
         self.editable = editable
         self.graph_tooltip = graph_tooltip if graph_tooltip is not None else DashboardCursorSync.OFF
         self.time = time
         self.timepicker = timepicker
         self.fiscal_year_start_month = fiscal_year_start_month
         self.live_now = live_now
@@ -87,14 +91,17 @@
         self.templating = templating if templating is not None else DashboardDashboardTemplating()
         self.annotations = annotations if annotations is not None else AnnotationContainer()
         self.links = links
         self.snapshot = snapshot
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
+            "style": self.style,
+            "editable": self.editable,
+            "graphTooltip": self.graph_tooltip,
             "schemaVersion": self.schema_version,
             "templating": self.templating,
             "annotations": self.annotations,
         }
         if self.id_val is not None:
             payload["id"] = self.id_val
         if self.uid is not None:
@@ -107,18 +114,14 @@
             payload["revision"] = self.revision
         if self.gnet_id is not None:
             payload["gnetId"] = self.gnet_id
         if self.tags is not None:
             payload["tags"] = self.tags
         if self.timezone is not None:
             payload["timezone"] = self.timezone
-        if self.editable is not None:
-            payload["editable"] = self.editable
-        if self.graph_tooltip is not None:
-            payload["graphTooltip"] = self.graph_tooltip
         if self.time is not None:
             payload["time"] = self.time
         if self.timepicker is not None:
             payload["timepicker"] = self.timepicker
         if self.fiscal_year_start_month is not None:
             payload["fiscalYearStartMonth"] = self.fiscal_year_start_month
         if self.live_now is not None:
@@ -151,24 +154,26 @@
             args["description"] = data["description"]
         if "revision" in data:
             args["revision"] = data["revision"]
         if "gnetId" in data:
             args["gnet_id"] = data["gnetId"]
         if "tags" in data:
             args["tags"] = data["tags"]
+        if "style" in data:
+            args["style"] = data["style"]
         if "timezone" in data:
             args["timezone"] = data["timezone"]
         if "editable" in data:
             args["editable"] = data["editable"]
         if "graphTooltip" in data:
             args["graph_tooltip"] = data["graphTooltip"]
         if "time" in data:
             args["time"] = DashboardDashboardTime.from_json(data["time"])
         if "timepicker" in data:
-            args["timepicker"] = TimePickerConfig.from_json(data["timepicker"])
+            args["timepicker"] = TimePicker.from_json(data["timepicker"])
         if "fiscalYearStartMonth" in data:
             args["fiscal_year_start_month"] = data["fiscalYearStartMonth"]
         if "liveNow" in data:
             args["live_now"] = data["liveNow"]
         if "weekStart" in data:
             args["week_start"] = data["weekStart"]
         if "refresh" in data:
@@ -322,27 +327,24 @@
     icon_color: str
     # Filters to apply when fetching annotations
     filter_val: typing.Optional['AnnotationPanelFilter']
     # TODO.. this should just be a normal query target
     target: typing.Optional['AnnotationTarget']
     # TODO -- this should not exist here, it is based on the --grafana-- datasource
     type_val: typing.Optional[str]
-    # Set to 1 for the standard annotation query all dashboards have by default.
-    built_in: typing.Optional[float]
 
-    def __init__(self, name: str = "", datasource: typing.Optional['DataSourceRef'] = None, enable: bool = True, hide: typing.Optional[bool] = False, icon_color: str = "", filter_val: typing.Optional['AnnotationPanelFilter'] = None, target: typing.Optional['AnnotationTarget'] = None, type_val: typing.Optional[str] = None, built_in: typing.Optional[float] = 0):
+    def __init__(self, name: str = "", datasource: typing.Optional['DataSourceRef'] = None, enable: bool = True, hide: typing.Optional[bool] = False, icon_color: str = "", filter_val: typing.Optional['AnnotationPanelFilter'] = None, target: typing.Optional['AnnotationTarget'] = None, type_val: typing.Optional[str] = None):
         self.name = name
         self.datasource = datasource if datasource is not None else DataSourceRef()
         self.enable = enable
         self.hide = hide
         self.icon_color = icon_color
         self.filter_val = filter_val
         self.target = target
         self.type_val = type_val
-        self.built_in = built_in
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "name": self.name,
             "datasource": self.datasource,
             "enable": self.enable,
             "iconColor": self.icon_color,
@@ -351,16 +353,14 @@
             payload["hide"] = self.hide
         if self.filter_val is not None:
             payload["filter"] = self.filter_val
         if self.target is not None:
             payload["target"] = self.target
         if self.type_val is not None:
             payload["type"] = self.type_val
-        if self.built_in is not None:
-            payload["builtIn"] = self.built_in
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "name" in data:
@@ -374,42 +374,44 @@
         if "iconColor" in data:
             args["icon_color"] = data["iconColor"]
         if "filter" in data:
             args["filter_val"] = AnnotationPanelFilter.from_json(data["filter"])
         if "target" in data:
             args["target"] = AnnotationTarget.from_json(data["target"])
         if "type" in data:
-            args["type_val"] = data["type"]
-        if "builtIn" in data:
-            args["built_in"] = data["builtIn"]        
+            args["type_val"] = data["type"]        
 
         return cls(**args)
 
 
 class VariableModel:
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
 
+    # Unique numeric identifier for the variable.
+    id_val: str
     # Type of variable
     type_val: 'VariableType'
     # Name of variable
     name: str
     # Optional display name
     label: typing.Optional[str]
     # Visibility configuration for the variable
-    hide: typing.Optional['VariableHide']
+    hide: 'VariableHide'
     # Whether the variable value should be managed by URL query params or not
-    skip_url_sync: typing.Optional[bool]
+    skip_url_sync: bool
     # Description of variable. It can be defined but `null`.
     description: typing.Optional[str]
     # Query used to fetch values for a variable
     query: typing.Optional[typing.Union[str, object]]
     # Data source used to fetch values for a variable. It can be defined but `null`.
     datasource: typing.Optional['DataSourceRef']
+    # Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
+    all_format: typing.Optional[str]
     # Shows current selected variable text/value on the dashboard
     current: typing.Optional['VariableOption']
     # Whether multiple values can be selected or not from variable value list
     multi: typing.Optional[bool]
     # Options that can be selected for a variable.
     options: typing.Optional[list['VariableOption']]
     # Options to config when to refresh a variable
@@ -420,49 +422,52 @@
     include_all: typing.Optional[bool]
     # Custom all value
     all_value: typing.Optional[str]
     # Optional field, if you want to extract part of a series name or metric node segment.
     # Named capture groups can be used to separate the display text and value.
     regex: typing.Optional[str]
 
-    def __init__(self, type_val: typing.Optional['VariableType'] = None, name: str = "", label: typing.Optional[str] = None, hide: typing.Optional['VariableHide'] = None, skip_url_sync: typing.Optional[bool] = False, description: typing.Optional[str] = None, query: typing.Optional[typing.Union[str, object]] = None, datasource: typing.Optional['DataSourceRef'] = None, current: typing.Optional['VariableOption'] = None, multi: typing.Optional[bool] = False, options: typing.Optional[list['VariableOption']] = None, refresh: typing.Optional['VariableRefresh'] = None, sort: typing.Optional['VariableSort'] = None, include_all: typing.Optional[bool] = False, all_value: typing.Optional[str] = None, regex: typing.Optional[str] = None):
+    def __init__(self, id_val: str = "00000000-0000-0000-0000-000000000000", type_val: typing.Optional['VariableType'] = None, name: str = "", label: typing.Optional[str] = None, hide: typing.Optional['VariableHide'] = None, skip_url_sync: bool = False, description: typing.Optional[str] = None, query: typing.Optional[typing.Union[str, object]] = None, datasource: typing.Optional['DataSourceRef'] = None, all_format: typing.Optional[str] = None, current: typing.Optional['VariableOption'] = None, multi: typing.Optional[bool] = False, options: typing.Optional[list['VariableOption']] = None, refresh: typing.Optional['VariableRefresh'] = None, sort: typing.Optional['VariableSort'] = None, include_all: typing.Optional[bool] = False, all_value: typing.Optional[str] = None, regex: typing.Optional[str] = None):
+        self.id_val = id_val
         self.type_val = type_val if type_val is not None else VariableType.QUERY
         self.name = name
         self.label = label
-        self.hide = hide
+        self.hide = hide if hide is not None else VariableHide.DONT_HIDE
         self.skip_url_sync = skip_url_sync
         self.description = description
         self.query = query
         self.datasource = datasource
+        self.all_format = all_format
         self.current = current
         self.multi = multi
         self.options = options
         self.refresh = refresh
         self.sort = sort
         self.include_all = include_all
         self.all_value = all_value
         self.regex = regex
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
+            "id": self.id_val,
             "type": self.type_val,
             "name": self.name,
+            "hide": self.hide,
+            "skipUrlSync": self.skip_url_sync,
         }
         if self.label is not None:
             payload["label"] = self.label
-        if self.hide is not None:
-            payload["hide"] = self.hide
-        if self.skip_url_sync is not None:
-            payload["skipUrlSync"] = self.skip_url_sync
         if self.description is not None:
             payload["description"] = self.description
         if self.query is not None:
             payload["query"] = self.query
         if self.datasource is not None:
             payload["datasource"] = self.datasource
+        if self.all_format is not None:
+            payload["allFormat"] = self.all_format
         if self.current is not None:
             payload["current"] = self.current
         if self.multi is not None:
             payload["multi"] = self.multi
         if self.options is not None:
             payload["options"] = self.options
         if self.refresh is not None:
@@ -477,14 +482,16 @@
             payload["regex"] = self.regex
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
+        if "id" in data:
+            args["id_val"] = data["id"]
         if "type" in data:
             args["type_val"] = data["type"]
         if "name" in data:
             args["name"] = data["name"]
         if "label" in data:
             args["label"] = data["label"]
         if "hide" in data:
@@ -493,14 +500,16 @@
             args["skip_url_sync"] = data["skipUrlSync"]
         if "description" in data:
             args["description"] = data["description"]
         if "query" in data:
             args["query"] = data["query"]
         if "datasource" in data:
             args["datasource"] = DataSourceRef.from_json(data["datasource"])
+        if "allFormat" in data:
+            args["all_format"] = data["allFormat"]
         if "current" in data:
             args["current"] = VariableOption.from_json(data["current"])
         if "multi" in data:
             args["multi"] = data["multi"]
         if "options" in data:
             args["options"] = data["options"]
         if "refresh" in data:
@@ -588,27 +597,36 @@
     `0`: No sorting
     `1`: Alphabetical ASC
     `2`: Alphabetical DESC
     `3`: Numerical ASC
     `4`: Numerical DESC
     `5`: Alphabetical Case Insensitive ASC
     `6`: Alphabetical Case Insensitive DESC
-    `7`: Natural ASC
-    `8`: Natural DESC
     """
 
     DISABLED = 0
     ALPHABETICAL_ASC = 1
     ALPHABETICAL_DESC = 2
     NUMERICAL_ASC = 3
     NUMERICAL_DESC = 4
     ALPHABETICAL_CASE_INSENSITIVE_ASC = 5
     ALPHABETICAL_CASE_INSENSITIVE_DESC = 6
-    NATURAL_ASC = 7
-    NATURAL_DESC = 8
+
+
+class LoadingState(enum.StrEnum):
+    """
+    Loading status
+    Accepted values are `NotStarted` (the request is not started), `Loading` (waiting for response), `Streaming` (pulling continuous data), `Done` (response received successfully) or `Error` (failed request).
+    """
+
+    NOT_STARTED = "NotStarted"
+    LOADING = "Loading"
+    STREAMING = "Streaming"
+    DONE = "Done"
+    ERROR = "Error"
 
 
 class DataSourceRef:
     """
     Ref to a DataSource instance
     """
 
@@ -652,27 +670,27 @@
     # Link type. Accepted values are dashboards (to refer to another dashboard) and link (to refer to an external resource)
     type_val: 'DashboardLinkType'
     # Icon name to be displayed with the link
     icon: str
     # Tooltip to display when the user hovers their mouse over it
     tooltip: str
     # Link URL. Only required/valid if the type is link
-    url: typing.Optional[str]
+    url: str
     # List of tags to limit the linked dashboards. If empty, all dashboards will be displayed. Only valid if the type is dashboards
     tags: list[str]
     # If true, all dashboards links will be displayed in a dropdown. If false, all dashboards links will be displayed side by side. Only valid if the type is dashboards
     as_dropdown: bool
     # If true, the link will be opened in a new tab
     target_blank: bool
     # If true, includes current template variables values in the link as query params
     include_vars: bool
     # If true, includes current time range in the link as query params
     keep_time: bool
 
-    def __init__(self, title: str = "", type_val: typing.Optional['DashboardLinkType'] = None, icon: str = "", tooltip: str = "", url: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, as_dropdown: bool = False, target_blank: bool = False, include_vars: bool = False, keep_time: bool = False):
+    def __init__(self, title: str = "", type_val: typing.Optional['DashboardLinkType'] = None, icon: str = "", tooltip: str = "", url: str = "", tags: typing.Optional[list[str]] = None, as_dropdown: bool = False, target_blank: bool = False, include_vars: bool = False, keep_time: bool = False):
         self.title = title
         self.type_val = type_val if type_val is not None else DashboardLinkType.LINK
         self.icon = icon
         self.tooltip = tooltip
         self.url = url
         self.tags = tags if tags is not None else []
         self.as_dropdown = as_dropdown
@@ -682,22 +700,21 @@
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "title": self.title,
             "type": self.type_val,
             "icon": self.icon,
             "tooltip": self.tooltip,
+            "url": self.url,
             "tags": self.tags,
             "asDropdown": self.as_dropdown,
             "targetBlank": self.target_blank,
             "includeVars": self.include_vars,
             "keepTime": self.keep_time,
         }
-        if self.url is not None:
-            payload["url"] = self.url
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "title" in data:
@@ -744,15 +761,14 @@
     `textbox`: Display a free text input field with an optional default value.
     `custom`: Define the variable options manually using a comma-separated list.
     `system`: Variables defined by Grafana. See: https://grafana.com/docs/grafana/latest/dashboards/variables/add-template-variables/#global-variables
     """
 
     QUERY = "query"
     ADHOC = "adhoc"
-    GROUPBY = "groupby"
     CONSTANT = "constant"
     DATASOURCE = "datasource"
     INTERVAL = "interval"
     TEXTBOX = "textbox"
     CUSTOM = "custom"
     SYSTEM = "system"
 
@@ -1190,108 +1206,51 @@
 
     # Unique identifier of transformer
     id_val: str
     # Disabled transformations are skipped
     disabled: typing.Optional[bool]
     # Optional frame matcher. When missing it will be applied to all results
     filter_val: typing.Optional['MatcherConfig']
-    # Where to pull DataFrames from as input to transformation
-    topic: typing.Optional[typing.Literal["series", "annotations", "alertStates"]]
     # Options to be passed to the transformer
     # Valid options depend on the transformer id
     options: object
 
-    def __init__(self, id_val: str = "", disabled: typing.Optional[bool] = None, filter_val: typing.Optional['MatcherConfig'] = None, topic: typing.Optional[typing.Literal["series", "annotations", "alertStates"]] = None, options: object = None):
+    def __init__(self, id_val: str = "", disabled: typing.Optional[bool] = None, filter_val: typing.Optional['MatcherConfig'] = None, options: object = None):
         self.id_val = id_val
         self.disabled = disabled
         self.filter_val = filter_val
-        self.topic = topic
         self.options = options
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "id": self.id_val,
             "options": self.options,
         }
         if self.disabled is not None:
             payload["disabled"] = self.disabled
         if self.filter_val is not None:
             payload["filter"] = self.filter_val
-        if self.topic is not None:
-            payload["topic"] = self.topic
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "id" in data:
             args["id_val"] = data["id"]
         if "disabled" in data:
             args["disabled"] = data["disabled"]
         if "filter" in data:
             args["filter_val"] = MatcherConfig.from_json(data["filter"])
-        if "topic" in data:
-            args["topic"] = data["topic"]
         if "options" in data:
             args["options"] = data["options"]        
 
         return cls(**args)
 
 
-class TimePickerConfig:
-    """
-    Time picker configuration
-    It defines the default config for the time picker and the refresh picker for the specific dashboard.
-    """
-
-    # Whether timepicker is visible or not.
-    hidden: typing.Optional[bool]
-    # Interval options available in the refresh picker dropdown.
-    refresh_intervals: typing.Optional[list[str]]
-    # Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
-    time_options: typing.Optional[list[str]]
-    # Override the now time by entering a time delay. Use this option to accommodate known delays in data aggregation to avoid null values.
-    now_delay: typing.Optional[str]
-
-    def __init__(self, hidden: typing.Optional[bool] = False, refresh_intervals: typing.Optional[list[str]] = None, time_options: typing.Optional[list[str]] = None, now_delay: typing.Optional[str] = None):
-        self.hidden = hidden
-        self.refresh_intervals = refresh_intervals if refresh_intervals is not None else ["5s", "10s", "30s", "1m", "5m", "15m", "30m", "1h", "2h", "1d"]
-        self.time_options = time_options if time_options is not None else ["5m", "15m", "1h", "6h", "12h", "24h", "2d", "7d", "30d"]
-        self.now_delay = now_delay
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-        }
-        if self.hidden is not None:
-            payload["hidden"] = self.hidden
-        if self.refresh_intervals is not None:
-            payload["refresh_intervals"] = self.refresh_intervals
-        if self.time_options is not None:
-            payload["time_options"] = self.time_options
-        if self.now_delay is not None:
-            payload["nowDelay"] = self.now_delay
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "hidden" in data:
-            args["hidden"] = data["hidden"]
-        if "refresh_intervals" in data:
-            args["refresh_intervals"] = data["refresh_intervals"]
-        if "time_options" in data:
-            args["time_options"] = data["time_options"]
-        if "nowDelay" in data:
-            args["now_delay"] = data["nowDelay"]        
-
-        return cls(**args)
-
-
 class DashboardCursorSync(enum.IntEnum):
     """
     0 for no shared crosshair or tooltip (default).
     1 for shared crosshair.
     2 for shared crosshair AND shared tooltip.
     """
 
@@ -1313,16 +1272,14 @@
     created: str
     # Time when the snapshot expires, default is never to expire
     expires: str
     # Is the snapshot saved in an external grafana instance
     external: bool
     # external url, if snapshot was shared in external grafana instance
     external_url: str
-    # original url, url of the dashboard that was snapshotted
-    original_url: str
     # Unique identifier of the snapshot
     id_val: int
     # Optional, defined the unique key of the snapshot, required if external is true
     key: str
     # Optional, name of the snapshot
     name: str
     # org id of the snapshot
@@ -1330,35 +1287,33 @@
     # last time when the snapshot was updated
     updated: str
     # url of the snapshot, if snapshot was shared internally
     url: typing.Optional[str]
     # user id of the snapshot creator
     user_id: int
 
-    def __init__(self, created: str = "", expires: str = "", external: bool = False, external_url: str = "", original_url: str = "", id_val: int = 0, key: str = "", name: str = "", org_id: int = 0, updated: str = "", url: typing.Optional[str] = None, user_id: int = 0):
+    def __init__(self, created: str = "", expires: str = "", external: bool = False, external_url: str = "", id_val: int = 0, key: str = "", name: str = "", org_id: int = 0, updated: str = "", url: typing.Optional[str] = None, user_id: int = 0):
         self.created = created
         self.expires = expires
         self.external = external
         self.external_url = external_url
-        self.original_url = original_url
         self.id_val = id_val
         self.key = key
         self.name = name
         self.org_id = org_id
         self.updated = updated
         self.url = url
         self.user_id = user_id
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "created": self.created,
             "expires": self.expires,
             "external": self.external,
             "externalUrl": self.external_url,
-            "originalUrl": self.original_url,
             "id": self.id_val,
             "key": self.key,
             "name": self.name,
             "orgId": self.org_id,
             "updated": self.updated,
             "userId": self.user_id,
         }
@@ -1374,16 +1329,14 @@
             args["created"] = data["created"]
         if "expires" in data:
             args["expires"] = data["expires"]
         if "external" in data:
             args["external"] = data["external"]
         if "externalUrl" in data:
             args["external_url"] = data["externalUrl"]
-        if "originalUrl" in data:
-            args["original_url"] = data["originalUrl"]
         if "id" in data:
             args["id_val"] = data["id"]
         if "key" in data:
             args["key"] = data["key"]
         if "name" in data:
             args["name"] = data["name"]
         if "orgId" in data:
@@ -1405,42 +1358,43 @@
 
     # The panel plugin type id. This is used to find the plugin to display the panel.
     type_val: str
     # Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
     id_val: typing.Optional[int]
     # The version of the plugin that is used for this panel. This is used to find the plugin to display the panel and to migrate old panel configs.
     plugin_version: typing.Optional[str]
+    # Tags for the panel.
+    tags: typing.Optional[list[str]]
     # Depends on the panel plugin. See the plugin documentation for details.
     targets: typing.Optional[list[cogvariants.Dataquery]]
     # Panel title.
     title: typing.Optional[str]
     # Panel description.
     description: typing.Optional[str]
     # Whether to display the panel without a background.
-    transparent: typing.Optional[bool]
+    transparent: bool
     # The datasource used in all targets.
     datasource: typing.Optional['DataSourceRef']
     # Grid position.
     grid_pos: typing.Optional['GridPos']
     # Panel links.
     links: typing.Optional[list['DashboardLink']]
     # Name of template variable to repeat for.
     repeat: typing.Optional[str]
     # Direction to repeat in if 'repeat' is set.
     # `h` for horizontal, `v` for vertical.
     repeat_direction: typing.Optional[typing.Literal["h", "v"]]
-    # Option for repeated panels that controls max items per row
-    # Only relevant for horizontally repeated panels
-    max_per_row: typing.Optional[float]
+    # Id of the repeating panel.
+    repeat_panel_id: typing.Optional[int]
     # The maximum number of data points that the panel queries are retrieving.
     max_data_points: typing.Optional[float]
     # List of transformations that are applied to the panel data before rendering.
     # When there are multiple transformations, Grafana applies them in the order they are listed.
     # Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
-    transformations: typing.Optional[list['DataTransformerConfig']]
+    transformations: list['DataTransformerConfig']
     # The min time interval setting defines a lower limit for the $__interval and $__interval_ms variables.
     # This value must be formatted as a number followed by a valid time
     # identifier like: "40s", "3d", etc.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     interval: typing.Optional[str]
     # Overrides the relative time range for individual panels,
     # which causes them to be different than what is selected in
@@ -1452,115 +1406,101 @@
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_from: typing.Optional[str]
     # Overrides the time range for individual panels by shifting its start and end relative to the time picker.
     # For example, you can shift the time range for the panel to be two hours earlier than the dashboard time picker setting `2h`.
     # Note: Panel time overrides have no effect when the dashboard’s time range is absolute.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_shift: typing.Optional[str]
-    # Controls if the timeFrom or timeShift overrides are shown in the panel header
-    hide_time_override: typing.Optional[bool]
     # Dynamically load the panel
     library_panel: typing.Optional['LibraryPanelRef']
-    # Sets panel queries cache timeout.
-    cache_timeout: typing.Optional[str]
-    # Overrides the data source configured time-to-live for a query cache item in milliseconds
-    query_caching_ttl: typing.Optional[float]
     # It depends on the panel plugin. They are specified by the Options field in panel plugin schemas.
-    options: typing.Optional[object]
+    options: object
     # Field options allow you to change how the data is displayed in your visualizations.
-    field_config: typing.Optional['FieldConfigSource']
+    field_config: 'FieldConfigSource'
 
-    def __init__(self, type_val: str = "", id_val: typing.Optional[int] = None, plugin_version: typing.Optional[str] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: typing.Optional[bool] = False, datasource: typing.Optional['DataSourceRef'] = None, grid_pos: typing.Optional['GridPos'] = None, links: typing.Optional[list['DashboardLink']] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, max_per_row: typing.Optional[float] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list['DataTransformerConfig']] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, hide_time_override: typing.Optional[bool] = None, library_panel: typing.Optional['LibraryPanelRef'] = None, cache_timeout: typing.Optional[str] = None, query_caching_ttl: typing.Optional[float] = None, options: typing.Optional[object] = None, field_config: typing.Optional['FieldConfigSource'] = None):
+    def __init__(self, type_val: str = "", id_val: typing.Optional[int] = None, plugin_version: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: bool = False, datasource: typing.Optional['DataSourceRef'] = None, grid_pos: typing.Optional['GridPos'] = None, links: typing.Optional[list['DashboardLink']] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, repeat_panel_id: typing.Optional[int] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list['DataTransformerConfig']] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, library_panel: typing.Optional['LibraryPanelRef'] = None, options: object = None, field_config: typing.Optional['FieldConfigSource'] = None):
         self.type_val = type_val
         self.id_val = id_val
         self.plugin_version = plugin_version
+        self.tags = tags
         self.targets = targets
         self.title = title
         self.description = description
         self.transparent = transparent
         self.datasource = datasource
         self.grid_pos = grid_pos
         self.links = links
         self.repeat = repeat
         self.repeat_direction = repeat_direction if repeat_direction is not None else "h"
-        self.max_per_row = max_per_row
+        self.repeat_panel_id = repeat_panel_id
         self.max_data_points = max_data_points
-        self.transformations = transformations
+        self.transformations = transformations if transformations is not None else []
         self.interval = interval
         self.time_from = time_from
         self.time_shift = time_shift
-        self.hide_time_override = hide_time_override
         self.library_panel = library_panel
-        self.cache_timeout = cache_timeout
-        self.query_caching_ttl = query_caching_ttl
         self.options = options
-        self.field_config = field_config
+        self.field_config = field_config if field_config is not None else FieldConfigSource()
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
+            "transparent": self.transparent,
+            "transformations": self.transformations,
+            "options": self.options,
+            "fieldConfig": self.field_config,
         }
         if self.id_val is not None:
             payload["id"] = self.id_val
         if self.plugin_version is not None:
             payload["pluginVersion"] = self.plugin_version
+        if self.tags is not None:
+            payload["tags"] = self.tags
         if self.targets is not None:
             payload["targets"] = self.targets
         if self.title is not None:
             payload["title"] = self.title
         if self.description is not None:
             payload["description"] = self.description
-        if self.transparent is not None:
-            payload["transparent"] = self.transparent
         if self.datasource is not None:
             payload["datasource"] = self.datasource
         if self.grid_pos is not None:
             payload["gridPos"] = self.grid_pos
         if self.links is not None:
             payload["links"] = self.links
         if self.repeat is not None:
             payload["repeat"] = self.repeat
         if self.repeat_direction is not None:
             payload["repeatDirection"] = self.repeat_direction
-        if self.max_per_row is not None:
-            payload["maxPerRow"] = self.max_per_row
+        if self.repeat_panel_id is not None:
+            payload["repeatPanelId"] = self.repeat_panel_id
         if self.max_data_points is not None:
             payload["maxDataPoints"] = self.max_data_points
-        if self.transformations is not None:
-            payload["transformations"] = self.transformations
         if self.interval is not None:
             payload["interval"] = self.interval
         if self.time_from is not None:
             payload["timeFrom"] = self.time_from
         if self.time_shift is not None:
             payload["timeShift"] = self.time_shift
-        if self.hide_time_override is not None:
-            payload["hideTimeOverride"] = self.hide_time_override
         if self.library_panel is not None:
             payload["libraryPanel"] = self.library_panel
-        if self.cache_timeout is not None:
-            payload["cacheTimeout"] = self.cache_timeout
-        if self.query_caching_ttl is not None:
-            payload["queryCachingTTL"] = self.query_caching_ttl
-        if self.options is not None:
-            payload["options"] = self.options
-        if self.field_config is not None:
-            payload["fieldConfig"] = self.field_config
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "type" in data:
             args["type_val"] = data["type"]
         if "id" in data:
             args["id_val"] = data["id"]
         if "pluginVersion" in data:
             args["plugin_version"] = data["pluginVersion"]
+        if "tags" in data:
+            args["tags"] = data["tags"]
         if "targets" in data:
             args["targets"] = [cogruntime.dataquery_from_json(dataquery_json, data["datasource"]["type"] if data.get("datasource") is not None and data["datasource"].get("type", "") != "" else "") for dataquery_json in data["targets"]]
         if "title" in data:
             args["title"] = data["title"]
         if "description" in data:
             args["description"] = data["description"]
         if "transparent" in data:
@@ -1571,34 +1511,28 @@
             args["grid_pos"] = GridPos.from_json(data["gridPos"])
         if "links" in data:
             args["links"] = data["links"]
         if "repeat" in data:
             args["repeat"] = data["repeat"]
         if "repeatDirection" in data:
             args["repeat_direction"] = data["repeatDirection"]
-        if "maxPerRow" in data:
-            args["max_per_row"] = data["maxPerRow"]
+        if "repeatPanelId" in data:
+            args["repeat_panel_id"] = data["repeatPanelId"]
         if "maxDataPoints" in data:
             args["max_data_points"] = data["maxDataPoints"]
         if "transformations" in data:
             args["transformations"] = data["transformations"]
         if "interval" in data:
             args["interval"] = data["interval"]
         if "timeFrom" in data:
             args["time_from"] = data["timeFrom"]
         if "timeShift" in data:
             args["time_shift"] = data["timeShift"]
-        if "hideTimeOverride" in data:
-            args["hide_time_override"] = data["hideTimeOverride"]
         if "libraryPanel" in data:
             args["library_panel"] = LibraryPanelRef.from_json(data["libraryPanel"])
-        if "cacheTimeout" in data:
-            args["cache_timeout"] = data["cacheTimeout"]
-        if "queryCachingTTL" in data:
-            args["query_caching_ttl"] = data["queryCachingTTL"]
         if "options" in data:
             config = cogruntime.panelcfg_config(data.get("type", ""))
             if config is not None and config.options_from_json_hook is not None:
                 args["options"] = config.options_from_json_hook(data["options"])
             else:
                 args["options"] = data["options"]
         if "fieldConfig" in data:
@@ -1967,14 +1901,116 @@
             args["panels"] = data["panels"]
         if "repeat" in data:
             args["repeat"] = data["repeat"]        
 
         return cls(**args)
 
 
+class GraphPanel:
+    """
+    Support for legacy graph panel.
+    @deprecated this a deprecated panel type
+    """
+
+    type_val: typing.Literal["graph"]
+    # @deprecated this is part of deprecated graph panel
+    legend: typing.Optional['DashboardGraphPanelLegend']
+
+    def __init__(self, legend: typing.Optional['DashboardGraphPanelLegend'] = None):
+        self.type_val = "graph"
+        self.legend = legend
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "type": self.type_val,
+        }
+        if self.legend is not None:
+            payload["legend"] = self.legend
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "legend" in data:
+            args["legend"] = DashboardGraphPanelLegend.from_json(data["legend"])        
+
+        return cls(**args)
+
+
+class HeatmapPanel:
+    """
+    Support for legacy heatmap panel.
+    @deprecated this a deprecated panel type
+    """
+
+    type_val: typing.Literal["heatmap"]
+
+    def __init__(self, ):
+        self.type_val = "heatmap"
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "type": self.type_val,
+        }
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        return cls(**args)
+
+
+class TimePicker:
+    # Whether timepicker is visible or not.
+    hidden: bool
+    # Interval options available in the refresh picker dropdown.
+    refresh_intervals: list[str]
+    # Whether timepicker is collapsed or not. Has no effect on provisioned dashboard.
+    collapse: bool
+    # Whether timepicker is enabled or not. Has no effect on provisioned dashboard.
+    enable: bool
+    # Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
+    time_options: list[str]
+
+    def __init__(self, hidden: bool = False, refresh_intervals: typing.Optional[list[str]] = None, collapse: bool = False, enable: bool = True, time_options: typing.Optional[list[str]] = None):
+        self.hidden = hidden
+        self.refresh_intervals = refresh_intervals if refresh_intervals is not None else ["5s", "10s", "30s", "1m", "5m", "15m", "30m", "1h", "2h", "1d"]
+        self.collapse = collapse
+        self.enable = enable
+        self.time_options = time_options if time_options is not None else ["5m", "15m", "1h", "6h", "12h", "24h", "2d", "7d", "30d"]
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "hidden": self.hidden,
+            "refresh_intervals": self.refresh_intervals,
+            "collapse": self.collapse,
+            "enable": self.enable,
+            "time_options": self.time_options,
+        }
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "hidden" in data:
+            args["hidden"] = data["hidden"]
+        if "refresh_intervals" in data:
+            args["refresh_intervals"] = data["refresh_intervals"]
+        if "collapse" in data:
+            args["collapse"] = data["collapse"]
+        if "enable" in data:
+            args["enable"] = data["enable"]
+        if "time_options" in data:
+            args["time_options"] = data["time_options"]        
+
+        return cls(**args)
+
+
 class DashboardDashboardTime:
     from_val: str
     to: str
 
     def __init__(self, from_val: str = "now-6h", to: str = "now"):
         self.from_val = from_val
         self.to = to
@@ -2138,8 +2174,42 @@
             args["matcher"] = MatcherConfig.from_json(data["matcher"])
         if "properties" in data:
             args["properties"] = data["properties"]        
 
         return cls(**args)
 
 
+class DashboardGraphPanelLegend:
+    show: bool
+    sort: typing.Optional[str]
+    sort_desc: typing.Optional[bool]
+
+    def __init__(self, show: bool = True, sort: typing.Optional[str] = None, sort_desc: typing.Optional[bool] = None):
+        self.show = show
+        self.sort = sort
+        self.sort_desc = sort_desc
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "show": self.show,
+        }
+        if self.sort is not None:
+            payload["sort"] = self.sort
+        if self.sort_desc is not None:
+            payload["sortDesc"] = self.sort_desc
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "show" in data:
+            args["show"] = data["show"]
+        if "sort" in data:
+            args["sort"] = data["sort"]
+        if "sortDesc" in data:
+            args["sort_desc"] = data["sortDesc"]        
+
+        return cls(**args)
+
+
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/dashboardlist.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/dashboardlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,31 +9,28 @@
     include_vars: bool
     show_starred: bool
     show_recently_viewed: bool
     show_search: bool
     show_headings: bool
     max_items: int
     query: str
-    tags: list[str]
-    # folderId is deprecated, and migrated to folderUid on panel init
     folder_id: typing.Optional[int]
-    folder_uid: typing.Optional[str]
+    tags: list[str]
 
-    def __init__(self, keep_time: bool = False, include_vars: bool = False, show_starred: bool = True, show_recently_viewed: bool = False, show_search: bool = False, show_headings: bool = True, max_items: int = 10, query: str = "", tags: typing.Optional[list[str]] = None, folder_id: typing.Optional[int] = None, folder_uid: typing.Optional[str] = None):
+    def __init__(self, keep_time: bool = False, include_vars: bool = False, show_starred: bool = True, show_recently_viewed: bool = False, show_search: bool = False, show_headings: bool = True, max_items: int = 10, query: str = "", folder_id: typing.Optional[int] = None, tags: typing.Optional[list[str]] = None):
         self.keep_time = keep_time
         self.include_vars = include_vars
         self.show_starred = show_starred
         self.show_recently_viewed = show_recently_viewed
         self.show_search = show_search
         self.show_headings = show_headings
         self.max_items = max_items
         self.query = query
-        self.tags = tags if tags is not None else []
         self.folder_id = folder_id
-        self.folder_uid = folder_uid
+        self.tags = tags if tags is not None else []
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "keepTime": self.keep_time,
             "includeVars": self.include_vars,
             "showStarred": self.show_starred,
             "showRecentlyViewed": self.show_recently_viewed,
@@ -41,16 +38,14 @@
             "showHeadings": self.show_headings,
             "maxItems": self.max_items,
             "query": self.query,
             "tags": self.tags,
         }
         if self.folder_id is not None:
             payload["folderId"] = self.folder_id
-        if self.folder_uid is not None:
-            payload["folderUID"] = self.folder_uid
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "keepTime" in data:
@@ -65,20 +60,18 @@
             args["show_search"] = data["showSearch"]
         if "showHeadings" in data:
             args["show_headings"] = data["showHeadings"]
         if "maxItems" in data:
             args["max_items"] = data["maxItems"]
         if "query" in data:
             args["query"] = data["query"]
-        if "tags" in data:
-            args["tags"] = data["tags"]
         if "folderId" in data:
             args["folder_id"] = data["folderId"]
-        if "folderUID" in data:
-            args["folder_uid"] = data["folderUID"]        
+        if "tags" in data:
+            args["tags"] = data["tags"]        
 
         return cls(**args)
 
 
 def variant_config():
     return cogruntime.PanelCfgConfig(
         identifier="dashlist",
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/datagrid.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/debug.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/elasticsearch.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/elasticsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1910,15 +1910,17 @@
     bucket_aggs: typing.Optional[list['BucketAggregation']]
     # List of metric aggregations
     metrics: typing.Optional[list['MetricAggregation']]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/expr.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/expr.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/gauge.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/gauge.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,64 +3,49 @@
 from ..models import common
 import typing
 from ..cog import runtime as cogruntime
 
 
 class Options:
     show_threshold_labels: bool
-    show_threshold_markers: bool
-    sizing: common.BarGaugeSizing
-    min_viz_width: int
     reduce_options: common.ReduceDataOptions
     text: typing.Optional[common.VizTextDisplayOptions]
-    min_viz_height: int
+    show_threshold_markers: bool
     orientation: common.VizOrientation
 
-    def __init__(self, show_threshold_labels: bool = False, show_threshold_markers: bool = True, sizing: typing.Optional[common.BarGaugeSizing] = None, min_viz_width: int = 75, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, min_viz_height: int = 75, orientation: typing.Optional[common.VizOrientation] = None):
+    def __init__(self, show_threshold_labels: bool = False, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, show_threshold_markers: bool = True, orientation: typing.Optional[common.VizOrientation] = None):
         self.show_threshold_labels = show_threshold_labels
-        self.show_threshold_markers = show_threshold_markers
-        self.sizing = sizing if sizing is not None else common.BarGaugeSizing.AUTO
-        self.min_viz_width = min_viz_width
         self.reduce_options = reduce_options if reduce_options is not None else common.ReduceDataOptions()
         self.text = text
-        self.min_viz_height = min_viz_height
+        self.show_threshold_markers = show_threshold_markers
         self.orientation = orientation if orientation is not None else common.VizOrientation.AUTO
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "showThresholdLabels": self.show_threshold_labels,
-            "showThresholdMarkers": self.show_threshold_markers,
-            "sizing": self.sizing,
-            "minVizWidth": self.min_viz_width,
             "reduceOptions": self.reduce_options,
-            "minVizHeight": self.min_viz_height,
+            "showThresholdMarkers": self.show_threshold_markers,
             "orientation": self.orientation,
         }
         if self.text is not None:
             payload["text"] = self.text
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "showThresholdLabels" in data:
             args["show_threshold_labels"] = data["showThresholdLabels"]
-        if "showThresholdMarkers" in data:
-            args["show_threshold_markers"] = data["showThresholdMarkers"]
-        if "sizing" in data:
-            args["sizing"] = data["sizing"]
-        if "minVizWidth" in data:
-            args["min_viz_width"] = data["minVizWidth"]
         if "reduceOptions" in data:
             args["reduce_options"] = common.ReduceDataOptions.from_json(data["reduceOptions"])
         if "text" in data:
             args["text"] = common.VizTextDisplayOptions.from_json(data["text"])
-        if "minVizHeight" in data:
-            args["min_viz_height"] = data["minVizHeight"]
+        if "showThresholdMarkers" in data:
+            args["show_threshold_markers"] = data["showThresholdMarkers"]
         if "orientation" in data:
             args["orientation"] = data["orientation"]        
 
         return cls(**args)
 
 
 def variant_config():
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/geomap.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/googlecloudmonitoring.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/googlecloudmonitoring.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 
 
 class CloudMonitoringQuery(cogvariants.Dataquery):
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # Aliases can be set to modify the legend labels. e.g. {{metric.label.xxx}}. See docs for more detail.
     alias_by: typing.Optional[str]
     # GCM query type.
     # queryType: #QueryType
     # Time Series List sub-query properties.
     time_series_list: typing.Optional['TimeSeriesList']
     # Time Series sub-query properties.
     time_series_query: typing.Optional['TimeSeriesQuery']
     # SLO sub-query properties.
     slo_query: typing.Optional['SLOQuery']
-    # PromQL sub-query properties.
-    prom_ql_query: typing.Optional['PromQLQuery']
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
     # Time interval in milliseconds.
     interval_ms: typing.Optional[float]
 
-    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, alias_by: typing.Optional[str] = None, time_series_list: typing.Optional['TimeSeriesList'] = None, time_series_query: typing.Optional['TimeSeriesQuery'] = None, slo_query: typing.Optional['SLOQuery'] = None, prom_ql_query: typing.Optional['PromQLQuery'] = None, datasource: typing.Optional[object] = None, interval_ms: typing.Optional[float] = None):
+    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, alias_by: typing.Optional[str] = None, time_series_list: typing.Optional['TimeSeriesList'] = None, time_series_query: typing.Optional['TimeSeriesQuery'] = None, slo_query: typing.Optional['SLOQuery'] = None, datasource: typing.Optional[object] = None, interval_ms: typing.Optional[float] = None):
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.alias_by = alias_by
         self.time_series_list = time_series_list
         self.time_series_query = time_series_query
         self.slo_query = slo_query
-        self.prom_ql_query = prom_ql_query
         self.datasource = datasource
         self.interval_ms = interval_ms
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "refId": self.ref_id,
         }
@@ -60,16 +59,14 @@
             payload["aliasBy"] = self.alias_by
         if self.time_series_list is not None:
             payload["timeSeriesList"] = self.time_series_list
         if self.time_series_query is not None:
             payload["timeSeriesQuery"] = self.time_series_query
         if self.slo_query is not None:
             payload["sloQuery"] = self.slo_query
-        if self.prom_ql_query is not None:
-            payload["promQLQuery"] = self.prom_ql_query
         if self.datasource is not None:
             payload["datasource"] = self.datasource
         if self.interval_ms is not None:
             payload["intervalMs"] = self.interval_ms
         return payload
 
     @classmethod
@@ -86,16 +83,14 @@
             args["alias_by"] = data["aliasBy"]
         if "timeSeriesList" in data:
             args["time_series_list"] = TimeSeriesList.from_json(data["timeSeriesList"])
         if "timeSeriesQuery" in data:
             args["time_series_query"] = TimeSeriesQuery.from_json(data["timeSeriesQuery"])
         if "sloQuery" in data:
             args["slo_query"] = SLOQuery.from_json(data["sloQuery"])
-        if "promQLQuery" in data:
-            args["prom_ql_query"] = PromQLQuery.from_json(data["promQLQuery"])
         if "datasource" in data:
             args["datasource"] = data["datasource"]
         if "intervalMs" in data:
             args["interval_ms"] = data["intervalMs"]        
 
         return cls(**args)
 
@@ -112,15 +107,14 @@
     Defines the supported queryTypes.
     """
 
     TIME_SERIES_LIST = "timeSeriesList"
     TIME_SERIES_QUERY = "timeSeriesQuery"
     SLO = "slo"
     ANNOTATION = "annotation"
-    PROMQL = "promQL"
 
 
 class TimeSeriesList:
     """
     Time Series List sub-query properties.
     """
 
@@ -134,44 +128,44 @@
     per_series_aligner: typing.Optional[str]
     # Array of labels to group data by.
     group_bys: typing.Optional[list[str]]
     # Array of filters to query data by. Labels that can be filtered on are defined by the metric.
     filters: typing.Optional[list[str]]
     # Data view, defaults to FULL.
     view: typing.Optional[str]
-    # Annotation title.
-    title: typing.Optional[str]
-    # Annotation text.
-    text: typing.Optional[str]
     # Only present if a preprocessor is selected. Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
     secondary_cross_series_reducer: typing.Optional[str]
     # Only present if a preprocessor is selected. Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
     secondary_alignment_period: typing.Optional[str]
     # Only present if a preprocessor is selected. Alignment function to be used. Defaults to ALIGN_MEAN.
     secondary_per_series_aligner: typing.Optional[str]
     # Only present if a preprocessor is selected. Array of labels to group data by.
     secondary_group_bys: typing.Optional[list[str]]
     # Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
     preprocessor: typing.Optional['PreprocessorType']
+    # Annotation title.
+    title: typing.Optional[str]
+    # Annotation text.
+    text: typing.Optional[str]
 
-    def __init__(self, project_name: str = "", cross_series_reducer: str = "", alignment_period: typing.Optional[str] = None, per_series_aligner: typing.Optional[str] = None, group_bys: typing.Optional[list[str]] = None, filters: typing.Optional[list[str]] = None, view: typing.Optional[str] = None, title: typing.Optional[str] = None, text: typing.Optional[str] = None, secondary_cross_series_reducer: typing.Optional[str] = None, secondary_alignment_period: typing.Optional[str] = None, secondary_per_series_aligner: typing.Optional[str] = None, secondary_group_bys: typing.Optional[list[str]] = None, preprocessor: typing.Optional['PreprocessorType'] = None):
+    def __init__(self, project_name: str = "", cross_series_reducer: str = "", alignment_period: typing.Optional[str] = None, per_series_aligner: typing.Optional[str] = None, group_bys: typing.Optional[list[str]] = None, filters: typing.Optional[list[str]] = None, view: typing.Optional[str] = None, secondary_cross_series_reducer: typing.Optional[str] = None, secondary_alignment_period: typing.Optional[str] = None, secondary_per_series_aligner: typing.Optional[str] = None, secondary_group_bys: typing.Optional[list[str]] = None, preprocessor: typing.Optional['PreprocessorType'] = None, title: typing.Optional[str] = None, text: typing.Optional[str] = None):
         self.project_name = project_name
         self.cross_series_reducer = cross_series_reducer
         self.alignment_period = alignment_period
         self.per_series_aligner = per_series_aligner
         self.group_bys = group_bys
         self.filters = filters
         self.view = view
-        self.title = title
-        self.text = text
         self.secondary_cross_series_reducer = secondary_cross_series_reducer
         self.secondary_alignment_period = secondary_alignment_period
         self.secondary_per_series_aligner = secondary_per_series_aligner
         self.secondary_group_bys = secondary_group_bys
         self.preprocessor = preprocessor
+        self.title = title
+        self.text = text
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "projectName": self.project_name,
             "crossSeriesReducer": self.cross_series_reducer,
         }
         if self.alignment_period is not None:
@@ -180,28 +174,28 @@
             payload["perSeriesAligner"] = self.per_series_aligner
         if self.group_bys is not None:
             payload["groupBys"] = self.group_bys
         if self.filters is not None:
             payload["filters"] = self.filters
         if self.view is not None:
             payload["view"] = self.view
-        if self.title is not None:
-            payload["title"] = self.title
-        if self.text is not None:
-            payload["text"] = self.text
         if self.secondary_cross_series_reducer is not None:
             payload["secondaryCrossSeriesReducer"] = self.secondary_cross_series_reducer
         if self.secondary_alignment_period is not None:
             payload["secondaryAlignmentPeriod"] = self.secondary_alignment_period
         if self.secondary_per_series_aligner is not None:
             payload["secondaryPerSeriesAligner"] = self.secondary_per_series_aligner
         if self.secondary_group_bys is not None:
             payload["secondaryGroupBys"] = self.secondary_group_bys
         if self.preprocessor is not None:
             payload["preprocessor"] = self.preprocessor
+        if self.title is not None:
+            payload["title"] = self.title
+        if self.text is not None:
+            payload["text"] = self.text
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "projectName" in data:
@@ -214,42 +208,159 @@
             args["per_series_aligner"] = data["perSeriesAligner"]
         if "groupBys" in data:
             args["group_bys"] = data["groupBys"]
         if "filters" in data:
             args["filters"] = data["filters"]
         if "view" in data:
             args["view"] = data["view"]
-        if "title" in data:
-            args["title"] = data["title"]
-        if "text" in data:
-            args["text"] = data["text"]
         if "secondaryCrossSeriesReducer" in data:
             args["secondary_cross_series_reducer"] = data["secondaryCrossSeriesReducer"]
         if "secondaryAlignmentPeriod" in data:
             args["secondary_alignment_period"] = data["secondaryAlignmentPeriod"]
         if "secondaryPerSeriesAligner" in data:
             args["secondary_per_series_aligner"] = data["secondaryPerSeriesAligner"]
         if "secondaryGroupBys" in data:
             args["secondary_group_bys"] = data["secondaryGroupBys"]
         if "preprocessor" in data:
-            args["preprocessor"] = data["preprocessor"]        
+            args["preprocessor"] = data["preprocessor"]
+        if "title" in data:
+            args["title"] = data["title"]
+        if "text" in data:
+            args["text"] = data["text"]        
 
         return cls(**args)
 
 
 class PreprocessorType(enum.StrEnum):
     """
     Types of pre-processor available. Defined by the metric.
     """
 
     NONE = "none"
     RATE = "rate"
     DELTA = "delta"
 
 
+class AnnotationQuery:
+    """
+    Annotation sub-query properties.
+    """
+
+    # GCP project to execute the query against.
+    project_name: str
+    # Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
+    cross_series_reducer: str
+    # Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
+    alignment_period: typing.Optional[str]
+    # Alignment function to be used. Defaults to ALIGN_MEAN.
+    per_series_aligner: typing.Optional[str]
+    # Array of labels to group data by.
+    group_bys: typing.Optional[list[str]]
+    # Array of filters to query data by. Labels that can be filtered on are defined by the metric.
+    filters: typing.Optional[list[str]]
+    # Data view, defaults to FULL.
+    view: typing.Optional[str]
+    # Only present if a preprocessor is selected. Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
+    secondary_cross_series_reducer: typing.Optional[str]
+    # Only present if a preprocessor is selected. Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
+    secondary_alignment_period: typing.Optional[str]
+    # Only present if a preprocessor is selected. Alignment function to be used. Defaults to ALIGN_MEAN.
+    secondary_per_series_aligner: typing.Optional[str]
+    # Only present if a preprocessor is selected. Array of labels to group data by.
+    secondary_group_bys: typing.Optional[list[str]]
+    # Annotation title.
+    title: typing.Optional[str]
+    # Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
+    preprocessor: typing.Optional['PreprocessorType']
+    # Annotation text.
+    text: typing.Optional[str]
+
+    def __init__(self, project_name: str = "", cross_series_reducer: str = "", alignment_period: typing.Optional[str] = None, per_series_aligner: typing.Optional[str] = None, group_bys: typing.Optional[list[str]] = None, filters: typing.Optional[list[str]] = None, view: typing.Optional[str] = None, secondary_cross_series_reducer: typing.Optional[str] = None, secondary_alignment_period: typing.Optional[str] = None, secondary_per_series_aligner: typing.Optional[str] = None, secondary_group_bys: typing.Optional[list[str]] = None, title: typing.Optional[str] = None, preprocessor: typing.Optional['PreprocessorType'] = None, text: typing.Optional[str] = None):
+        self.project_name = project_name
+        self.cross_series_reducer = cross_series_reducer
+        self.alignment_period = alignment_period
+        self.per_series_aligner = per_series_aligner
+        self.group_bys = group_bys
+        self.filters = filters
+        self.view = view
+        self.secondary_cross_series_reducer = secondary_cross_series_reducer
+        self.secondary_alignment_period = secondary_alignment_period
+        self.secondary_per_series_aligner = secondary_per_series_aligner
+        self.secondary_group_bys = secondary_group_bys
+        self.title = title
+        self.preprocessor = preprocessor
+        self.text = text
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "projectName": self.project_name,
+            "crossSeriesReducer": self.cross_series_reducer,
+        }
+        if self.alignment_period is not None:
+            payload["alignmentPeriod"] = self.alignment_period
+        if self.per_series_aligner is not None:
+            payload["perSeriesAligner"] = self.per_series_aligner
+        if self.group_bys is not None:
+            payload["groupBys"] = self.group_bys
+        if self.filters is not None:
+            payload["filters"] = self.filters
+        if self.view is not None:
+            payload["view"] = self.view
+        if self.secondary_cross_series_reducer is not None:
+            payload["secondaryCrossSeriesReducer"] = self.secondary_cross_series_reducer
+        if self.secondary_alignment_period is not None:
+            payload["secondaryAlignmentPeriod"] = self.secondary_alignment_period
+        if self.secondary_per_series_aligner is not None:
+            payload["secondaryPerSeriesAligner"] = self.secondary_per_series_aligner
+        if self.secondary_group_bys is not None:
+            payload["secondaryGroupBys"] = self.secondary_group_bys
+        if self.title is not None:
+            payload["title"] = self.title
+        if self.preprocessor is not None:
+            payload["preprocessor"] = self.preprocessor
+        if self.text is not None:
+            payload["text"] = self.text
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "projectName" in data:
+            args["project_name"] = data["projectName"]
+        if "crossSeriesReducer" in data:
+            args["cross_series_reducer"] = data["crossSeriesReducer"]
+        if "alignmentPeriod" in data:
+            args["alignment_period"] = data["alignmentPeriod"]
+        if "perSeriesAligner" in data:
+            args["per_series_aligner"] = data["perSeriesAligner"]
+        if "groupBys" in data:
+            args["group_bys"] = data["groupBys"]
+        if "filters" in data:
+            args["filters"] = data["filters"]
+        if "view" in data:
+            args["view"] = data["view"]
+        if "secondaryCrossSeriesReducer" in data:
+            args["secondary_cross_series_reducer"] = data["secondaryCrossSeriesReducer"]
+        if "secondaryAlignmentPeriod" in data:
+            args["secondary_alignment_period"] = data["secondaryAlignmentPeriod"]
+        if "secondaryPerSeriesAligner" in data:
+            args["secondary_per_series_aligner"] = data["secondaryPerSeriesAligner"]
+        if "secondaryGroupBys" in data:
+            args["secondary_group_bys"] = data["secondaryGroupBys"]
+        if "title" in data:
+            args["title"] = data["title"]
+        if "preprocessor" in data:
+            args["preprocessor"] = data["preprocessor"]
+        if "text" in data:
+            args["text"] = data["text"]        
+
+        return cls(**args)
+
+
 class TimeSeriesQuery:
     """
     Time Series sub-query properties.
     """
 
     # GCP project to execute the query against.
     project_name: str
@@ -367,53 +478,14 @@
             args["goal"] = data["goal"]
         if "lookbackPeriod" in data:
             args["lookback_period"] = data["lookbackPeriod"]        
 
         return cls(**args)
 
 
-class PromQLQuery:
-    """
-    PromQL sub-query properties.
-    """
-
-    # GCP project to execute the query against.
-    project_name: str
-    # PromQL expression/query to be executed.
-    expr: str
-    # PromQL min step
-    step: str
-
-    def __init__(self, project_name: str = "", expr: str = "", step: str = ""):
-        self.project_name = project_name
-        self.expr = expr
-        self.step = step
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "projectName": self.project_name,
-            "expr": self.expr,
-            "step": self.step,
-        }
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "projectName" in data:
-            args["project_name"] = data["projectName"]
-        if "expr" in data:
-            args["expr"] = data["expr"]
-        if "step" in data:
-            args["step"] = data["step"]        
-
-        return cls(**args)
-
-
 class MetricQuery:
     """
     @deprecated This type is for migration purposes only. Replaced by TimeSeriesList Metric sub-query properties.
     """
 
     # GCP project to execute the query against.
     project_name: str
@@ -563,15 +635,15 @@
     ALIGN_PERCENTILE_05 = "ALIGN_PERCENTILE_05"
     ALIGN_PERCENT_CHANGE = "ALIGN_PERCENT_CHANGE"
     ALIGN_NONE = "ALIGN_NONE"
 
 
 class LegacyCloudMonitoringAnnotationQuery:
     """
-    @deprecated Use TimeSeriesList instead. Legacy annotation query properties for migration purposes.
+    @deprecated Use AnnotationQuery instead. Legacy annotation query properties for migration purposes.
     """
 
     # GCP project to execute the query against.
     project_name: str
     metric_type: str
     # Query refId.
     ref_id: str
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/grafanapyroscope.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/grafanapyroscope.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,64 +2,61 @@
 
 import enum
 from ..cog import variants as cogvariants
 import typing
 from ..cog import runtime as cogruntime
 
 
-class PyroscopeQueryType(enum.StrEnum):
+class PhlareQueryType(enum.StrEnum):
     METRICS = "metrics"
     PROFILE = "profile"
     BOTH = "both"
 
 
 class Dataquery(cogvariants.Dataquery):
     # Specifies the query label selectors.
     label_selector: typing.Optional[str]
-    # Specifies the query span selectors.
-    span_selector: typing.Optional[list[str]]
     # Specifies the type of profile to query.
     profile_type_id: typing.Optional[str]
     # Allows to group the results.
     group_by: typing.Optional[list[str]]
     # Sets the maximum number of nodes in the flamegraph.
     max_nodes: typing.Optional[int]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
 
-    def __init__(self, label_selector: typing.Optional[str] = "{}", span_selector: typing.Optional[list[str]] = None, profile_type_id: typing.Optional[str] = None, group_by: typing.Optional[list[str]] = None, max_nodes: typing.Optional[int] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
+    def __init__(self, label_selector: typing.Optional[str] = "{}", profile_type_id: typing.Optional[str] = None, group_by: typing.Optional[list[str]] = None, max_nodes: typing.Optional[int] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
         self.label_selector = label_selector
-        self.span_selector = span_selector
         self.profile_type_id = profile_type_id
         self.group_by = group_by
         self.max_nodes = max_nodes
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.datasource = datasource
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.label_selector is not None:
             payload["labelSelector"] = self.label_selector
-        if self.span_selector is not None:
-            payload["spanSelector"] = self.span_selector
         if self.profile_type_id is not None:
             payload["profileTypeId"] = self.profile_type_id
         if self.group_by is not None:
             payload["groupBy"] = self.group_by
         if self.max_nodes is not None:
             payload["maxNodes"] = self.max_nodes
         if self.ref_id is not None:
@@ -74,16 +71,14 @@
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "labelSelector" in data:
             args["label_selector"] = data["labelSelector"]
-        if "spanSelector" in data:
-            args["span_selector"] = data["spanSelector"]
         if "profileTypeId" in data:
             args["profile_type_id"] = data["profileTypeId"]
         if "groupBy" in data:
             args["group_by"] = data["groupBy"]
         if "maxNodes" in data:
             args["max_nodes"] = data["maxNodes"]
         if "refId" in data:
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/heatmap.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/heatmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,35 +120,33 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
-    axis_centered_zero: typing.Optional[bool]
     # Sets the maximum value for the yAxis
     max_val: typing.Optional[float]
-    axis_border_show: typing.Optional[bool]
+    axis_centered_zero: typing.Optional[bool]
 
-    def __init__(self, unit: typing.Optional[str] = None, reverse: typing.Optional[bool] = None, decimals: typing.Optional[float] = None, min_val: typing.Optional[float] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, max_val: typing.Optional[float] = None, axis_border_show: typing.Optional[bool] = None):
+    def __init__(self, unit: typing.Optional[str] = None, reverse: typing.Optional[bool] = None, decimals: typing.Optional[float] = None, min_val: typing.Optional[float] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, max_val: typing.Optional[float] = None, axis_centered_zero: typing.Optional[bool] = None):
         self.unit = unit
         self.reverse = reverse
         self.decimals = decimals
         self.min_val = min_val
         self.axis_placement = axis_placement
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
-        self.axis_centered_zero = axis_centered_zero
         self.max_val = max_val
-        self.axis_border_show = axis_border_show
+        self.axis_centered_zero = axis_centered_zero
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.unit is not None:
             payload["unit"] = self.unit
         if self.reverse is not None:
@@ -169,20 +167,18 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.max_val is not None:
             payload["max"] = self.max_val
-        if self.axis_border_show is not None:
-            payload["axisBorderShow"] = self.axis_border_show
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "unit" in data:
@@ -205,20 +201,18 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "max" in data:
             args["max_val"] = data["max"]
-        if "axisBorderShow" in data:
-            args["axis_border_show"] = data["axisBorderShow"]        
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]        
 
         return cls(**args)
 
 
 class CellValues:
     """
     Controls cell value options
@@ -290,58 +284,39 @@
 
 
 class HeatmapTooltip:
     """
     Controls tooltip options
     """
 
-    # Controls how the tooltip is shown
-    mode: common.TooltipDisplayMode
-    max_height: typing.Optional[float]
-    max_width: typing.Optional[float]
+    # Controls if the tooltip is shown
+    show: bool
     # Controls if the tooltip shows a histogram of the y-axis values
     y_histogram: typing.Optional[bool]
-    # Controls if the tooltip shows a color scale in header
-    show_color_scale: typing.Optional[bool]
 
-    def __init__(self, mode: typing.Optional[common.TooltipDisplayMode] = None, max_height: typing.Optional[float] = None, max_width: typing.Optional[float] = None, y_histogram: typing.Optional[bool] = None, show_color_scale: typing.Optional[bool] = None):
-        self.mode = mode if mode is not None else common.TooltipDisplayMode.SINGLE
-        self.max_height = max_height
-        self.max_width = max_width
+    def __init__(self, show: bool = False, y_histogram: typing.Optional[bool] = None):
+        self.show = show
         self.y_histogram = y_histogram
-        self.show_color_scale = show_color_scale
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "mode": self.mode,
+            "show": self.show,
         }
-        if self.max_height is not None:
-            payload["maxHeight"] = self.max_height
-        if self.max_width is not None:
-            payload["maxWidth"] = self.max_width
         if self.y_histogram is not None:
             payload["yHistogram"] = self.y_histogram
-        if self.show_color_scale is not None:
-            payload["showColorScale"] = self.show_color_scale
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "mode" in data:
-            args["mode"] = data["mode"]
-        if "maxHeight" in data:
-            args["max_height"] = data["maxHeight"]
-        if "maxWidth" in data:
-            args["max_width"] = data["maxWidth"]
+        if "show" in data:
+            args["show"] = data["show"]
         if "yHistogram" in data:
-            args["y_histogram"] = data["yHistogram"]
-        if "showColorScale" in data:
-            args["show_color_scale"] = data["showColorScale"]        
+            args["y_histogram"] = data["yHistogram"]        
 
         return cls(**args)
 
 
 class HeatmapLegend:
     """
     Controls legend options
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/histogram.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/histogram.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,54 +2,47 @@
 
 import typing
 from ..models import common
 from ..cog import runtime as cogruntime
 
 
 class Options:
-    # Bucket count (approx)
-    bucket_count: typing.Optional[int]
     # Size of each bucket
     bucket_size: typing.Optional[int]
     # Offset buckets by this amount
-    bucket_offset: typing.Optional[float]
+    bucket_offset: typing.Optional[int]
     legend: common.VizLegendOptions
     tooltip: common.VizTooltipOptions
     # Combines multiple series into a single histogram
     combine: typing.Optional[bool]
 
-    def __init__(self, bucket_count: typing.Optional[int] = 30, bucket_size: typing.Optional[int] = None, bucket_offset: typing.Optional[float] = 0, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, combine: typing.Optional[bool] = None):
-        self.bucket_count = bucket_count
+    def __init__(self, bucket_size: typing.Optional[int] = None, bucket_offset: typing.Optional[int] = 0, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, combine: typing.Optional[bool] = None):
         self.bucket_size = bucket_size
         self.bucket_offset = bucket_offset
         self.legend = legend if legend is not None else common.VizLegendOptions()
         self.tooltip = tooltip if tooltip is not None else common.VizTooltipOptions()
         self.combine = combine
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "legend": self.legend,
             "tooltip": self.tooltip,
         }
-        if self.bucket_count is not None:
-            payload["bucketCount"] = self.bucket_count
         if self.bucket_size is not None:
             payload["bucketSize"] = self.bucket_size
         if self.bucket_offset is not None:
             payload["bucketOffset"] = self.bucket_offset
         if self.combine is not None:
             payload["combine"] = self.combine
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "bucketCount" in data:
-            args["bucket_count"] = data["bucketCount"]
         if "bucketSize" in data:
             args["bucket_size"] = data["bucketSize"]
         if "bucketOffset" in data:
             args["bucket_offset"] = data["bucketOffset"]
         if "legend" in data:
             args["legend"] = common.VizLegendOptions.from_json(data["legend"])
         if "tooltip" in data:
@@ -69,38 +62,34 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
-    axis_centered_zero: typing.Optional[bool]
     hide_from: typing.Optional[common.HideSeriesConfig]
-    stacking: typing.Optional[common.StackingConfig]
     # Set the mode of the gradient fill. Fill gradient is based on the line color. To change the color, use the standard color scheme field option.
     # Gradient appearance is influenced by the Fill opacity setting.
     gradient_mode: typing.Optional[common.GraphGradientMode]
-    axis_border_show: typing.Optional[bool]
+    axis_centered_zero: typing.Optional[bool]
 
-    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, stacking: typing.Optional[common.StackingConfig] = None, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_border_show: typing.Optional[bool] = None):
+    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_centered_zero: typing.Optional[bool] = None):
         self.line_width = line_width
         self.fill_opacity = fill_opacity
         self.axis_placement = axis_placement
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
-        self.axis_centered_zero = axis_centered_zero
         self.hide_from = hide_from
-        self.stacking = stacking
         self.gradient_mode = gradient_mode if gradient_mode is not None else common.GraphGradientMode.NONE
-        self.axis_border_show = axis_border_show
+        self.axis_centered_zero = axis_centered_zero
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.line_width is not None:
             payload["lineWidth"] = self.line_width
         if self.fill_opacity is not None:
@@ -117,24 +106,20 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.hide_from is not None:
             payload["hideFrom"] = self.hide_from
-        if self.stacking is not None:
-            payload["stacking"] = self.stacking
         if self.gradient_mode is not None:
             payload["gradientMode"] = self.gradient_mode
-        if self.axis_border_show is not None:
-            payload["axisBorderShow"] = self.axis_border_show
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "lineWidth" in data:
@@ -153,24 +138,20 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "hideFrom" in data:
             args["hide_from"] = common.HideSeriesConfig.from_json(data["hideFrom"])
-        if "stacking" in data:
-            args["stacking"] = common.StackingConfig.from_json(data["stacking"])
         if "gradientMode" in data:
             args["gradient_mode"] = data["gradientMode"]
-        if "axisBorderShow" in data:
-            args["axis_border_show"] = data["axisBorderShow"]        
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/librarypanel.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/librarypanel.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,40 +167,41 @@
 
 
 class LibrarypanelLibraryPanelModel:
     # The panel plugin type id. This is used to find the plugin to display the panel.
     type_val: str
     # The version of the plugin that is used for this panel. This is used to find the plugin to display the panel and to migrate old panel configs.
     plugin_version: typing.Optional[str]
+    # Tags for the panel.
+    tags: typing.Optional[list[str]]
     # Depends on the panel plugin. See the plugin documentation for details.
     targets: typing.Optional[list[cogvariants.Dataquery]]
     # Panel title.
     title: typing.Optional[str]
     # Panel description.
     description: typing.Optional[str]
     # Whether to display the panel without a background.
-    transparent: typing.Optional[bool]
+    transparent: bool
     # The datasource used in all targets.
     datasource: typing.Optional[dashboard.DataSourceRef]
     # Panel links.
     links: typing.Optional[list[dashboard.DashboardLink]]
     # Name of template variable to repeat for.
     repeat: typing.Optional[str]
     # Direction to repeat in if 'repeat' is set.
     # `h` for horizontal, `v` for vertical.
     repeat_direction: typing.Optional[typing.Literal["h", "v"]]
-    # Option for repeated panels that controls max items per row
-    # Only relevant for horizontally repeated panels
-    max_per_row: typing.Optional[float]
+    # Id of the repeating panel.
+    repeat_panel_id: typing.Optional[int]
     # The maximum number of data points that the panel queries are retrieving.
     max_data_points: typing.Optional[float]
     # List of transformations that are applied to the panel data before rendering.
     # When there are multiple transformations, Grafana applies them in the order they are listed.
     # Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
-    transformations: typing.Optional[list[dashboard.DataTransformerConfig]]
+    transformations: list[dashboard.DataTransformerConfig]
     # The min time interval setting defines a lower limit for the $__interval and $__interval_ms variables.
     # This value must be formatted as a number followed by a valid time
     # identifier like: "40s", "3d", etc.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     interval: typing.Optional[str]
     # Overrides the relative time range for individual panels,
     # which causes them to be different than what is selected in
@@ -212,102 +213,88 @@
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_from: typing.Optional[str]
     # Overrides the time range for individual panels by shifting its start and end relative to the time picker.
     # For example, you can shift the time range for the panel to be two hours earlier than the dashboard time picker setting `2h`.
     # Note: Panel time overrides have no effect when the dashboard’s time range is absolute.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_shift: typing.Optional[str]
-    # Controls if the timeFrom or timeShift overrides are shown in the panel header
-    hide_time_override: typing.Optional[bool]
-    # Sets panel queries cache timeout.
-    cache_timeout: typing.Optional[str]
-    # Overrides the data source configured time-to-live for a query cache item in milliseconds
-    query_caching_ttl: typing.Optional[float]
     # It depends on the panel plugin. They are specified by the Options field in panel plugin schemas.
-    options: typing.Optional[object]
+    options: object
     # Field options allow you to change how the data is displayed in your visualizations.
-    field_config: typing.Optional[dashboard.FieldConfigSource]
+    field_config: dashboard.FieldConfigSource
 
-    def __init__(self, type_val: str = "", plugin_version: typing.Optional[str] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: typing.Optional[bool] = False, datasource: typing.Optional[dashboard.DataSourceRef] = None, links: typing.Optional[list[dashboard.DashboardLink]] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, max_per_row: typing.Optional[float] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list[dashboard.DataTransformerConfig]] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, hide_time_override: typing.Optional[bool] = None, cache_timeout: typing.Optional[str] = None, query_caching_ttl: typing.Optional[float] = None, options: typing.Optional[object] = None, field_config: typing.Optional[dashboard.FieldConfigSource] = None):
+    def __init__(self, type_val: str = "", plugin_version: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: bool = False, datasource: typing.Optional[dashboard.DataSourceRef] = None, links: typing.Optional[list[dashboard.DashboardLink]] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, repeat_panel_id: typing.Optional[int] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list[dashboard.DataTransformerConfig]] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, options: object = None, field_config: typing.Optional[dashboard.FieldConfigSource] = None):
         self.type_val = type_val
         self.plugin_version = plugin_version
+        self.tags = tags
         self.targets = targets
         self.title = title
         self.description = description
         self.transparent = transparent
         self.datasource = datasource
         self.links = links
         self.repeat = repeat
         self.repeat_direction = repeat_direction if repeat_direction is not None else "h"
-        self.max_per_row = max_per_row
+        self.repeat_panel_id = repeat_panel_id
         self.max_data_points = max_data_points
-        self.transformations = transformations
+        self.transformations = transformations if transformations is not None else []
         self.interval = interval
         self.time_from = time_from
         self.time_shift = time_shift
-        self.hide_time_override = hide_time_override
-        self.cache_timeout = cache_timeout
-        self.query_caching_ttl = query_caching_ttl
         self.options = options
-        self.field_config = field_config
+        self.field_config = field_config if field_config is not None else dashboard.FieldConfigSource()
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
+            "transparent": self.transparent,
+            "transformations": self.transformations,
+            "options": self.options,
+            "fieldConfig": self.field_config,
         }
         if self.plugin_version is not None:
             payload["pluginVersion"] = self.plugin_version
+        if self.tags is not None:
+            payload["tags"] = self.tags
         if self.targets is not None:
             payload["targets"] = self.targets
         if self.title is not None:
             payload["title"] = self.title
         if self.description is not None:
             payload["description"] = self.description
-        if self.transparent is not None:
-            payload["transparent"] = self.transparent
         if self.datasource is not None:
             payload["datasource"] = self.datasource
         if self.links is not None:
             payload["links"] = self.links
         if self.repeat is not None:
             payload["repeat"] = self.repeat
         if self.repeat_direction is not None:
             payload["repeatDirection"] = self.repeat_direction
-        if self.max_per_row is not None:
-            payload["maxPerRow"] = self.max_per_row
+        if self.repeat_panel_id is not None:
+            payload["repeatPanelId"] = self.repeat_panel_id
         if self.max_data_points is not None:
             payload["maxDataPoints"] = self.max_data_points
-        if self.transformations is not None:
-            payload["transformations"] = self.transformations
         if self.interval is not None:
             payload["interval"] = self.interval
         if self.time_from is not None:
             payload["timeFrom"] = self.time_from
         if self.time_shift is not None:
             payload["timeShift"] = self.time_shift
-        if self.hide_time_override is not None:
-            payload["hideTimeOverride"] = self.hide_time_override
-        if self.cache_timeout is not None:
-            payload["cacheTimeout"] = self.cache_timeout
-        if self.query_caching_ttl is not None:
-            payload["queryCachingTTL"] = self.query_caching_ttl
-        if self.options is not None:
-            payload["options"] = self.options
-        if self.field_config is not None:
-            payload["fieldConfig"] = self.field_config
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "type" in data:
             args["type_val"] = data["type"]
         if "pluginVersion" in data:
             args["plugin_version"] = data["pluginVersion"]
+        if "tags" in data:
+            args["tags"] = data["tags"]
         if "targets" in data:
             args["targets"] = [cogruntime.dataquery_from_json(dataquery_json, data["datasource"]["type"] if data.get("datasource") is not None and data["datasource"].get("type", "") != "" else "") for dataquery_json in data["targets"]]
         if "title" in data:
             args["title"] = data["title"]
         if "description" in data:
             args["description"] = data["description"]
         if "transparent" in data:
@@ -316,32 +303,26 @@
             args["datasource"] = dashboard.DataSourceRef.from_json(data["datasource"])
         if "links" in data:
             args["links"] = data["links"]
         if "repeat" in data:
             args["repeat"] = data["repeat"]
         if "repeatDirection" in data:
             args["repeat_direction"] = data["repeatDirection"]
-        if "maxPerRow" in data:
-            args["max_per_row"] = data["maxPerRow"]
+        if "repeatPanelId" in data:
+            args["repeat_panel_id"] = data["repeatPanelId"]
         if "maxDataPoints" in data:
             args["max_data_points"] = data["maxDataPoints"]
         if "transformations" in data:
             args["transformations"] = data["transformations"]
         if "interval" in data:
             args["interval"] = data["interval"]
         if "timeFrom" in data:
             args["time_from"] = data["timeFrom"]
         if "timeShift" in data:
             args["time_shift"] = data["timeShift"]
-        if "hideTimeOverride" in data:
-            args["hide_time_override"] = data["hideTimeOverride"]
-        if "cacheTimeout" in data:
-            args["cache_timeout"] = data["cacheTimeout"]
-        if "queryCachingTTL" in data:
-            args["query_caching_ttl"] = data["queryCachingTTL"]
         if "options" in data:
             args["options"] = data["options"]
         if "fieldConfig" in data:
             args["field_config"] = dashboard.FieldConfigSource.from_json(data["fieldConfig"])        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/logs.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/logs.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,38 +5,35 @@
 from ..cog import runtime as cogruntime
 
 
 class Options:
     show_labels: bool
     show_common_labels: bool
     show_time: bool
-    show_log_context_toggle: bool
     wrap_log_message: bool
     prettify_log_message: bool
     enable_log_details: bool
     sort_order: common.LogsSortOrder
     dedup_strategy: common.LogsDedupStrategy
 
-    def __init__(self, show_labels: bool = False, show_common_labels: bool = False, show_time: bool = False, show_log_context_toggle: bool = False, wrap_log_message: bool = False, prettify_log_message: bool = False, enable_log_details: bool = False, sort_order: typing.Optional[common.LogsSortOrder] = None, dedup_strategy: typing.Optional[common.LogsDedupStrategy] = None):
+    def __init__(self, show_labels: bool = False, show_common_labels: bool = False, show_time: bool = False, wrap_log_message: bool = False, prettify_log_message: bool = False, enable_log_details: bool = False, sort_order: typing.Optional[common.LogsSortOrder] = None, dedup_strategy: typing.Optional[common.LogsDedupStrategy] = None):
         self.show_labels = show_labels
         self.show_common_labels = show_common_labels
         self.show_time = show_time
-        self.show_log_context_toggle = show_log_context_toggle
         self.wrap_log_message = wrap_log_message
         self.prettify_log_message = prettify_log_message
         self.enable_log_details = enable_log_details
         self.sort_order = sort_order if sort_order is not None else common.LogsSortOrder.DESCENDING
         self.dedup_strategy = dedup_strategy if dedup_strategy is not None else common.LogsDedupStrategy.NONE
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "showLabels": self.show_labels,
             "showCommonLabels": self.show_common_labels,
             "showTime": self.show_time,
-            "showLogContextToggle": self.show_log_context_toggle,
             "wrapLogMessage": self.wrap_log_message,
             "prettifyLogMessage": self.prettify_log_message,
             "enableLogDetails": self.enable_log_details,
             "sortOrder": self.sort_order,
             "dedupStrategy": self.dedup_strategy,
         }
         return payload
@@ -47,16 +44,14 @@
         
         if "showLabels" in data:
             args["show_labels"] = data["showLabels"]
         if "showCommonLabels" in data:
             args["show_common_labels"] = data["showCommonLabels"]
         if "showTime" in data:
             args["show_time"] = data["showTime"]
-        if "showLogContextToggle" in data:
-            args["show_log_context_toggle"] = data["showLogContextToggle"]
         if "wrapLogMessage" in data:
             args["wrap_log_message"] = data["wrapLogMessage"]
         if "prettifyLogMessage" in data:
             args["prettify_log_message"] = data["prettifyLogMessage"]
         if "enableLogDetails" in data:
             args["enable_log_details"] = data["enableLogDetails"]
         if "sortOrder" in data:
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/loki.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/loki.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     STREAM = "stream"
 
 
 class SupportingQueryType(enum.StrEnum):
     LOGS_VOLUME = "logsVolume"
     LOGS_SAMPLE = "logsSample"
     DATA_SAMPLE = "dataSample"
-    INFINITE_SCROLL = "infiniteScroll"
 
 
 class LokiQueryDirection(enum.StrEnum):
     FORWARD = "forward"
     BACKWARD = "backward"
 
 
@@ -45,15 +44,17 @@
     instant: typing.Optional[bool]
     # Used to set step value for range queries.
     step: typing.Optional[str]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/news.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/nodegraph.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/parca.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/parca.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     label_selector: typing.Optional[str]
     # Specifies the type of profile to query.
     profile_type_id: typing.Optional[str]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/piechart.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/piechart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/preferences.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/preferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 
 
 class Preferences:
-    """
-    Spec defines user, team or org Grafana preferences
-    swagger:model Preferences
-    """
-
     # UID for the home dashboard
     home_dashboard_uid: typing.Optional[str]
     # The timezone selection
     # TODO: this should use the timezone defined in common
     timezone: typing.Optional[str]
     # day of the week (sunday, monday, etc)
     week_start: typing.Optional[str]
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/prometheus.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/prometheus.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     # @deprecated Used to specify how many times to divide max data points by. We use max data points under query options
     # See https://github.com/grafana/grafana/issues/48081
     interval_factor: typing.Optional[float]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: typing.Optional[str]
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/publicdashboard.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/role.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/rolebinding.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/stat.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/stat.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,41 +5,35 @@
 from ..cog import runtime as cogruntime
 
 
 class Options:
     graph_mode: common.BigValueGraphMode
     color_mode: common.BigValueColorMode
     justify_mode: common.BigValueJustifyMode
-    text_mode: common.BigValueTextMode
-    wide_layout: bool
     reduce_options: common.ReduceDataOptions
     text: typing.Optional[common.VizTextDisplayOptions]
-    show_percent_change: bool
+    text_mode: common.BigValueTextMode
     orientation: common.VizOrientation
 
-    def __init__(self, graph_mode: typing.Optional[common.BigValueGraphMode] = None, color_mode: typing.Optional[common.BigValueColorMode] = None, justify_mode: typing.Optional[common.BigValueJustifyMode] = None, text_mode: typing.Optional[common.BigValueTextMode] = None, wide_layout: bool = True, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, show_percent_change: bool = False, orientation: typing.Optional[common.VizOrientation] = None):
+    def __init__(self, graph_mode: typing.Optional[common.BigValueGraphMode] = None, color_mode: typing.Optional[common.BigValueColorMode] = None, justify_mode: typing.Optional[common.BigValueJustifyMode] = None, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, text_mode: typing.Optional[common.BigValueTextMode] = None, orientation: typing.Optional[common.VizOrientation] = None):
         self.graph_mode = graph_mode if graph_mode is not None else common.BigValueGraphMode.AREA
         self.color_mode = color_mode if color_mode is not None else common.BigValueColorMode.VALUE
         self.justify_mode = justify_mode if justify_mode is not None else common.BigValueJustifyMode.AUTO
-        self.text_mode = text_mode if text_mode is not None else common.BigValueTextMode.AUTO
-        self.wide_layout = wide_layout
         self.reduce_options = reduce_options if reduce_options is not None else common.ReduceDataOptions()
         self.text = text
-        self.show_percent_change = show_percent_change
+        self.text_mode = text_mode if text_mode is not None else common.BigValueTextMode.AUTO
         self.orientation = orientation if orientation is not None else common.VizOrientation.AUTO
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "graphMode": self.graph_mode,
             "colorMode": self.color_mode,
             "justifyMode": self.justify_mode,
-            "textMode": self.text_mode,
-            "wideLayout": self.wide_layout,
             "reduceOptions": self.reduce_options,
-            "showPercentChange": self.show_percent_change,
+            "textMode": self.text_mode,
             "orientation": self.orientation,
         }
         if self.text is not None:
             payload["text"] = self.text
         return payload
 
     @classmethod
@@ -48,24 +42,20 @@
         
         if "graphMode" in data:
             args["graph_mode"] = data["graphMode"]
         if "colorMode" in data:
             args["color_mode"] = data["colorMode"]
         if "justifyMode" in data:
             args["justify_mode"] = data["justifyMode"]
-        if "textMode" in data:
-            args["text_mode"] = data["textMode"]
-        if "wideLayout" in data:
-            args["wide_layout"] = data["wideLayout"]
         if "reduceOptions" in data:
             args["reduce_options"] = common.ReduceDataOptions.from_json(data["reduceOptions"])
         if "text" in data:
             args["text"] = common.VizTextDisplayOptions.from_json(data["text"])
-        if "showPercentChange" in data:
-            args["show_percent_change"] = data["showPercentChange"]
+        if "textMode" in data:
+            args["text_mode"] = data["textMode"]
         if "orientation" in data:
             args["orientation"] = data["orientation"]        
 
         return cls(**args)
 
 
 def variant_config():
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/statetimeline.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/statushistory.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/table.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,13 @@
             args["footer"] = common.TableFooterOptions.from_json(data["footer"])
         if "cellHeight" in data:
             args["cell_height"] = data["cellHeight"]        
 
         return cls(**args)
 
 
-FieldConfig: typing.TypeAlias = common.TableFieldOptions
-
-
-
-
-
 def variant_config():
     return cogruntime.PanelCfgConfig(
         identifier="table",
         options_from_json_hook=Options.from_json,
-        field_config_from_json_hook=FieldConfig.from_json,
+        field_config_from_json_hook=None,
     )
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/team.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/tempo.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/tempo.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,80 +7,72 @@
 
 
 class TempoQuery(cogvariants.Dataquery):
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
-    # If hide is set to true, Grafana will filter out the response(s) associated with this query before returning it to the panel.
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # TraceQL query or trace ID
-    query: typing.Optional[str]
+    query: str
     # @deprecated Logfmt query to filter traces by their tags. Example: http.status_code=200 error=true
     search: typing.Optional[str]
     # @deprecated Query traces by service name
     service_name: typing.Optional[str]
     # @deprecated Query traces by span name
     span_name: typing.Optional[str]
     # @deprecated Define the minimum duration to select traces. Use duration format, for example: 1.2s, 100ms
     min_duration: typing.Optional[str]
     # @deprecated Define the maximum duration to select traces. Use duration format, for example: 1.2s, 100ms
     max_duration: typing.Optional[str]
-    # Filters to be included in a PromQL query to select data for the service graph. Example: {client="app",service="app"}. Providing multiple values will produce union of results for each filter, using PromQL OR operator internally.
-    service_map_query: typing.Optional[typing.Union[str, list[str]]]
+    # Filters to be included in a PromQL query to select data for the service graph. Example: {client="app",service="app"}
+    service_map_query: typing.Optional[str]
     # Use service.namespace in addition to service.name to uniquely identify a service.
     service_map_include_namespace: typing.Optional[bool]
     # Defines the maximum number of traces that are returned from Tempo
     limit: typing.Optional[int]
-    # Defines the maximum number of spans per spanset that are returned from Tempo
-    spss: typing.Optional[int]
-    filters: list['TraceqlFilter']
-    # Filters that are used to query the metrics summary
-    group_by: typing.Optional[list['TraceqlFilter']]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
-    # The type of the table that is used to display the search results
-    table_type: typing.Optional['SearchTableType']
+    filters: list['TraceqlFilter']
 
-    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, query: typing.Optional[str] = None, search: typing.Optional[str] = None, service_name: typing.Optional[str] = None, span_name: typing.Optional[str] = None, min_duration: typing.Optional[str] = None, max_duration: typing.Optional[str] = None, service_map_query: typing.Optional[typing.Union[str, list[str]]] = None, service_map_include_namespace: typing.Optional[bool] = None, limit: typing.Optional[int] = None, spss: typing.Optional[int] = None, filters: typing.Optional[list['TraceqlFilter']] = None, group_by: typing.Optional[list['TraceqlFilter']] = None, datasource: typing.Optional[object] = None, table_type: typing.Optional['SearchTableType'] = None):
+    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, query: str = "", search: typing.Optional[str] = None, service_name: typing.Optional[str] = None, span_name: typing.Optional[str] = None, min_duration: typing.Optional[str] = None, max_duration: typing.Optional[str] = None, service_map_query: typing.Optional[str] = None, service_map_include_namespace: typing.Optional[bool] = None, limit: typing.Optional[int] = None, datasource: typing.Optional[object] = None, filters: typing.Optional[list['TraceqlFilter']] = None):
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.query = query
         self.search = search
         self.service_name = service_name
         self.span_name = span_name
         self.min_duration = min_duration
         self.max_duration = max_duration
         self.service_map_query = service_map_query
         self.service_map_include_namespace = service_map_include_namespace
         self.limit = limit
-        self.spss = spss
-        self.filters = filters if filters is not None else []
-        self.group_by = group_by
         self.datasource = datasource
-        self.table_type = table_type
+        self.filters = filters if filters is not None else []
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "refId": self.ref_id,
+            "query": self.query,
             "filters": self.filters,
         }
         if self.hide is not None:
             payload["hide"] = self.hide
         if self.query_type is not None:
             payload["queryType"] = self.query_type
-        if self.query is not None:
-            payload["query"] = self.query
         if self.search is not None:
             payload["search"] = self.search
         if self.service_name is not None:
             payload["serviceName"] = self.service_name
         if self.span_name is not None:
             payload["spanName"] = self.span_name
         if self.min_duration is not None:
@@ -89,22 +81,16 @@
             payload["maxDuration"] = self.max_duration
         if self.service_map_query is not None:
             payload["serviceMapQuery"] = self.service_map_query
         if self.service_map_include_namespace is not None:
             payload["serviceMapIncludeNamespace"] = self.service_map_include_namespace
         if self.limit is not None:
             payload["limit"] = self.limit
-        if self.spss is not None:
-            payload["spss"] = self.spss
-        if self.group_by is not None:
-            payload["groupBy"] = self.group_by
         if self.datasource is not None:
             payload["datasource"] = self.datasource
-        if self.table_type is not None:
-            payload["tableType"] = self.table_type
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "refId" in data:
@@ -127,38 +113,37 @@
             args["max_duration"] = data["maxDuration"]
         if "serviceMapQuery" in data:
             args["service_map_query"] = data["serviceMapQuery"]
         if "serviceMapIncludeNamespace" in data:
             args["service_map_include_namespace"] = data["serviceMapIncludeNamespace"]
         if "limit" in data:
             args["limit"] = data["limit"]
-        if "spss" in data:
-            args["spss"] = data["spss"]
-        if "filters" in data:
-            args["filters"] = data["filters"]
-        if "groupBy" in data:
-            args["group_by"] = data["groupBy"]
         if "datasource" in data:
             args["datasource"] = data["datasource"]
-        if "tableType" in data:
-            args["table_type"] = data["tableType"]        
+        if "filters" in data:
+            args["filters"] = data["filters"]        
 
         return cls(**args)
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
     return cogruntime.DataqueryConfig(
         identifier="tempo",
         from_json_hook=TempoQuery.from_json,
     )
 
 
 class TempoQueryType(enum.StrEnum):
+    """
+    search = Loki search, nativeSearch = Tempo search for backwards compatibility
+    """
+
     TRACEQL = "traceql"
     TRACEQL_SEARCH = "traceqlSearch"
+    SEARCH = "search"
     SERVICE_MAP = "serviceMap"
     UPLOAD = "upload"
     NATIVE_SEARCH = "nativeSearch"
     TRACE_ID = "traceId"
     CLEAR = "clear"
 
 
@@ -169,29 +154,19 @@
 
     PENDING = "pending"
     STREAMING = "streaming"
     DONE = "done"
     ERROR = "error"
 
 
-class SearchTableType(enum.StrEnum):
-    """
-    The type of the table that is used to display the search results
-    """
-
-    TRACES = "traces"
-    SPANS = "spans"
-
-
 class TraceqlSearchScope(enum.StrEnum):
     """
     static fields are pre-set in the UI, dynamic fields are added by the user
     """
 
-    INTRINSIC = "intrinsic"
     UNSCOPED = "unscoped"
     RESOURCE = "resource"
     SPAN = "span"
 
 
 class TraceqlFilter:
     # Uniquely identify the filter, will not be used in the query generation
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/testdata.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/testdata.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,708 +1,556 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-from ..cog import variants as cogvariants
+import enum
 import typing
+from ..cog import variants as cogvariants
 from ..cog import runtime as cogruntime
 
 
-class Dataquery(cogvariants.Dataquery):
-    alias: typing.Optional[str]
-    # Used for live query
-    channel: typing.Optional[str]
-    csv_content: typing.Optional[str]
-    csv_file_name: typing.Optional[str]
-    csv_wave: typing.Optional[list['CSVWave']]
-    # The datasource
-    datasource: typing.Optional['Datasource']
-    # Drop percentage (the chance we will lose a point 0-100)
-    drop_percent: typing.Optional[float]
-    # Possible enum values:
-    #  - `"frontend_exception"` 
-    #  - `"frontend_observable"` 
-    #  - `"server_panic"` 
-    error_type: typing.Optional[typing.Literal["frontend_exception", "frontend_observable", "server_panic"]]
-    flamegraph_diff: typing.Optional[bool]
-    # true if query is disabled (ie should not be returned to the dashboard)
-    # NOTE: this does not always imply that the query should not be executed since
-    # the results from a hidden query may be used as the input to other queries (SSE etc)
-    hide: typing.Optional[bool]
-    # Interval is the suggested duration between time points in a time series query.
-    # NOTE: the values for intervalMs is not saved in the query model.  It is typically calculated
-    # from the interval required to fill a pixels in the visualization
-    interval_ms: typing.Optional[float]
-    labels: typing.Optional[str]
-    level_column: typing.Optional[bool]
-    lines: typing.Optional[int]
-    max_val: typing.Optional[float]
-    # MaxDataPoints is the maximum number of data points that should be returned from a time series query.
-    # NOTE: the values for maxDataPoints is not saved in the query model.  It is typically calculated
-    # from the number of pixels visible in a visualization
-    max_data_points: typing.Optional[int]
-    min_val: typing.Optional[float]
-    nodes: typing.Optional['NodesQuery']
-    noise: typing.Optional[float]
-    points: typing.Optional[list[list[object]]]
-    pulse_wave: typing.Optional['PulseWaveQuery']
-    # QueryType is an optional identifier for the type of query.
-    # It can be used to distinguish different types of queries.
-    query_type: typing.Optional[str]
-    raw_frame_content: typing.Optional[str]
-    # RefID is the unique identifier of the query, set by the frontend call.
-    ref_id: typing.Optional[str]
-    # Optionally define expected query result behavior
-    result_assertions: typing.Optional['ResultAssertions']
-    # Possible enum values:
-    #  - `"annotations"` 
-    #  - `"arrow"` 
-    #  - `"csv_content"` 
-    #  - `"csv_file"` 
-    #  - `"csv_metric_values"` 
-    #  - `"datapoints_outside_range"` 
-    #  - `"exponential_heatmap_bucket_data"` 
-    #  - `"flame_graph"` 
-    #  - `"grafana_api"` 
-    #  - `"linear_heatmap_bucket_data"` 
-    #  - `"live"` 
-    #  - `"logs"` 
-    #  - `"manual_entry"` 
-    #  - `"no_data_points"` 
-    #  - `"node_graph"` 
-    #  - `"predictable_csv_wave"` 
-    #  - `"predictable_pulse"` 
-    #  - `"random_walk"` 
-    #  - `"random_walk_table"` 
-    #  - `"random_walk_with_error"` 
-    #  - `"raw_frame"` 
-    #  - `"server_error_500"` 
-    #  - `"simulation"` 
-    #  - `"slow_query"` 
-    #  - `"streaming_client"` 
-    #  - `"table_static"` 
-    #  - `"trace"` 
-    #  - `"usa"` 
-    #  - `"variables-query"` 
-    scenario_id: typing.Optional[typing.Literal["annotations", "arrow", "csv_content", "csv_file", "csv_metric_values", "datapoints_outside_range", "exponential_heatmap_bucket_data", "flame_graph", "grafana_api", "linear_heatmap_bucket_data", "live", "logs", "manual_entry", "no_data_points", "node_graph", "predictable_csv_wave", "predictable_pulse", "random_walk", "random_walk_table", "random_walk_with_error", "raw_frame", "server_error_500", "simulation", "slow_query", "streaming_client", "table_static", "trace", "usa", "variables-query"]]
-    series_count: typing.Optional[int]
-    sim: typing.Optional['SimulationQuery']
-    span_count: typing.Optional[int]
-    spread: typing.Optional[float]
-    start_value: typing.Optional[float]
-    stream: typing.Optional['StreamingQuery']
-    # common parameter used by many query types
-    string_input: typing.Optional[str]
-    # TimeRange represents the query range
-    # NOTE: unlike generic /ds/query, we can now send explicit time values in each query
-    # NOTE: the values for timeRange are not saved in a dashboard, they are constructed on the fly
-    time_range: typing.Optional['TimeRange']
-    usa: typing.Optional['USAQuery']
-    with_nil: typing.Optional[bool]
+class TestDataQueryType(enum.StrEnum):
+    RANDOM_WALK = "random_walk"
+    SLOW_QUERY = "slow_query"
+    RANDOM_WALK_WITH_ERROR = "random_walk_with_error"
+    RANDOM_WALK_TABLE = "random_walk_table"
+    EXPONENTIAL_HEATMAP_BUCKET_DATA = "exponential_heatmap_bucket_data"
+    LINEAR_HEATMAP_BUCKET_DATA = "linear_heatmap_bucket_data"
+    NO_DATA_POINTS = "no_data_points"
+    DATA_POINTS_OUTSIDE_RANGE = "datapoints_outside_range"
+    CSV_METRIC_VALUES = "csv_metric_values"
+    PREDICTABLE_PULSE = "predictable_pulse"
+    PREDICTABLE_CSV_WAVE = "predictable_csv_wave"
+    STREAMING_CLIENT = "streaming_client"
+    SIMULATION = "simulation"
+    USA = "usa"
+    LIVE = "live"
+    GRAFANA_API = "grafana_api"
+    ARROW = "arrow"
+    ANNOTATIONS = "annotations"
+    TABLE_STATIC = "table_static"
+    SERVER_ERROR500 = "server_error_500"
+    LOGS = "logs"
+    NODE_GRAPH = "node_graph"
+    FLAME_GRAPH = "flame_graph"
+    RAW_FRAME = "raw_frame"
+    CSV_FILE = "csv_file"
+    CSV_CONTENT = "csv_content"
+    TRACE = "trace"
+    MANUAL_ENTRY = "manual_entry"
+    VARIABLES_QUERY = "variables-query"
 
-    def __init__(self, alias: typing.Optional[str] = None, channel: typing.Optional[str] = None, csv_content: typing.Optional[str] = None, csv_file_name: typing.Optional[str] = None, csv_wave: typing.Optional[list['CSVWave']] = None, datasource: typing.Optional['Datasource'] = None, drop_percent: typing.Optional[float] = None, error_type: typing.Optional[typing.Literal["frontend_exception", "frontend_observable", "server_panic"]] = None, flamegraph_diff: typing.Optional[bool] = None, hide: typing.Optional[bool] = None, interval_ms: typing.Optional[float] = None, labels: typing.Optional[str] = None, level_column: typing.Optional[bool] = None, lines: typing.Optional[int] = None, max_val: typing.Optional[float] = None, max_data_points: typing.Optional[int] = None, min_val: typing.Optional[float] = None, nodes: typing.Optional['NodesQuery'] = None, noise: typing.Optional[float] = None, points: typing.Optional[list[list[object]]] = None, pulse_wave: typing.Optional['PulseWaveQuery'] = None, query_type: typing.Optional[str] = None, raw_frame_content: typing.Optional[str] = None, ref_id: typing.Optional[str] = None, result_assertions: typing.Optional['ResultAssertions'] = None, scenario_id: typing.Optional[typing.Literal["annotations", "arrow", "csv_content", "csv_file", "csv_metric_values", "datapoints_outside_range", "exponential_heatmap_bucket_data", "flame_graph", "grafana_api", "linear_heatmap_bucket_data", "live", "logs", "manual_entry", "no_data_points", "node_graph", "predictable_csv_wave", "predictable_pulse", "random_walk", "random_walk_table", "random_walk_with_error", "raw_frame", "server_error_500", "simulation", "slow_query", "streaming_client", "table_static", "trace", "usa", "variables-query"]] = None, series_count: typing.Optional[int] = None, sim: typing.Optional['SimulationQuery'] = None, span_count: typing.Optional[int] = None, spread: typing.Optional[float] = None, start_value: typing.Optional[float] = None, stream: typing.Optional['StreamingQuery'] = None, string_input: typing.Optional[str] = None, time_range: typing.Optional['TimeRange'] = None, usa: typing.Optional['USAQuery'] = None, with_nil: typing.Optional[bool] = None):
-        self.alias = alias
-        self.channel = channel
-        self.csv_content = csv_content
-        self.csv_file_name = csv_file_name
-        self.csv_wave = csv_wave
-        self.datasource = datasource
-        self.drop_percent = drop_percent
-        self.error_type = error_type
-        self.flamegraph_diff = flamegraph_diff
-        self.hide = hide
-        self.interval_ms = interval_ms
-        self.labels = labels
-        self.level_column = level_column
-        self.lines = lines
-        self.max_val = max_val
-        self.max_data_points = max_data_points
-        self.min_val = min_val
-        self.nodes = nodes
-        self.noise = noise
-        self.points = points
-        self.pulse_wave = pulse_wave
-        self.query_type = query_type
-        self.raw_frame_content = raw_frame_content
-        self.ref_id = ref_id
-        self.result_assertions = result_assertions
-        self.scenario_id = scenario_id
-        self.series_count = series_count
-        self.sim = sim
-        self.span_count = span_count
+
+class StreamingQuery:
+    type_val: typing.Literal["signal", "logs", "fetch"]
+    speed: int
+    spread: int
+    noise: int
+    bands: typing.Optional[int]
+    url: typing.Optional[str]
+
+    def __init__(self, type_val: typing.Optional[typing.Literal["signal", "logs", "fetch"]] = None, speed: int = 0, spread: int = 0, noise: int = 0, bands: typing.Optional[int] = None, url: typing.Optional[str] = None):
+        self.type_val = type_val if type_val is not None else "signal"
+        self.speed = speed
         self.spread = spread
-        self.start_value = start_value
-        self.stream = stream
-        self.string_input = string_input
-        self.time_range = time_range
-        self.usa = usa
-        self.with_nil = with_nil
+        self.noise = noise
+        self.bands = bands
+        self.url = url
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
+            "type": self.type_val,
+            "speed": self.speed,
+            "spread": self.spread,
+            "noise": self.noise,
         }
-        if self.alias is not None:
-            payload["alias"] = self.alias
-        if self.channel is not None:
-            payload["channel"] = self.channel
-        if self.csv_content is not None:
-            payload["csvContent"] = self.csv_content
-        if self.csv_file_name is not None:
-            payload["csvFileName"] = self.csv_file_name
-        if self.csv_wave is not None:
-            payload["csvWave"] = self.csv_wave
-        if self.datasource is not None:
-            payload["datasource"] = self.datasource
-        if self.drop_percent is not None:
-            payload["dropPercent"] = self.drop_percent
-        if self.error_type is not None:
-            payload["errorType"] = self.error_type
-        if self.flamegraph_diff is not None:
-            payload["flamegraphDiff"] = self.flamegraph_diff
-        if self.hide is not None:
-            payload["hide"] = self.hide
-        if self.interval_ms is not None:
-            payload["intervalMs"] = self.interval_ms
-        if self.labels is not None:
-            payload["labels"] = self.labels
-        if self.level_column is not None:
-            payload["levelColumn"] = self.level_column
-        if self.lines is not None:
-            payload["lines"] = self.lines
-        if self.max_val is not None:
-            payload["max"] = self.max_val
-        if self.max_data_points is not None:
-            payload["maxDataPoints"] = self.max_data_points
-        if self.min_val is not None:
-            payload["min"] = self.min_val
-        if self.nodes is not None:
-            payload["nodes"] = self.nodes
-        if self.noise is not None:
-            payload["noise"] = self.noise
-        if self.points is not None:
-            payload["points"] = self.points
-        if self.pulse_wave is not None:
-            payload["pulseWave"] = self.pulse_wave
-        if self.query_type is not None:
-            payload["queryType"] = self.query_type
-        if self.raw_frame_content is not None:
-            payload["rawFrameContent"] = self.raw_frame_content
-        if self.ref_id is not None:
-            payload["refId"] = self.ref_id
-        if self.result_assertions is not None:
-            payload["resultAssertions"] = self.result_assertions
-        if self.scenario_id is not None:
-            payload["scenarioId"] = self.scenario_id
-        if self.series_count is not None:
-            payload["seriesCount"] = self.series_count
-        if self.sim is not None:
-            payload["sim"] = self.sim
-        if self.span_count is not None:
-            payload["spanCount"] = self.span_count
-        if self.spread is not None:
-            payload["spread"] = self.spread
-        if self.start_value is not None:
-            payload["startValue"] = self.start_value
-        if self.stream is not None:
-            payload["stream"] = self.stream
-        if self.string_input is not None:
-            payload["stringInput"] = self.string_input
-        if self.time_range is not None:
-            payload["timeRange"] = self.time_range
-        if self.usa is not None:
-            payload["usa"] = self.usa
-        if self.with_nil is not None:
-            payload["withNil"] = self.with_nil
+        if self.bands is not None:
+            payload["bands"] = self.bands
+        if self.url is not None:
+            payload["url"] = self.url
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "alias" in data:
-            args["alias"] = data["alias"]
-        if "channel" in data:
-            args["channel"] = data["channel"]
-        if "csvContent" in data:
-            args["csv_content"] = data["csvContent"]
-        if "csvFileName" in data:
-            args["csv_file_name"] = data["csvFileName"]
-        if "csvWave" in data:
-            args["csv_wave"] = data["csvWave"]
-        if "datasource" in data:
-            args["datasource"] = Datasource.from_json(data["datasource"])
-        if "dropPercent" in data:
-            args["drop_percent"] = data["dropPercent"]
-        if "errorType" in data:
-            args["error_type"] = data["errorType"]
-        if "flamegraphDiff" in data:
-            args["flamegraph_diff"] = data["flamegraphDiff"]
-        if "hide" in data:
-            args["hide"] = data["hide"]
-        if "intervalMs" in data:
-            args["interval_ms"] = data["intervalMs"]
-        if "labels" in data:
-            args["labels"] = data["labels"]
-        if "levelColumn" in data:
-            args["level_column"] = data["levelColumn"]
-        if "lines" in data:
-            args["lines"] = data["lines"]
-        if "max" in data:
-            args["max_val"] = data["max"]
-        if "maxDataPoints" in data:
-            args["max_data_points"] = data["maxDataPoints"]
-        if "min" in data:
-            args["min_val"] = data["min"]
-        if "nodes" in data:
-            args["nodes"] = NodesQuery.from_json(data["nodes"])
-        if "noise" in data:
-            args["noise"] = data["noise"]
-        if "points" in data:
-            args["points"] = data["points"]
-        if "pulseWave" in data:
-            args["pulse_wave"] = PulseWaveQuery.from_json(data["pulseWave"])
-        if "queryType" in data:
-            args["query_type"] = data["queryType"]
-        if "rawFrameContent" in data:
-            args["raw_frame_content"] = data["rawFrameContent"]
-        if "refId" in data:
-            args["ref_id"] = data["refId"]
-        if "resultAssertions" in data:
-            args["result_assertions"] = ResultAssertions.from_json(data["resultAssertions"])
-        if "scenarioId" in data:
-            args["scenario_id"] = data["scenarioId"]
-        if "seriesCount" in data:
-            args["series_count"] = data["seriesCount"]
-        if "sim" in data:
-            args["sim"] = SimulationQuery.from_json(data["sim"])
-        if "spanCount" in data:
-            args["span_count"] = data["spanCount"]
+        if "type" in data:
+            args["type_val"] = data["type"]
+        if "speed" in data:
+            args["speed"] = data["speed"]
         if "spread" in data:
             args["spread"] = data["spread"]
-        if "startValue" in data:
-            args["start_value"] = data["startValue"]
-        if "stream" in data:
-            args["stream"] = StreamingQuery.from_json(data["stream"])
-        if "stringInput" in data:
-            args["string_input"] = data["stringInput"]
-        if "timeRange" in data:
-            args["time_range"] = TimeRange.from_json(data["timeRange"])
-        if "usa" in data:
-            args["usa"] = USAQuery.from_json(data["usa"])
-        if "withNil" in data:
-            args["with_nil"] = data["withNil"]        
+        if "noise" in data:
+            args["noise"] = data["noise"]
+        if "bands" in data:
+            args["bands"] = data["bands"]
+        if "url" in data:
+            args["url"] = data["url"]        
 
         return cls(**args)
 
 
-def variant_config() -> cogruntime.DataqueryConfig:
-    return cogruntime.DataqueryConfig(
-        identifier="",
-        from_json_hook=Dataquery.from_json,
-    )
-
-
-class CSVWave:
-    labels: typing.Optional[str]
-    name: typing.Optional[str]
+class PulseWaveQuery:
     time_step: typing.Optional[int]
-    values_csv: typing.Optional[str]
+    on_count: typing.Optional[int]
+    off_count: typing.Optional[int]
+    on_value: typing.Optional[float]
+    off_value: typing.Optional[float]
 
-    def __init__(self, labels: typing.Optional[str] = None, name: typing.Optional[str] = None, time_step: typing.Optional[int] = None, values_csv: typing.Optional[str] = None):
-        self.labels = labels
-        self.name = name
+    def __init__(self, time_step: typing.Optional[int] = None, on_count: typing.Optional[int] = None, off_count: typing.Optional[int] = None, on_value: typing.Optional[float] = None, off_value: typing.Optional[float] = None):
         self.time_step = time_step
-        self.values_csv = values_csv
+        self.on_count = on_count
+        self.off_count = off_count
+        self.on_value = on_value
+        self.off_value = off_value
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
-        if self.labels is not None:
-            payload["labels"] = self.labels
-        if self.name is not None:
-            payload["name"] = self.name
         if self.time_step is not None:
             payload["timeStep"] = self.time_step
-        if self.values_csv is not None:
-            payload["valuesCSV"] = self.values_csv
+        if self.on_count is not None:
+            payload["onCount"] = self.on_count
+        if self.off_count is not None:
+            payload["offCount"] = self.off_count
+        if self.on_value is not None:
+            payload["onValue"] = self.on_value
+        if self.off_value is not None:
+            payload["offValue"] = self.off_value
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "labels" in data:
-            args["labels"] = data["labels"]
-        if "name" in data:
-            args["name"] = data["name"]
         if "timeStep" in data:
             args["time_step"] = data["timeStep"]
-        if "valuesCSV" in data:
-            args["values_csv"] = data["valuesCSV"]        
+        if "onCount" in data:
+            args["on_count"] = data["onCount"]
+        if "offCount" in data:
+            args["off_count"] = data["offCount"]
+        if "onValue" in data:
+            args["on_value"] = data["onValue"]
+        if "offValue" in data:
+            args["off_value"] = data["offValue"]        
 
         return cls(**args)
 
 
-class Datasource:
-    # The datasource plugin type
-    type_val: str
-    # Datasource UID
-    uid: typing.Optional[str]
+class SimulationQuery:
+    key: 'Key'
+    config: typing.Optional[object]
+    stream: typing.Optional[bool]
+    last: typing.Optional[bool]
 
-    def __init__(self, type_val: str = "", uid: typing.Optional[str] = None):
-        self.type_val = type_val
-        self.uid = uid
+    def __init__(self, key: typing.Optional['Key'] = None, config: typing.Optional[object] = None, stream: typing.Optional[bool] = None, last: typing.Optional[bool] = None):
+        self.key = key if key is not None else Key()
+        self.config = config
+        self.stream = stream
+        self.last = last
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "type": self.type_val,
+            "key": self.key,
         }
-        if self.uid is not None:
-            payload["uid"] = self.uid
+        if self.config is not None:
+            payload["config"] = self.config
+        if self.stream is not None:
+            payload["stream"] = self.stream
+        if self.last is not None:
+            payload["last"] = self.last
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "type" in data:
-            args["type_val"] = data["type"]
-        if "uid" in data:
-            args["uid"] = data["uid"]        
+        if "key" in data:
+            args["key"] = Key.from_json(data["key"])
+        if "config" in data:
+            args["config"] = data["config"]
+        if "stream" in data:
+            args["stream"] = data["stream"]
+        if "last" in data:
+            args["last"] = data["last"]        
 
         return cls(**args)
 
 
 class NodesQuery:
+    type_val: typing.Optional[typing.Literal["random", "response", "random edges"]]
     count: typing.Optional[int]
-    seed: typing.Optional[int]
-    # Possible enum values:
-    #  - `"random"` 
-    #  - `"random edges"` 
-    #  - `"response_medium"` 
-    #  - `"response_small"` 
-    #  - `"feature_showcase"` 
-    type_val: typing.Optional[typing.Literal["random", "random edges", "response_medium", "response_small", "feature_showcase"]]
 
-    def __init__(self, count: typing.Optional[int] = None, seed: typing.Optional[int] = None, type_val: typing.Optional[typing.Literal["random", "random edges", "response_medium", "response_small", "feature_showcase"]] = None):
-        self.count = count
-        self.seed = seed
+    def __init__(self, type_val: typing.Optional[typing.Literal["random", "response", "random edges"]] = None, count: typing.Optional[int] = None):
         self.type_val = type_val
+        self.count = count
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
-        if self.count is not None:
-            payload["count"] = self.count
-        if self.seed is not None:
-            payload["seed"] = self.seed
         if self.type_val is not None:
             payload["type"] = self.type_val
+        if self.count is not None:
+            payload["count"] = self.count
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "count" in data:
-            args["count"] = data["count"]
-        if "seed" in data:
-            args["seed"] = data["seed"]
         if "type" in data:
-            args["type_val"] = data["type"]        
+            args["type_val"] = data["type"]
+        if "count" in data:
+            args["count"] = data["count"]        
 
         return cls(**args)
 
 
-class PulseWaveQuery:
-    off_count: typing.Optional[int]
-    off_value: typing.Optional[float]
-    on_count: typing.Optional[int]
-    on_value: typing.Optional[float]
-    time_step: typing.Optional[int]
+class USAQuery:
+    mode: typing.Optional[str]
+    period: typing.Optional[str]
+    fields: typing.Optional[list[str]]
+    states: typing.Optional[list[str]]
 
-    def __init__(self, off_count: typing.Optional[int] = None, off_value: typing.Optional[float] = None, on_count: typing.Optional[int] = None, on_value: typing.Optional[float] = None, time_step: typing.Optional[int] = None):
-        self.off_count = off_count
-        self.off_value = off_value
-        self.on_count = on_count
-        self.on_value = on_value
-        self.time_step = time_step
+    def __init__(self, mode: typing.Optional[str] = None, period: typing.Optional[str] = None, fields: typing.Optional[list[str]] = None, states: typing.Optional[list[str]] = None):
+        self.mode = mode
+        self.period = period
+        self.fields = fields
+        self.states = states
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
-        if self.off_count is not None:
-            payload["offCount"] = self.off_count
-        if self.off_value is not None:
-            payload["offValue"] = self.off_value
-        if self.on_count is not None:
-            payload["onCount"] = self.on_count
-        if self.on_value is not None:
-            payload["onValue"] = self.on_value
-        if self.time_step is not None:
-            payload["timeStep"] = self.time_step
+        if self.mode is not None:
+            payload["mode"] = self.mode
+        if self.period is not None:
+            payload["period"] = self.period
+        if self.fields is not None:
+            payload["fields"] = self.fields
+        if self.states is not None:
+            payload["states"] = self.states
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "offCount" in data:
-            args["off_count"] = data["offCount"]
-        if "offValue" in data:
-            args["off_value"] = data["offValue"]
-        if "onCount" in data:
-            args["on_count"] = data["onCount"]
-        if "onValue" in data:
-            args["on_value"] = data["onValue"]
-        if "timeStep" in data:
-            args["time_step"] = data["timeStep"]        
+        if "mode" in data:
+            args["mode"] = data["mode"]
+        if "period" in data:
+            args["period"] = data["period"]
+        if "fields" in data:
+            args["fields"] = data["fields"]
+        if "states" in data:
+            args["states"] = data["states"]        
 
         return cls(**args)
 
 
-class ResultAssertions:
-    # Maximum frame count
-    max_frames: typing.Optional[int]
-    # Type asserts that the frame matches a known type structure.
-    # Possible enum values:
-    #  - `""` 
-    #  - `"timeseries-wide"` 
-    #  - `"timeseries-long"` 
-    #  - `"timeseries-many"` 
-    #  - `"timeseries-multi"` 
-    #  - `"directory-listing"` 
-    #  - `"table"` 
-    #  - `"numeric-wide"` 
-    #  - `"numeric-multi"` 
-    #  - `"numeric-long"` 
-    #  - `"log-lines"` 
-    type_val: typing.Optional[typing.Literal["", "timeseries-wide", "timeseries-long", "timeseries-many", "timeseries-multi", "directory-listing", "table", "numeric-wide", "numeric-multi", "numeric-long", "log-lines"]]
-    # TypeVersion is the version of the Type property. Versions greater than 0.0 correspond to the dataplane
-    # contract documentation https://grafana.github.io/dataplane/contract/.
-    type_version: list[int]
+class CSVWave:
+    time_step: typing.Optional[int]
+    name: typing.Optional[str]
+    values_csv: typing.Optional[str]
+    labels: typing.Optional[str]
 
-    def __init__(self, max_frames: typing.Optional[int] = None, type_val: typing.Optional[typing.Literal["", "timeseries-wide", "timeseries-long", "timeseries-many", "timeseries-multi", "directory-listing", "table", "numeric-wide", "numeric-multi", "numeric-long", "log-lines"]] = None, type_version: typing.Optional[list[int]] = None):
-        self.max_frames = max_frames
-        self.type_val = type_val
-        self.type_version = type_version if type_version is not None else []
+    def __init__(self, time_step: typing.Optional[int] = None, name: typing.Optional[str] = None, values_csv: typing.Optional[str] = None, labels: typing.Optional[str] = None):
+        self.time_step = time_step
+        self.name = name
+        self.values_csv = values_csv
+        self.labels = labels
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "typeVersion": self.type_version,
         }
-        if self.max_frames is not None:
-            payload["maxFrames"] = self.max_frames
-        if self.type_val is not None:
-            payload["type"] = self.type_val
+        if self.time_step is not None:
+            payload["timeStep"] = self.time_step
+        if self.name is not None:
+            payload["name"] = self.name
+        if self.values_csv is not None:
+            payload["valuesCSV"] = self.values_csv
+        if self.labels is not None:
+            payload["labels"] = self.labels
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "maxFrames" in data:
-            args["max_frames"] = data["maxFrames"]
-        if "type" in data:
-            args["type_val"] = data["type"]
-        if "typeVersion" in data:
-            args["type_version"] = data["typeVersion"]        
+        if "timeStep" in data:
+            args["time_step"] = data["timeStep"]
+        if "name" in data:
+            args["name"] = data["name"]
+        if "valuesCSV" in data:
+            args["values_csv"] = data["valuesCSV"]
+        if "labels" in data:
+            args["labels"] = data["labels"]        
 
         return cls(**args)
 
 
-class Key:
-    tick: float
-    type_val: str
-    uid: typing.Optional[str]
+class Scenario:
+    """
+    TODO: Should this live here given it's not used in the dataquery?
+    """
 
-    def __init__(self, tick: float = 0, type_val: str = "", uid: typing.Optional[str] = None):
-        self.tick = tick
-        self.type_val = type_val
-        self.uid = uid
+    id_val: str
+    name: str
+    string_input: str
+    description: typing.Optional[str]
+    hide_alias_field: typing.Optional[bool]
+
+    def __init__(self, id_val: str = "", name: str = "", string_input: str = "", description: typing.Optional[str] = None, hide_alias_field: typing.Optional[bool] = None):
+        self.id_val = id_val
+        self.name = name
+        self.string_input = string_input
+        self.description = description
+        self.hide_alias_field = hide_alias_field
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "tick": self.tick,
-            "type": self.type_val,
+            "id": self.id_val,
+            "name": self.name,
+            "stringInput": self.string_input,
         }
-        if self.uid is not None:
-            payload["uid"] = self.uid
+        if self.description is not None:
+            payload["description"] = self.description
+        if self.hide_alias_field is not None:
+            payload["hideAliasField"] = self.hide_alias_field
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "tick" in data:
-            args["tick"] = data["tick"]
-        if "type" in data:
-            args["type_val"] = data["type"]
-        if "uid" in data:
-            args["uid"] = data["uid"]        
+        if "id" in data:
+            args["id_val"] = data["id"]
+        if "name" in data:
+            args["name"] = data["name"]
+        if "stringInput" in data:
+            args["string_input"] = data["stringInput"]
+        if "description" in data:
+            args["description"] = data["description"]
+        if "hideAliasField" in data:
+            args["hide_alias_field"] = data["hideAliasField"]        
 
         return cls(**args)
 
 
-class SimulationQuery:
-    config: typing.Optional[object]
-    key: 'Key'
-    last: typing.Optional[bool]
-    stream: typing.Optional[bool]
+class Dataquery(cogvariants.Dataquery):
+    alias: typing.Optional[str]
+    scenario_id: typing.Optional['TestDataQueryType']
+    string_input: typing.Optional[str]
+    stream: typing.Optional['StreamingQuery']
+    pulse_wave: typing.Optional['PulseWaveQuery']
+    sim: typing.Optional['SimulationQuery']
+    csv_wave: typing.Optional[list['CSVWave']]
+    labels: typing.Optional[str]
+    lines: typing.Optional[int]
+    level_column: typing.Optional[bool]
+    channel: typing.Optional[str]
+    nodes: typing.Optional['NodesQuery']
+    csv_file_name: typing.Optional[str]
+    csv_content: typing.Optional[str]
+    raw_frame_content: typing.Optional[str]
+    series_count: typing.Optional[int]
+    usa: typing.Optional['USAQuery']
+    error_type: typing.Optional[typing.Literal["server_panic", "frontend_exception", "frontend_observable"]]
+    span_count: typing.Optional[int]
+    points: typing.Optional[list[list[typing.Union[str, int]]]]
+    # Drop percentage (the chance we will lose a point 0-100)
+    drop_percent: typing.Optional[float]
+    # A unique identifier for the query within the list of targets.
+    # In server side expressions, the refId is used as a variable name to identify results.
+    # By default, the UI will assign A->Z; however setting meaningful names may be useful.
+    ref_id: typing.Optional[str]
+    # true if query is disabled (ie should not be returned to the dashboard)
+    # Note this does not always imply that the query should not be executed since
+    # the results from a hidden query may be used as the input to other queries (SSE etc)
+    hide: typing.Optional[bool]
+    # Specify the query flavor
+    # TODO make this required and give it a default
+    query_type: typing.Optional[str]
+    # For mixed data sources the selected datasource is on the query level.
+    # For non mixed scenarios this is undefined.
+    # TODO find a better way to do this ^ that's friendly to schema
+    # TODO this shouldn't be unknown but DataSourceRef | null
+    datasource: typing.Optional[object]
 
-    def __init__(self, config: typing.Optional[object] = None, key: typing.Optional['Key'] = None, last: typing.Optional[bool] = None, stream: typing.Optional[bool] = None):
-        self.config = config
-        self.key = key if key is not None else Key()
-        self.last = last
+    def __init__(self, alias: typing.Optional[str] = None, scenario_id: typing.Optional['TestDataQueryType'] = None, string_input: typing.Optional[str] = None, stream: typing.Optional['StreamingQuery'] = None, pulse_wave: typing.Optional['PulseWaveQuery'] = None, sim: typing.Optional['SimulationQuery'] = None, csv_wave: typing.Optional[list['CSVWave']] = None, labels: typing.Optional[str] = None, lines: typing.Optional[int] = None, level_column: typing.Optional[bool] = None, channel: typing.Optional[str] = None, nodes: typing.Optional['NodesQuery'] = None, csv_file_name: typing.Optional[str] = None, csv_content: typing.Optional[str] = None, raw_frame_content: typing.Optional[str] = None, series_count: typing.Optional[int] = None, usa: typing.Optional['USAQuery'] = None, error_type: typing.Optional[typing.Literal["server_panic", "frontend_exception", "frontend_observable"]] = None, span_count: typing.Optional[int] = None, points: typing.Optional[list[list[typing.Union[str, int]]]] = None, drop_percent: typing.Optional[float] = None, ref_id: typing.Optional[str] = None, hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
+        self.alias = alias
+        self.scenario_id = scenario_id if scenario_id is not None else TestDataQueryType.RANDOM_WALK
+        self.string_input = string_input
         self.stream = stream
+        self.pulse_wave = pulse_wave
+        self.sim = sim
+        self.csv_wave = csv_wave
+        self.labels = labels
+        self.lines = lines
+        self.level_column = level_column
+        self.channel = channel
+        self.nodes = nodes
+        self.csv_file_name = csv_file_name
+        self.csv_content = csv_content
+        self.raw_frame_content = raw_frame_content
+        self.series_count = series_count
+        self.usa = usa
+        self.error_type = error_type
+        self.span_count = span_count
+        self.points = points
+        self.drop_percent = drop_percent
+        self.ref_id = ref_id
+        self.hide = hide
+        self.query_type = query_type
+        self.datasource = datasource
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "key": self.key,
         }
-        if self.config is not None:
-            payload["config"] = self.config
-        if self.last is not None:
-            payload["last"] = self.last
+        if self.alias is not None:
+            payload["alias"] = self.alias
+        if self.scenario_id is not None:
+            payload["scenarioId"] = self.scenario_id
+        if self.string_input is not None:
+            payload["stringInput"] = self.string_input
         if self.stream is not None:
             payload["stream"] = self.stream
+        if self.pulse_wave is not None:
+            payload["pulseWave"] = self.pulse_wave
+        if self.sim is not None:
+            payload["sim"] = self.sim
+        if self.csv_wave is not None:
+            payload["csvWave"] = self.csv_wave
+        if self.labels is not None:
+            payload["labels"] = self.labels
+        if self.lines is not None:
+            payload["lines"] = self.lines
+        if self.level_column is not None:
+            payload["levelColumn"] = self.level_column
+        if self.channel is not None:
+            payload["channel"] = self.channel
+        if self.nodes is not None:
+            payload["nodes"] = self.nodes
+        if self.csv_file_name is not None:
+            payload["csvFileName"] = self.csv_file_name
+        if self.csv_content is not None:
+            payload["csvContent"] = self.csv_content
+        if self.raw_frame_content is not None:
+            payload["rawFrameContent"] = self.raw_frame_content
+        if self.series_count is not None:
+            payload["seriesCount"] = self.series_count
+        if self.usa is not None:
+            payload["usa"] = self.usa
+        if self.error_type is not None:
+            payload["errorType"] = self.error_type
+        if self.span_count is not None:
+            payload["spanCount"] = self.span_count
+        if self.points is not None:
+            payload["points"] = self.points
+        if self.drop_percent is not None:
+            payload["dropPercent"] = self.drop_percent
+        if self.ref_id is not None:
+            payload["refId"] = self.ref_id
+        if self.hide is not None:
+            payload["hide"] = self.hide
+        if self.query_type is not None:
+            payload["queryType"] = self.query_type
+        if self.datasource is not None:
+            payload["datasource"] = self.datasource
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "config" in data:
-            args["config"] = data["config"]
-        if "key" in data:
-            args["key"] = Key.from_json(data["key"])
-        if "last" in data:
-            args["last"] = data["last"]
+        if "alias" in data:
+            args["alias"] = data["alias"]
+        if "scenarioId" in data:
+            args["scenario_id"] = data["scenarioId"]
+        if "stringInput" in data:
+            args["string_input"] = data["stringInput"]
         if "stream" in data:
-            args["stream"] = data["stream"]        
+            args["stream"] = StreamingQuery.from_json(data["stream"])
+        if "pulseWave" in data:
+            args["pulse_wave"] = PulseWaveQuery.from_json(data["pulseWave"])
+        if "sim" in data:
+            args["sim"] = SimulationQuery.from_json(data["sim"])
+        if "csvWave" in data:
+            args["csv_wave"] = data["csvWave"]
+        if "labels" in data:
+            args["labels"] = data["labels"]
+        if "lines" in data:
+            args["lines"] = data["lines"]
+        if "levelColumn" in data:
+            args["level_column"] = data["levelColumn"]
+        if "channel" in data:
+            args["channel"] = data["channel"]
+        if "nodes" in data:
+            args["nodes"] = NodesQuery.from_json(data["nodes"])
+        if "csvFileName" in data:
+            args["csv_file_name"] = data["csvFileName"]
+        if "csvContent" in data:
+            args["csv_content"] = data["csvContent"]
+        if "rawFrameContent" in data:
+            args["raw_frame_content"] = data["rawFrameContent"]
+        if "seriesCount" in data:
+            args["series_count"] = data["seriesCount"]
+        if "usa" in data:
+            args["usa"] = USAQuery.from_json(data["usa"])
+        if "errorType" in data:
+            args["error_type"] = data["errorType"]
+        if "spanCount" in data:
+            args["span_count"] = data["spanCount"]
+        if "points" in data:
+            args["points"] = data["points"]
+        if "dropPercent" in data:
+            args["drop_percent"] = data["dropPercent"]
+        if "refId" in data:
+            args["ref_id"] = data["refId"]
+        if "hide" in data:
+            args["hide"] = data["hide"]
+        if "queryType" in data:
+            args["query_type"] = data["queryType"]
+        if "datasource" in data:
+            args["datasource"] = data["datasource"]        
 
         return cls(**args)
 
 
-class StreamingQuery:
-    bands: typing.Optional[int]
-    noise: float
-    speed: float
-    spread: float
-    # Possible enum values:
-    #  - `"fetch"` 
-    #  - `"logs"` 
-    #  - `"signal"` 
-    #  - `"traces"` 
-    type_val: typing.Literal["fetch", "logs", "signal", "traces"]
-    url: typing.Optional[str]
+def variant_config() -> cogruntime.DataqueryConfig:
+    return cogruntime.DataqueryConfig(
+        identifier="testdata",
+        from_json_hook=Dataquery.from_json,
+    )
 
-    def __init__(self, bands: typing.Optional[int] = None, noise: float = 0, speed: float = 0, spread: float = 0, type_val: typing.Optional[typing.Literal["fetch", "logs", "signal", "traces"]] = None, url: typing.Optional[str] = None):
-        self.bands = bands
-        self.noise = noise
-        self.speed = speed
-        self.spread = spread
-        self.type_val = type_val if type_val is not None else "fetch"
-        self.url = url
+
+class Key:
+    type_val: str
+    tick: float
+    uid: typing.Optional[str]
+
+    def __init__(self, type_val: str = "", tick: float = 0, uid: typing.Optional[str] = None):
+        self.type_val = type_val
+        self.tick = tick
+        self.uid = uid
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "noise": self.noise,
-            "speed": self.speed,
-            "spread": self.spread,
             "type": self.type_val,
+            "tick": self.tick,
         }
-        if self.bands is not None:
-            payload["bands"] = self.bands
-        if self.url is not None:
-            payload["url"] = self.url
+        if self.uid is not None:
+            payload["uid"] = self.uid
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "bands" in data:
-            args["bands"] = data["bands"]
-        if "noise" in data:
-            args["noise"] = data["noise"]
-        if "speed" in data:
-            args["speed"] = data["speed"]
-        if "spread" in data:
-            args["spread"] = data["spread"]
         if "type" in data:
             args["type_val"] = data["type"]
-        if "url" in data:
-            args["url"] = data["url"]        
-
-        return cls(**args)
-
-
-class TimeRange:
-    # From is the start time of the query.
-    from_val: str
-    # To is the end time of the query.
-    to: str
-
-    def __init__(self, from_val: str = "now-6h", to: str = "now"):
-        self.from_val = from_val
-        self.to = to
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "from": self.from_val,
-            "to": self.to,
-        }
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "from" in data:
-            args["from_val"] = data["from"]
-        if "to" in data:
-            args["to"] = data["to"]        
-
-        return cls(**args)
-
-
-class USAQuery:
-    fields: typing.Optional[list[str]]
-    mode: typing.Optional[str]
-    period: typing.Optional[str]
-    states: typing.Optional[list[str]]
-
-    def __init__(self, fields: typing.Optional[list[str]] = None, mode: typing.Optional[str] = None, period: typing.Optional[str] = None, states: typing.Optional[list[str]] = None):
-        self.fields = fields
-        self.mode = mode
-        self.period = period
-        self.states = states
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-        }
-        if self.fields is not None:
-            payload["fields"] = self.fields
-        if self.mode is not None:
-            payload["mode"] = self.mode
-        if self.period is not None:
-            payload["period"] = self.period
-        if self.states is not None:
-            payload["states"] = self.states
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "fields" in data:
-            args["fields"] = data["fields"]
-        if "mode" in data:
-            args["mode"] = data["mode"]
-        if "period" in data:
-            args["period"] = data["period"]
-        if "states" in data:
-            args["states"] = data["states"]        
+        if "tick" in data:
+            args["tick"] = data["tick"]
+        if "uid" in data:
+            args["uid"] = data["uid"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/text.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/text.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/timeseries.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/timeseries.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,45 +5,39 @@
 from ..cog import runtime as cogruntime
 
 
 class Options:
     timezone: typing.Optional[list[common.TimeZone]]
     legend: common.VizLegendOptions
     tooltip: common.VizTooltipOptions
-    orientation: typing.Optional[common.VizOrientation]
 
-    def __init__(self, timezone: typing.Optional[list[common.TimeZone]] = None, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, orientation: typing.Optional[common.VizOrientation] = None):
+    def __init__(self, timezone: typing.Optional[list[common.TimeZone]] = None, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None):
         self.timezone = timezone
         self.legend = legend if legend is not None else common.VizLegendOptions(calcs=[], display_mode=common.LegendDisplayMode.LIST, placement=common.LegendPlacement.BOTTOM)
         self.tooltip = tooltip if tooltip is not None else common.VizTooltipOptions()
-        self.orientation = orientation
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "legend": self.legend,
             "tooltip": self.tooltip,
         }
         if self.timezone is not None:
             payload["timezone"] = self.timezone
-        if self.orientation is not None:
-            payload["orientation"] = self.orientation
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "timezone" in data:
             args["timezone"] = data["timezone"]
         if "legend" in data:
             args["legend"] = common.VizLegendOptions.from_json(data["legend"])
         if "tooltip" in data:
-            args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])
-        if "orientation" in data:
-            args["orientation"] = data["orientation"]        
+            args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])        
 
         return cls(**args)
 
 
 FieldConfig: typing.TypeAlias = common.GraphFieldConfig
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/trend.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/trend.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/grafana_foundation_sdk/models/xychart.py` & `grafana_foundation_sdk-1716541850!10.1.0/grafana_foundation_sdk/models/xychart.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,33 +3,25 @@
 import enum
 import typing
 from ..models import common
 from ..cog import runtime as cogruntime
 
 
 class SeriesMapping(enum.StrEnum):
-    """
-    Auto is "table" in the UI
-    """
-
     AUTO = "auto"
     MANUAL = "manual"
 
 
 class ScatterShow(enum.StrEnum):
     POINTS = "points"
     LINES = "lines"
     POINTS_AND_LINES = "points+lines"
 
 
 class XYDimensionConfig:
-    """
-    Configuration for the Table/Auto mode
-    """
-
     frame: int
     x: typing.Optional[str]
     exclude: typing.Optional[list[str]]
 
     def __init__(self, frame: int = 0, x: typing.Optional[str] = None, exclude: typing.Optional[list[str]] = None):
         self.frame = frame
         self.x = x
@@ -72,19 +64,18 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
-    axis_centered_zero: typing.Optional[bool]
     label_value: typing.Optional[common.TextDimensionConfig]
-    axis_border_show: typing.Optional[bool]
+    axis_centered_zero: typing.Optional[bool]
 
-    def __init__(self, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_border_show: typing.Optional[bool] = None):
+    def __init__(self, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_centered_zero: typing.Optional[bool] = None):
         self.show = show if show is not None else ScatterShow.POINTS
         self.point_size = point_size
         self.point_color = point_color
         self.line_color = line_color
         self.line_width = line_width
         self.line_style = line_style
         self.label = label if label is not None else common.VisibilityMode.AUTO
@@ -93,17 +84,16 @@
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
-        self.axis_centered_zero = axis_centered_zero
         self.label_value = label_value
-        self.axis_border_show = axis_border_show
+        self.axis_centered_zero = axis_centered_zero
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.show is not None:
             payload["show"] = self.show
         if self.point_size is not None:
@@ -132,20 +122,18 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.label_value is not None:
             payload["labelValue"] = self.label_value
-        if self.axis_border_show is not None:
-            payload["axisBorderShow"] = self.axis_border_show
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "show" in data:
@@ -176,28 +164,25 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "labelValue" in data:
             args["label_value"] = common.TextDimensionConfig.from_json(data["labelValue"])
-        if "axisBorderShow" in data:
-            args["axis_border_show"] = data["axisBorderShow"]        
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]        
 
         return cls(**args)
 
 
 class ScatterSeriesConfig:
     x: typing.Optional[str]
     y: typing.Optional[str]
-    name: typing.Optional[str]
     show: typing.Optional['ScatterShow']
     point_size: typing.Optional[common.ScaleDimensionConfig]
     point_color: typing.Optional[common.ColorDimensionConfig]
     line_color: typing.Optional[common.ColorDimensionConfig]
     line_width: typing.Optional[int]
     line_style: typing.Optional[common.LineStyle]
     label: typing.Optional[common.VisibilityMode]
@@ -206,23 +191,21 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
-    axis_centered_zero: typing.Optional[bool]
-    frame: typing.Optional[float]
+    name: typing.Optional[str]
     label_value: typing.Optional[common.TextDimensionConfig]
-    axis_border_show: typing.Optional[bool]
+    axis_centered_zero: typing.Optional[bool]
 
-    def __init__(self, x: typing.Optional[str] = None, y: typing.Optional[str] = None, name: typing.Optional[str] = None, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, frame: typing.Optional[float] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_border_show: typing.Optional[bool] = None):
+    def __init__(self, x: typing.Optional[str] = None, y: typing.Optional[str] = None, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, name: typing.Optional[str] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_centered_zero: typing.Optional[bool] = None):
         self.x = x
         self.y = y
-        self.name = name
         self.show = show if show is not None else ScatterShow.POINTS
         self.point_size = point_size
         self.point_color = point_color
         self.line_color = line_color
         self.line_width = line_width
         self.line_style = line_style
         self.label = label if label is not None else common.VisibilityMode.AUTO
@@ -231,28 +214,25 @@
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
-        self.axis_centered_zero = axis_centered_zero
-        self.frame = frame
+        self.name = name
         self.label_value = label_value
-        self.axis_border_show = axis_border_show
+        self.axis_centered_zero = axis_centered_zero
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.x is not None:
             payload["x"] = self.x
         if self.y is not None:
             payload["y"] = self.y
-        if self.name is not None:
-            payload["name"] = self.name
         if self.show is not None:
             payload["show"] = self.show
         if self.point_size is not None:
             payload["pointSize"] = self.point_size
         if self.point_color is not None:
             payload["pointColor"] = self.point_color
         if self.line_color is not None:
@@ -277,34 +257,30 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
-        if self.frame is not None:
-            payload["frame"] = self.frame
+        if self.name is not None:
+            payload["name"] = self.name
         if self.label_value is not None:
             payload["labelValue"] = self.label_value
-        if self.axis_border_show is not None:
-            payload["axisBorderShow"] = self.axis_border_show
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "x" in data:
             args["x"] = data["x"]
         if "y" in data:
             args["y"] = data["y"]
-        if "name" in data:
-            args["name"] = data["name"]
         if "show" in data:
             args["show"] = data["show"]
         if "pointSize" in data:
             args["point_size"] = common.ScaleDimensionConfig.from_json(data["pointSize"])
         if "pointColor" in data:
             args["point_color"] = common.ColorDimensionConfig.from_json(data["pointColor"])
         if "lineColor" in data:
@@ -329,33 +305,29 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
-        if "frame" in data:
-            args["frame"] = data["frame"]
+        if "name" in data:
+            args["name"] = data["name"]
         if "labelValue" in data:
             args["label_value"] = common.TextDimensionConfig.from_json(data["labelValue"])
-        if "axisBorderShow" in data:
-            args["axis_border_show"] = data["axisBorderShow"]        
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]        
 
         return cls(**args)
 
 
 class Options:
     series_mapping: typing.Optional['SeriesMapping']
-    # Table Mode (auto)
     dims: 'XYDimensionConfig'
     legend: common.VizLegendOptions
     tooltip: common.VizTooltipOptions
-    # Manual Mode
     series: list['ScatterSeriesConfig']
 
     def __init__(self, series_mapping: typing.Optional['SeriesMapping'] = None, dims: typing.Optional['XYDimensionConfig'] = None, legend: typing.Optional[common.VizLegendOptions] = None, tooltip: typing.Optional[common.VizTooltipOptions] = None, series: typing.Optional[list['ScatterSeriesConfig']] = None):
         self.series_mapping = series_mapping
         self.dims = dims if dims is not None else XYDimensionConfig()
         self.legend = legend if legend is not None else common.VizLegendOptions()
         self.tooltip = tooltip if tooltip is not None else common.VizTooltipOptions()
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/LICENSE.md` & `grafana_foundation_sdk-1716541850!10.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/README.md` & `grafana_foundation_sdk-1716541850!10.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v11.0.x.**
+> This branch contains **types and builders generated for Grafana v10.1.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1716541742!11.0.0'
+python3 -m pip install 'grafana_foundation_sdk==1716541850!10.1.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/pyproject.toml` & `grafana_foundation_sdk-1716541850!10.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "observability",
     "sdk",
     "grafana",
     "logs",
     "traces",
     "metrics"
 ]
-version = "1716541742!11.0.0"
+version = "1716541850!10.1.0"
 dependencies = []
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `grafana_foundation_sdk-1716541742!11.0.0/PKG-INFO` & `grafana_foundation_sdk-1716541850!10.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grafana_foundation_sdk
-Version: 1716541742!11.0.0
+Version: 1716541850!10.1.0
 Summary: A set of tools, types and libraries for building and manipulating Grafana objects.
 Project-URL: Homepage, https://github.com/grafana/grafana-foundation-sdk
 Project-URL: Repository, https://github.com/grafana/grafana-foundation-sdk.git
 Project-URL: Issues, https://github.com/grafana/grafana-foundation-sdk/issues
 Author: Grafana Labs
 License-File: LICENSE.md
 Keywords: grafana,logs,metrics,observability,sdk,traces
@@ -21,21 +21,21 @@
 Description-Content-Type: text/markdown
 
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v11.0.x.**
+> This branch contains **types and builders generated for Grafana v10.1.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1716541742!11.0.0'
+python3 -m pip install 'grafana_foundation_sdk==1716541850!10.1.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```


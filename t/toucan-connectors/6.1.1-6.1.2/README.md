# Comparing `tmp/toucan_connectors-6.1.1.tar.gz` & `tmp/toucan_connectors-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toucan_connectors-6.1.1.tar", max compression
+gzip compressed data, was "toucan_connectors-6.1.2.tar", max compression
```

## Comparing `toucan_connectors-6.1.1.tar` & `toucan_connectors-6.1.2.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0     1510 2019-04-24 08:29:11.299050 toucan_connectors-6.1.1/LICENSE
--rw-r--r--   0        0        0     9964 2024-03-18 10:21:58.580641 toucan_connectors-6.1.1/README.md
--rw-r--r--   0        0        0     5483 2024-03-18 10:49:11.910522 toucan_connectors-6.1.1/pyproject.toml
--rw-r--r--   0        0        0     8622 2024-03-18 10:21:58.624650 toucan_connectors-6.1.1/toucan_connectors/__init__.py
--rw-r--r--   0        0        0     4586 2024-03-18 10:21:58.624650 toucan_connectors-6.1.1/toucan_connectors/auth.py
--rw-r--r--   0        0        0    61900 2020-07-20 15:29:42.450505 toucan_connectors-6.1.1/toucan_connectors/aws/aws.png
--rw-r--r--   0        0        0        0 2022-06-20 06:28:51.009430 toucan_connectors-6.1.1/toucan_connectors/awsathena/__init__.py
--rw-r--r--   0        0        0     2524 2022-06-20 06:28:51.009430 toucan_connectors-6.1.1/toucan_connectors/awsathena/athena.png
--rw-r--r--   0        0        0     8470 2024-03-18 10:21:58.624650 toucan_connectors-6.1.1/toucan_connectors/awsathena/awsathena_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.323050 toucan_connectors-6.1.1/toucan_connectors/azure_mssql/__init__.py
--rw-r--r--   0        0        0     2504 2024-03-18 10:21:58.628651 toucan_connectors-6.1.1/toucan_connectors/azure_mssql/azure_mssql_connector.py
--rw-r--r--   0        0        0    24249 2020-07-20 15:29:42.450505 toucan_connectors-6.1.1/toucan_connectors/azure_mssql/sql-azure.png
--rw-r--r--   0        0        0        0 2022-06-20 06:28:51.013430 toucan_connectors-6.1.1/toucan_connectors/clickhouse/__init__.py
--rw-r--r--   0        0        0     1780 2022-06-20 06:28:51.013430 toucan_connectors-6.1.1/toucan_connectors/clickhouse/clickhouse.png
--rw-r--r--   0        0        0     5013 2024-03-18 10:21:58.628651 toucan_connectors-6.1.1/toucan_connectors/clickhouse/clickhouse_connector.py
--rw-r--r--   0        0        0    15822 2024-03-18 10:21:58.628651 toucan_connectors-6.1.1/toucan_connectors/common.py
--rw-r--r--   0        0        0     5443 2024-03-18 10:21:58.628651 toucan_connectors-6.1.1/toucan_connectors/condition_translator.py
--rw-r--r--   0        0        0     8002 2024-03-18 10:21:58.628651 toucan_connectors-6.1.1/toucan_connectors/connection_manager.py
--rw-r--r--   0        0        0     3534 2022-06-20 06:28:51.013430 toucan_connectors-6.1.1/toucan_connectors/databricks/databricks.png
--rw-r--r--   0        0        0     5550 2024-03-18 10:21:58.628651 toucan_connectors-6.1.1/toucan_connectors/databricks/databricks_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.323050 toucan_connectors-6.1.1/toucan_connectors/dataiku/__init__.py
--rw-r--r--   0        0        0    10971 2020-07-20 15:29:42.450505 toucan_connectors-6.1.1/toucan_connectors/dataiku/dataiku.png
--rw-r--r--   0        0        0     1109 2024-03-18 10:21:58.628651 toucan_connectors-6.1.1/toucan_connectors/dataiku/dataiku_connector.py
--rwxr-xr-x   0        0        0      235 2020-07-20 15:29:42.450505 toucan_connectors-6.1.1/toucan_connectors/default-logo.png
--rw-r--r--   0        0        0     3331 2020-07-20 15:29:42.450505 toucan_connectors-6.1.1/toucan_connectors/denodo/denodo.png
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.323050 toucan_connectors-6.1.1/toucan_connectors/elasticsearch/__init__.py
--rw-r--r--   0        0        0    29549 2020-07-20 15:29:42.450505 toucan_connectors-6.1.1/toucan_connectors/elasticsearch/elasticsearch.png
--rw-r--r--   0        0        0     5949 2024-03-18 10:49:11.910522 toucan_connectors-6.1.1/toucan_connectors/elasticsearch/elasticsearch_connector.py
--rw-r--r--   0        0        0    13001 2021-01-18 08:06:18.610354 toucan_connectors-6.1.1/toucan_connectors/github/GitHub_Logo.png
--rw-r--r--   0        0        0      412 2022-06-20 06:28:51.017430 toucan_connectors-6.1.1/toucan_connectors/github/doc.md
--rw-r--r--   0        0        0    16983 2024-03-18 10:21:58.628651 toucan_connectors-6.1.1/toucan_connectors/github/github_connector.py
--rw-r--r--   0        0        0    15882 2024-03-18 10:21:58.632652 toucan_connectors-6.1.1/toucan_connectors/github/helpers.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.323050 toucan_connectors-6.1.1/toucan_connectors/google_analytics/__init__.py
--rw-r--r--   0        0        0     6243 2020-07-20 15:29:42.450505 toucan_connectors-6.1.1/toucan_connectors/google_analytics/google-analytics.png
--rw-r--r--   0        0        0     6738 2024-03-18 10:21:58.632652 toucan_connectors-6.1.1/toucan_connectors/google_analytics/google_analytics_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.323050 toucan_connectors-6.1.1/toucan_connectors/google_big_query/__init__.py
--rw-r--r--   0        0        0    17667 2020-07-20 15:29:42.450505 toucan_connectors-6.1.1/toucan_connectors/google_big_query/google-bigquery.png
--rw-r--r--   0        0        0    20940 2024-03-18 10:21:58.632652 toucan_connectors-6.1.1/toucan_connectors/google_big_query/google_big_query_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.323050 toucan_connectors-6.1.1/toucan_connectors/google_cloud_mysql/__init__.py
--rw-r--r--   0        0        0    24008 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
--rw-r--r--   0        0        0     2588 2024-03-18 10:21:58.632652 toucan_connectors-6.1.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
--rw-r--r--   0        0        0     2937 2024-03-18 10:21:58.632652 toucan_connectors-6.1.1/toucan_connectors/google_credentials.py
--rw-r--r--   0        0        0        0 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/google_sheets/__init__.py
--rw-r--r--   0        0        0    14238 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/google_sheets/google-sheets.png
--rw-r--r--   0        0        0     9381 2024-03-18 10:21:58.632652 toucan_connectors-6.1.1/toucan_connectors/google_sheets/google_sheets_connector.py
--rw-r--r--   0        0        0        0 2020-11-23 13:33:53.879064 toucan_connectors-6.1.1/toucan_connectors/google_sheets_2/__init__.py
--rw-r--r--   0        0        0      361 2022-06-20 06:28:51.021430 toucan_connectors-6.1.1/toucan_connectors/google_sheets_2/doc.md
--rw-r--r--   0        0        0     9906 2024-03-18 10:21:58.632652 toucan_connectors-6.1.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.323050 toucan_connectors-6.1.1/toucan_connectors/google_spreadsheet/__init__.py
--rw-r--r--   0        0        0    14238 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png
--rw-r--r--   0        0        0     2945 2024-03-18 10:21:58.632652 toucan_connectors-6.1.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.323050 toucan_connectors-6.1.1/toucan_connectors/http_api/__init__.py
--rw-r--r--   0        0        0    19694 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/http_api/http-api.png
--rw-r--r--   0        0        0     8436 2024-03-18 10:21:58.632652 toucan_connectors-6.1.1/toucan_connectors/http_api/http_api_connector.py
--rw-r--r--   0        0        0        0 2023-10-18 16:04:44.333520 toucan_connectors-6.1.1/toucan_connectors/hubspot_private_app/__init__.py
--rw-r--r--   0        0        0    33203 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/hubspot_private_app/hubspot.png
--rw-r--r--   0        0        0     5036 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/hubspot_private_app/hubspot_connector.py
--rw-r--r--   0        0        0      140 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/install_scripts/__init__.py
--rwxr-xr-x   0        0        0      657 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/install_scripts/databricks.sh
--rwxr-xr-x   0        0        0      728 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/install_scripts/mssql.sh
--rwxr-xr-x   0        0        0     1144 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
--rwxr-xr-x   0        0        0      908 2022-06-20 06:28:51.025430 toucan_connectors-6.1.1/toucan_connectors/install_scripts/odbc.sh
--rwxr-xr-x   0        0        0      590 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/install_scripts/oracle.sh
--rw-r--r--   0        0        0     3285 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/json_wrapper.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.327050 toucan_connectors-6.1.1/toucan_connectors/mongo/__init__.py
--rw-r--r--   0        0        0    26880 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/mongo/mongo-db.png
--rw-r--r--   0        0        0    18178 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/mongo/mongo_connector.py
--rw-r--r--   0        0        0     1822 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/mongo/mongo_translator.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.327050 toucan_connectors-6.1.1/toucan_connectors/mssql/__init__.py
--rw-r--r--   0        0        0    26319 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/mssql/mssql.png
--rw-r--r--   0        0        0     4796 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/mssql/mssql_connector.py
--rw-r--r--   0        0        0        0 2022-06-20 06:28:51.029430 toucan_connectors-6.1.1/toucan_connectors/mssql_TLSv1_0/__init__.py
--rw-r--r--   0        0        0    26319 2022-06-20 06:28:51.029430 toucan_connectors-6.1.1/toucan_connectors/mssql_TLSv1_0/mssql.png
--rw-r--r--   0        0        0     5016 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.327050 toucan_connectors-6.1.1/toucan_connectors/mysql/__init__.py
--rw-r--r--   0        0        0     3761 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/mysql/mysql.png
--rw-r--r--   0        0        0    14675 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/mysql/mysql_connector.py
--rw-r--r--   0        0        0        0 2020-11-23 13:33:53.879064 toucan_connectors-6.1.1/toucan_connectors/oauth2_connector/__init__.py
--rw-r--r--   0        0        0     5874 2024-03-18 10:21:58.636653 toucan_connectors-6.1.1/toucan_connectors/oauth2_connector/oauth2connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.327050 toucan_connectors-6.1.1/toucan_connectors/odata/__init__.py
--rw-r--r--   0        0        0    31781 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/odata/odata.png
--rw-r--r--   0        0        0     2068 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/odata/odata_connector.py
--rw-r--r--   0        0        0        0 2020-11-23 13:33:53.879064 toucan_connectors-6.1.1/toucan_connectors/odbc/__init__.py
--rw-r--r--   0        0        0     3141 2020-11-23 13:33:53.879064 toucan_connectors-6.1.1/toucan_connectors/odbc/odbc.png
--rw-r--r--   0        0        0     1349 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/odbc/odbc_connector.py
--rw-r--r--   0        0        0    10551 2022-06-20 06:28:51.029430 toucan_connectors-6.1.1/toucan_connectors/one_drive/one_drive.png
--rwxr-xr-x   0        0        0    12336 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/one_drive/one_drive_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.327050 toucan_connectors-6.1.1/toucan_connectors/oracle_sql/__init__.py
--rw-r--r--   0        0        0    12887 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/oracle_sql/oracle-sql.png
--rw-r--r--   0        0        0     3492 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/oracle_sql/oracle_sql_connector.py
--rw-r--r--   0        0        0     3893 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/pagination.py
--rw-r--r--   0        0        0     2657 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/pandas_translator.py
--rw-r--r--   0        0        0        0 2023-10-18 16:04:44.333520 toucan_connectors-6.1.1/toucan_connectors/peakina/__init__.py
--rw-r--r--   0        0        0     1377 2023-10-18 16:04:44.333520 toucan_connectors-6.1.1/toucan_connectors/peakina/peakina.png
--rw-r--r--   0        0        0      539 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/peakina/peakina_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.327050 toucan_connectors-6.1.1/toucan_connectors/postgres/__init__.py
--rw-r--r--   0        0        0    28440 2020-07-20 15:29:42.454505 toucan_connectors-6.1.1/toucan_connectors/postgres/postgres.png
--rw-r--r--   0        0        0    10656 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/postgres/postgresql_connector.py
--rw-r--r--   0        0        0    19780 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/postgres/utils.py
--rw-r--r--   0        0        0     1440 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/query_manager.py
--rw-r--r--   0        0        0        0 2022-06-20 06:28:51.033430 toucan_connectors-6.1.1/toucan_connectors/redshift/__init__.py
--rw-r--r--   0        0        0     8867 2022-06-20 06:28:51.033430 toucan_connectors-6.1.1/toucan_connectors/redshift/redshift.png
--rw-r--r--   0        0        0    16907 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/redshift/redshift_database_connector.py
--rw-r--r--   0        0        0     1836 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/redshift/utils.py
--rw-r--r--   0        0        0        0 2023-10-18 16:04:44.333520 toucan_connectors-6.1.1/toucan_connectors/s3/__init__.py
--rw-r--r--   0        0        0    43569 2023-10-18 16:04:44.333520 toucan_connectors-6.1.1/toucan_connectors/s3/s3.png
--rw-r--r--   0        0        0     5932 2024-03-18 10:21:58.640653 toucan_connectors-6.1.1/toucan_connectors/s3/s3_connector.py
--rw-r--r--   0        0        0      410 2022-06-20 06:28:51.033430 toucan_connectors-6.1.1/toucan_connectors/salesforce/doc.md
--rw-r--r--   0        0        0   165347 2022-06-20 06:28:51.037430 toucan_connectors-6.1.1/toucan_connectors/salesforce/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2022-06-20 06:28:51.037430 toucan_connectors-6.1.1/toucan_connectors/salesforce/salesforce.jpg
--rw-r--r--   0        0        0     7319 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/salesforce/salesforce_connector.py
--rw-r--r--   0        0        0      410 2022-06-20 06:28:51.037430 toucan_connectors-6.1.1/toucan_connectors/salesforce_sandbox/doc.md
--rw-r--r--   0        0        0   165347 2022-06-20 06:28:51.037430 toucan_connectors-6.1.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2022-06-20 06:28:51.041430 toucan_connectors-6.1.1/toucan_connectors/salesforce_sandbox/salesforce.jpg
--rw-r--r--   0        0        0       84 2022-06-20 06:28:51.041430 toucan_connectors-6.1.1/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
--rw-r--r--   0        0        0        0 2019-04-24 08:29:11.327050 toucan_connectors-6.1.1/toucan_connectors/sap_hana/__init__.py
--rw-r--r--   0        0        0    20257 2020-07-20 15:29:42.458505 toucan_connectors-6.1.1/toucan_connectors/sap_hana/sap-hana.png
--rw-r--r--   0        0        0     1364 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/sap_hana/sap_hana_connector.py
--rw-r--r--   0        0        0    20013 2022-06-20 06:28:51.041430 toucan_connectors-6.1.1/toucan_connectors/share_point/share_point.png
--rw-r--r--   0        0        0      162 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/snowflake/__init__.py
--rw-r--r--   0        0        0    15417 2020-07-20 15:29:42.458505 toucan_connectors-6.1.1/toucan_connectors/snowflake/snowflake.png
--rw-r--r--   0        0        0    18694 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/snowflake/snowflake_connector.py
--rw-r--r--   0        0        0    12786 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/snowflake_common.py
--rw-r--r--   0        0        0        0 2022-06-20 06:28:51.041430 toucan_connectors-6.1.1/toucan_connectors/snowflake_oauth2/__init__.py
--rw-r--r--   0        0        0    15417 2022-06-20 06:28:51.041430 toucan_connectors-6.1.1/toucan_connectors/snowflake_oauth2/snowflake.png
--rw-r--r--   0        0        0    12114 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
--rw-r--r--   0        0        0        0 2022-06-20 06:28:51.041430 toucan_connectors-6.1.1/toucan_connectors/soap/__init__.py
--rw-r--r--   0        0        0      609 2022-06-20 06:28:51.041430 toucan_connectors-6.1.1/toucan_connectors/soap/helpers.py
--rw-r--r--   0        0        0    42145 2022-06-20 06:28:51.041430 toucan_connectors-6.1.1/toucan_connectors/soap/soap.png
--rw-r--r--   0        0        0     4509 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/soap/soap_connector.py
--rw-r--r--   0        0        0     3064 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/sql_query_helper.py
--rw-r--r--   0        0        0    20594 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/toucan_connector.py
--rw-r--r--   0        0        0        0 2022-08-31 09:41:10.973436 toucan_connectors-6.1.1/toucan_connectors/utils/__init__.py
--rw-r--r--   0        0        0      492 2022-10-07 07:29:14.573908 toucan_connectors-6.1.1/toucan_connectors/utils/datetime.py
--rw-r--r--   0        0        0     2620 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/utils/json_to_table.py
--rw-r--r--   0        0        0      629 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/utils/pem.py
--rw-r--r--   0        0        0      231 2024-03-18 10:21:58.644654 toucan_connectors-6.1.1/toucan_connectors/utils/slugify.py
--rw-r--r--   0        0        0    14044 1970-01-01 00:00:00.000000 toucan_connectors-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1510 2024-04-18 10:01:12.122791 toucan_connectors-6.1.2/LICENSE
+-rw-r--r--   0        0        0     9964 2024-04-18 10:01:12.122791 toucan_connectors-6.1.2/README.md
+-rw-r--r--   0        0        0     5484 2024-04-18 10:01:12.126791 toucan_connectors-6.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8622 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/__init__.py
+-rw-r--r--   0        0        0     4586 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/auth.py
+-rw-r--r--   0        0        0    61900 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/aws/aws.png
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/awsathena/__init__.py
+-rw-r--r--   0        0        0     2524 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/awsathena/athena.png
+-rw-r--r--   0        0        0     8470 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/awsathena/awsathena_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/azure_mssql/__init__.py
+-rw-r--r--   0        0        0     2504 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/azure_mssql/azure_mssql_connector.py
+-rw-r--r--   0        0        0    24249 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/azure_mssql/sql-azure.png
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1780 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/clickhouse/clickhouse.png
+-rw-r--r--   0        0        0     5013 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/clickhouse/clickhouse_connector.py
+-rw-r--r--   0        0        0    15822 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/common.py
+-rw-r--r--   0        0        0     5443 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/condition_translator.py
+-rw-r--r--   0        0        0     8002 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/connection_manager.py
+-rw-r--r--   0        0        0     3534 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/databricks/databricks.png
+-rw-r--r--   0        0        0     5550 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/databricks/databricks_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/dataiku/__init__.py
+-rw-r--r--   0        0        0    10971 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/dataiku/dataiku.png
+-rw-r--r--   0        0        0     1109 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/dataiku/dataiku_connector.py
+-rwxr-xr-x   0        0        0      235 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/default-logo.png
+-rw-r--r--   0        0        0     3331 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/denodo/denodo.png
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    29549 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/elasticsearch/elasticsearch.png
+-rw-r--r--   0        0        0     5949 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/elasticsearch/elasticsearch_connector.py
+-rw-r--r--   0        0        0    13001 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/github/GitHub_Logo.png
+-rw-r--r--   0        0        0      412 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/github/doc.md
+-rw-r--r--   0        0        0    16983 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/github/github_connector.py
+-rw-r--r--   0        0        0    15882 2024-04-18 10:01:12.138791 toucan_connectors-6.1.2/toucan_connectors/github/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_analytics/__init__.py
+-rw-r--r--   0        0        0     6243 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_analytics/google-analytics.png
+-rw-r--r--   0        0        0     6738 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_analytics/google_analytics_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_big_query/__init__.py
+-rw-r--r--   0        0        0    17667 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_big_query/google-bigquery.png
+-rw-r--r--   0        0        0    20944 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_big_query/google_big_query_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_cloud_mysql/__init__.py
+-rw-r--r--   0        0        0    24008 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
+-rw-r--r--   0        0        0     2588 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
+-rw-r--r--   0        0        0     2937 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_credentials.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_sheets/__init__.py
+-rw-r--r--   0        0        0    14238 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_sheets/google-sheets.png
+-rw-r--r--   0        0        0     9381 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_sheets/google_sheets_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_sheets_2/__init__.py
+-rw-r--r--   0        0        0      361 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_sheets_2/doc.md
+-rw-r--r--   0        0        0     9906 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_spreadsheet/__init__.py
+-rw-r--r--   0        0        0    14238 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_spreadsheet/google-spreadsheet.png
+-rw-r--r--   0        0        0     2945 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/http_api/__init__.py
+-rw-r--r--   0        0        0    19694 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/http_api/http-api.png
+-rw-r--r--   0        0        0     8436 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/http_api/http_api_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/hubspot_private_app/__init__.py
+-rw-r--r--   0        0        0    33203 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/hubspot_private_app/hubspot.png
+-rw-r--r--   0        0        0     5036 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/hubspot_private_app/hubspot_connector.py
+-rw-r--r--   0        0        0      140 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/install_scripts/__init__.py
+-rwxr-xr-x   0        0        0      657 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/install_scripts/databricks.sh
+-rwxr-xr-x   0        0        0      728 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/install_scripts/mssql.sh
+-rwxr-xr-x   0        0        0     1144 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
+-rwxr-xr-x   0        0        0      908 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/install_scripts/odbc.sh
+-rwxr-xr-x   0        0        0      590 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/install_scripts/oracle.sh
+-rw-r--r--   0        0        0     3285 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/json_wrapper.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mongo/__init__.py
+-rw-r--r--   0        0        0    26880 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mongo/mongo-db.png
+-rw-r--r--   0        0        0    18178 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mongo/mongo_connector.py
+-rw-r--r--   0        0        0     1822 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mongo/mongo_translator.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mssql/__init__.py
+-rw-r--r--   0        0        0    26319 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mssql/mssql.png
+-rw-r--r--   0        0        0     4796 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mssql/mssql_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mssql_TLSv1_0/__init__.py
+-rw-r--r--   0        0        0    26319 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mssql_TLSv1_0/mssql.png
+-rw-r--r--   0        0        0     5016 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mysql/__init__.py
+-rw-r--r--   0        0        0     3761 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mysql/mysql.png
+-rw-r--r--   0        0        0    14675 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/mysql/mysql_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/oauth2_connector/__init__.py
+-rw-r--r--   0        0        0     5874 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/oauth2_connector/oauth2connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/odata/__init__.py
+-rw-r--r--   0        0        0    31781 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/odata/odata.png
+-rw-r--r--   0        0        0     2068 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/odata/odata_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/odbc/__init__.py
+-rw-r--r--   0        0        0     3141 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/odbc/odbc.png
+-rw-r--r--   0        0        0     1349 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/odbc/odbc_connector.py
+-rw-r--r--   0        0        0    10551 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/one_drive/one_drive.png
+-rwxr-xr-x   0        0        0    12336 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/one_drive/one_drive_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/oracle_sql/__init__.py
+-rw-r--r--   0        0        0    12887 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/oracle_sql/oracle-sql.png
+-rw-r--r--   0        0        0     3492 2024-04-18 10:01:12.142791 toucan_connectors-6.1.2/toucan_connectors/oracle_sql/oracle_sql_connector.py
+-rw-r--r--   0        0        0     3893 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/pagination.py
+-rw-r--r--   0        0        0     2657 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/pandas_translator.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/peakina/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/peakina/peakina.png
+-rw-r--r--   0        0        0      539 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/peakina/peakina_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/postgres/__init__.py
+-rw-r--r--   0        0        0    28440 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/postgres/postgres.png
+-rw-r--r--   0        0        0    10656 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/postgres/postgresql_connector.py
+-rw-r--r--   0        0        0    19780 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/postgres/utils.py
+-rw-r--r--   0        0        0     1440 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/query_manager.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/redshift/__init__.py
+-rw-r--r--   0        0        0     8867 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/redshift/redshift.png
+-rw-r--r--   0        0        0    16907 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/redshift/redshift_database_connector.py
+-rw-r--r--   0        0        0     1836 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/redshift/utils.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/s3/__init__.py
+-rw-r--r--   0        0        0    43569 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/s3/s3.png
+-rw-r--r--   0        0        0     5932 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/s3/s3_connector.py
+-rw-r--r--   0        0        0      410 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/salesforce/doc.md
+-rw-r--r--   0        0        0   165347 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/salesforce/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/salesforce/salesforce.jpg
+-rw-r--r--   0        0        0     7319 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/salesforce/salesforce_connector.py
+-rw-r--r--   0        0        0      410 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/salesforce_sandbox/doc.md
+-rw-r--r--   0        0        0   165347 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/salesforce_sandbox/salesforce.jpg
+-rw-r--r--   0        0        0       84 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/sap_hana/__init__.py
+-rw-r--r--   0        0        0    20257 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/sap_hana/sap-hana.png
+-rw-r--r--   0        0        0     1364 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/sap_hana/sap_hana_connector.py
+-rw-r--r--   0        0        0    20013 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/share_point/share_point.png
+-rw-r--r--   0        0        0      162 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/snowflake/__init__.py
+-rw-r--r--   0        0        0    15417 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/snowflake/snowflake.png
+-rw-r--r--   0        0        0    18694 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/snowflake/snowflake_connector.py
+-rw-r--r--   0        0        0    12786 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/snowflake_common.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/snowflake_oauth2/__init__.py
+-rw-r--r--   0        0        0    15417 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/snowflake_oauth2/snowflake.png
+-rw-r--r--   0        0        0    12114 2024-04-18 10:01:12.146791 toucan_connectors-6.1.2/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/soap/__init__.py
+-rw-r--r--   0        0        0      609 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/soap/helpers.py
+-rw-r--r--   0        0        0    42145 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/soap/soap.png
+-rw-r--r--   0        0        0     4509 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/soap/soap_connector.py
+-rw-r--r--   0        0        0     3064 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/sql_query_helper.py
+-rw-r--r--   0        0        0    20594 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/toucan_connector.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/utils/__init__.py
+-rw-r--r--   0        0        0      492 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/utils/datetime.py
+-rw-r--r--   0        0        0     2620 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/utils/json_to_table.py
+-rw-r--r--   0        0        0      629 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/utils/pem.py
+-rw-r--r--   0        0        0      231 2024-04-18 10:01:12.150791 toucan_connectors-6.1.2/toucan_connectors/utils/slugify.py
+-rw-r--r--   0        0        0    14045 1970-01-01 00:00:00.000000 toucan_connectors-6.1.2/PKG-INFO
```

### Comparing `toucan_connectors-6.1.1/LICENSE` & `toucan_connectors-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/README.md` & `toucan_connectors-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/pyproject.toml` & `toucan_connectors-6.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toucan-connectors"
-version = "6.1.1"
+version = "6.1.2"
 description = "Toucan Toco Connectors"
 authors = ["Toucan Toco <dev@toucantoco.com>"]
 license = "BSD"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
@@ -20,15 +20,15 @@
 pandas = [
     {version = "<2", python = "<3.12"},
     {version = ">=2", python = ">=3.12"},
 ]
 
 # Dependencies for extras
 oauthlib = {version = "3.2.2", optional = true}
-requests-oauthlib = {version = "1.4.0", optional = true}
+requests-oauthlib = {version = "2.0.0", optional = true}
 awswrangler = {version = "^3.0.0", optional = true}
 pyodbc = {version = ">=4,<6", optional = true}
 clickhouse-driver = {version = ">=0.2.3,<1.0", optional = true}
 dataiku-api-client = {version = ">=9.0.1,<13.0.0", optional = true}
 elasticsearch = {version = ">=7.11.0,<8", optional = true}
 python-graphql-client = {version = ">=0.4.3,<1.0", optional = true}
 google-api-python-client = {version = "^2", optional = true}
@@ -46,43 +46,43 @@
 PyJWT = {version = ">=1.5.3,<3", optional = true}
 simplejson = {version = "^3.17.6", optional = true}
 pyhdb = {version = ">=0.3.4,<1.0", optional = true}
 zeep = {version = "^4.1.0", optional = true}
 snowflake-connector-python = {version = ">=2.7.12,<4.0.0", optional = true}
 pyarrow = {version = "*", optional = true}
 peakina = {version = ">=0.11,<0.13", optional = true}
-hubspot-api-client = {version = ">=7.4,<9.0", optional = true}
+hubspot-api-client = {version = ">=7.4,<10.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 Authlib = "^1.0.1"
 aioresponses = ">=0.7.3,<1.0"
 click = "^8.1.7"
 cryptography = ">=40.0.2"
 docker = "^7.0.0"
 mock = "^5.1.0"
 pytest-aiohttp = "^1.0.5"
 pytest-asyncio = ">=0.19.0,<1"
-pytest-cov = "^4.1.0"
+pytest-cov = "^5.0.0"
 pytest = "^8.1.1"
-pytest-mock = "^3.12.0"
+pytest-mock = "^3.14.0"
 pytest-rerunfailures = "^14.0"
 PyYAML = ">=6.0.1,<7"
 responses = ">=0.21.0,<1"
 psycopg2 = "^2.9.9"
 xmltodict = ">=0.13.0,<1"
 python-graphql-client = ">=0.4.3,<1"
 clickhouse-driver = ">=0.2.3,<1"
-lxml = "5.1.0"
+lxml = "5.2.1"
 zeep = "^4.2.1"
 mypy = "^1.9"
-pandas-stubs = "^2.2.0.240218"
+pandas-stubs = "^2.2.1.240316"
 types-requests = "^2.31.0.6"
 types-simplejson = "^3.19.0.20240310"
 types-python-slugify = "^8.0.2.20240310"
-types-pyopenssl = "^24.0.0.20240311"
+types-pyopenssl = "^24.0.0.20240417"
 
 [tool.poetry.extras]
 awsathena = ["awswrangler"]
 azure_mssql = ["pyodbc"]
 clickhouse = ["clickhouse-driver"]
 dataiku = ["dataiku-api-client"]
 elasticsearch = ["elasticsearch"]
```

### Comparing `toucan_connectors-6.1.1/toucan_connectors/__init__.py` & `toucan_connectors-6.1.2/toucan_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/auth.py` & `toucan_connectors-6.1.2/toucan_connectors/auth.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/aws/aws.png` & `toucan_connectors-6.1.2/toucan_connectors/aws/aws.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/awsathena/athena.png` & `toucan_connectors-6.1.2/toucan_connectors/awsathena/athena.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/awsathena/awsathena_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/awsathena/awsathena_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/azure_mssql/azure_mssql_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/azure_mssql/azure_mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/azure_mssql/sql-azure.png` & `toucan_connectors-6.1.2/toucan_connectors/azure_mssql/sql-azure.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/clickhouse/clickhouse.png` & `toucan_connectors-6.1.2/toucan_connectors/clickhouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/clickhouse/clickhouse_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/clickhouse/clickhouse_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/common.py` & `toucan_connectors-6.1.2/toucan_connectors/common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/condition_translator.py` & `toucan_connectors-6.1.2/toucan_connectors/condition_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/connection_manager.py` & `toucan_connectors-6.1.2/toucan_connectors/connection_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/databricks/databricks.png` & `toucan_connectors-6.1.2/toucan_connectors/databricks/databricks.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/databricks/databricks_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/databricks/databricks_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/dataiku/dataiku.png` & `toucan_connectors-6.1.2/toucan_connectors/dataiku/dataiku.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/dataiku/dataiku_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/dataiku/dataiku_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/denodo/denodo.png` & `toucan_connectors-6.1.2/toucan_connectors/denodo/denodo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/elasticsearch/elasticsearch.png` & `toucan_connectors-6.1.2/toucan_connectors/elasticsearch/elasticsearch.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/elasticsearch/elasticsearch_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/elasticsearch/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/github/GitHub_Logo.png` & `toucan_connectors-6.1.2/toucan_connectors/github/GitHub_Logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/github/github_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/github/github_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/github/helpers.py` & `toucan_connectors-6.1.2/toucan_connectors/github/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_analytics/google-analytics.png` & `toucan_connectors-6.1.2/toucan_connectors/google_analytics/google-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_analytics/google_analytics_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/google_analytics/google_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_big_query/google-bigquery.png` & `toucan_connectors-6.1.2/toucan_connectors/google_big_query/google-bigquery.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_big_query/google_big_query_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/google_big_query/google_big_query_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,16 +372,16 @@
     C.table_name AS name,
     C.table_schema AS schema,
     T.table_catalog AS database,
     T.table_type AS type,
     C.column_name,
     C.data_type
 FROM
-    {dataset_id}.INFORMATION_SCHEMA.COLUMNS C
-    JOIN {dataset_id}.INFORMATION_SCHEMA.TABLES T
+    `{dataset_id}`.INFORMATION_SCHEMA.COLUMNS C
+    JOIN `{dataset_id}`.INFORMATION_SCHEMA.TABLES T
         ON C.table_name = T.table_name
 WHERE
     IS_SYSTEM_DEFINED = 'NO'
     AND IS_HIDDEN = 'NO'
 """
 
         if db_name is not None:
```

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png` & `toucan_connectors-6.1.2/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_credentials.py` & `toucan_connectors-6.1.2/toucan_connectors/google_credentials.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_sheets/google-sheets.png` & `toucan_connectors-6.1.2/toucan_connectors/google_sheets/google-sheets.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_sheets/google_sheets_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/google_sheets/google_sheets_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/google_sheets_2/google_sheets_2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png` & `toucan_connectors-6.1.2/toucan_connectors/google_spreadsheet/google-spreadsheet.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/http_api/http-api.png` & `toucan_connectors-6.1.2/toucan_connectors/http_api/http-api.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/http_api/http_api_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/http_api/http_api_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/hubspot_private_app/hubspot.png` & `toucan_connectors-6.1.2/toucan_connectors/hubspot_private_app/hubspot.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/hubspot_private_app/hubspot_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/hubspot_private_app/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/install_scripts/databricks.sh` & `toucan_connectors-6.1.2/toucan_connectors/install_scripts/databricks.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/install_scripts/mssql.sh` & `toucan_connectors-6.1.2/toucan_connectors/install_scripts/mssql.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh` & `toucan_connectors-6.1.2/toucan_connectors/install_scripts/mssql_TLSv1_0.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/install_scripts/odbc.sh` & `toucan_connectors-6.1.2/toucan_connectors/install_scripts/odbc.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/install_scripts/oracle.sh` & `toucan_connectors-6.1.2/toucan_connectors/install_scripts/oracle.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/json_wrapper.py` & `toucan_connectors-6.1.2/toucan_connectors/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/mongo/mongo-db.png` & `toucan_connectors-6.1.2/toucan_connectors/mongo/mongo-db.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/mongo/mongo_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/mongo/mongo_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/mongo/mongo_translator.py` & `toucan_connectors-6.1.2/toucan_connectors/mongo/mongo_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/mssql/mssql.png` & `toucan_connectors-6.1.2/toucan_connectors/mssql/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/mssql/mssql_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/mssql/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/mssql_TLSv1_0/mssql.png` & `toucan_connectors-6.1.2/toucan_connectors/mssql_TLSv1_0/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/mssql_TLSv1_0/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/mysql/mysql.png` & `toucan_connectors-6.1.2/toucan_connectors/mysql/mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/mysql/mysql_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/mysql/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/oauth2_connector/oauth2connector.py` & `toucan_connectors-6.1.2/toucan_connectors/oauth2_connector/oauth2connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/odata/odata.png` & `toucan_connectors-6.1.2/toucan_connectors/odata/odata.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/odata/odata_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/odata/odata_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/odbc/odbc.png` & `toucan_connectors-6.1.2/toucan_connectors/odbc/odbc.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/odbc/odbc_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/odbc/odbc_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/one_drive/one_drive.png` & `toucan_connectors-6.1.2/toucan_connectors/one_drive/one_drive.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/one_drive/one_drive_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/one_drive/one_drive_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/oracle_sql/oracle-sql.png` & `toucan_connectors-6.1.2/toucan_connectors/oracle_sql/oracle-sql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/oracle_sql/oracle_sql_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/oracle_sql/oracle_sql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/pagination.py` & `toucan_connectors-6.1.2/toucan_connectors/pagination.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/pandas_translator.py` & `toucan_connectors-6.1.2/toucan_connectors/pandas_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/peakina/peakina.png` & `toucan_connectors-6.1.2/toucan_connectors/peakina/peakina.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/peakina/peakina_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/peakina/peakina_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/postgres/postgres.png` & `toucan_connectors-6.1.2/toucan_connectors/postgres/postgres.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/postgres/postgresql_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/postgres/postgresql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/postgres/utils.py` & `toucan_connectors-6.1.2/toucan_connectors/postgres/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/query_manager.py` & `toucan_connectors-6.1.2/toucan_connectors/query_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/redshift/redshift.png` & `toucan_connectors-6.1.2/toucan_connectors/redshift/redshift.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/redshift/redshift_database_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/redshift/redshift_database_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/redshift/utils.py` & `toucan_connectors-6.1.2/toucan_connectors/redshift/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/s3/s3.png` & `toucan_connectors-6.1.2/toucan_connectors/s3/s3.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/s3/s3_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/s3/s3_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/salesforce/salesforce-service-cloud.png` & `toucan_connectors-6.1.2/toucan_connectors/salesforce/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/salesforce/salesforce.jpg` & `toucan_connectors-6.1.2/toucan_connectors/salesforce/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/salesforce/salesforce_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/salesforce/salesforce_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png` & `toucan_connectors-6.1.2/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/salesforce_sandbox/salesforce.jpg` & `toucan_connectors-6.1.2/toucan_connectors/salesforce_sandbox/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/sap_hana/sap-hana.png` & `toucan_connectors-6.1.2/toucan_connectors/sap_hana/sap-hana.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/sap_hana/sap_hana_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/sap_hana/sap_hana_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/share_point/share_point.png` & `toucan_connectors-6.1.2/toucan_connectors/share_point/share_point.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/snowflake/snowflake.png` & `toucan_connectors-6.1.2/toucan_connectors/snowflake/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/snowflake/snowflake_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/snowflake/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/snowflake_common.py` & `toucan_connectors-6.1.2/toucan_connectors/snowflake_common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/snowflake_oauth2/snowflake.png` & `toucan_connectors-6.1.2/toucan_connectors/snowflake_oauth2/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/soap/helpers.py` & `toucan_connectors-6.1.2/toucan_connectors/soap/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/soap/soap.png` & `toucan_connectors-6.1.2/toucan_connectors/soap/soap.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/soap/soap_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/soap/soap_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/sql_query_helper.py` & `toucan_connectors-6.1.2/toucan_connectors/sql_query_helper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/toucan_connector.py` & `toucan_connectors-6.1.2/toucan_connectors/toucan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/utils/json_to_table.py` & `toucan_connectors-6.1.2/toucan_connectors/utils/json_to_table.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/toucan_connectors/utils/pem.py` & `toucan_connectors-6.1.2/toucan_connectors/utils/pem.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-6.1.1/PKG-INFO` & `toucan_connectors-6.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toucan-connectors
-Version: 6.1.1
+Version: 6.1.2
 Summary: Toucan Toco Connectors
 License: BSD
 Author: Toucan Toco
 Author-email: dev@toucantoco.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -46,15 +46,15 @@
 Requires-Dist: clickhouse-driver (>=0.2.3,<1.0) ; extra == "clickhouse" or extra == "all"
 Requires-Dist: cx-Oracle (>=8.3.0,<9.0.0) ; extra == "oracle-sql" or extra == "all"
 Requires-Dist: dataiku-api-client (>=9.0.1,<13.0.0) ; extra == "dataiku" or extra == "all"
 Requires-Dist: elasticsearch (>=7.11.0,<8) ; extra == "elasticsearch" or extra == "all"
 Requires-Dist: google-api-python-client (>=2,<3) ; extra == "google-analytics" or extra == "google-sheets" or extra == "all"
 Requires-Dist: google-cloud-bigquery[bqstorage,pandas] (>=3,<4) ; extra == "google-big-query" or extra == "all"
 Requires-Dist: gspread (>=5.4,<7.0) ; extra == "google-spreadsheet" or extra == "all"
-Requires-Dist: hubspot-api-client (>=7.4,<9.0) ; extra == "hubspot" or extra == "all"
+Requires-Dist: hubspot-api-client (>=7.4,<10.0) ; extra == "hubspot" or extra == "all"
 Requires-Dist: jq (>=1.2.2,<2.0.0)
 Requires-Dist: lxml (>=4.6.5,<6.0.0) ; extra == "redshift" or extra == "soap" or extra == "all"
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0) ; extra == "google-analytics" or extra == "google-spreadsheet" or extra == "all"
 Requires-Dist: oauthlib (==3.2.2) ; extra == "http-api" or extra == "odata" or extra == "all"
 Requires-Dist: pandas (<2) ; python_version < "3.12"
 Requires-Dist: pandas (>=2) ; python_version >= "3.12"
 Requires-Dist: peakina (>=0.11,<0.13) ; extra == "all"
@@ -64,15 +64,15 @@
 Requires-Dist: pyhdb (>=0.3.4,<1.0) ; extra == "sap-hana" or extra == "all"
 Requires-Dist: pymongo (>=3.12.0) ; extra == "mongo" or extra == "all"
 Requires-Dist: pyodbc (>=4,<6) ; extra == "azure-mssql" or extra == "mssql" or extra == "mssql-tlsv1-0" or extra == "all"
 Requires-Dist: python-graphql-client (>=0.4.3,<1.0) ; extra == "github" or extra == "all"
 Requires-Dist: python-slugify (>=5.0.2)
 Requires-Dist: redshift-connector (>=2.0.907,<3.0.0) ; extra == "redshift" or extra == "all"
 Requires-Dist: requests (>=2.28.0,<3.0.0)
-Requires-Dist: requests-oauthlib (==1.4.0) ; extra == "http-api" or extra == "odata" or extra == "all"
+Requires-Dist: requests-oauthlib (==2.0.0) ; extra == "http-api" or extra == "odata" or extra == "all"
 Requires-Dist: simplejson (>=3.17.6,<4.0.0) ; extra == "all"
 Requires-Dist: snowflake-connector-python (>=2.7.12,<4.0.0) ; extra == "snowflake" or extra == "all"
 Requires-Dist: tctc-odata (>=0.3,<1.0) ; extra == "odata" or extra == "all"
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<1.0) ; extra == "http-api" or extra == "all"
 Requires-Dist: zeep (>=4.1.0,<5.0.0) ; extra == "soap" or extra == "all"
 Description-Content-Type: text/markdown
```


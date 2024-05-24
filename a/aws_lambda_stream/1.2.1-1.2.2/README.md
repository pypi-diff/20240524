# Comparing `tmp/aws_lambda_stream-1.2.1.tar.gz` & `tmp/aws_lambda_stream-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_stream-1.2.1.tar", max compression
+gzip compressed data, was "aws_lambda_stream-1.2.2.tar", max compression
```

## Comparing `aws_lambda_stream-1.2.1.tar` & `aws_lambda_stream-1.2.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1076 2023-02-08 05:37:14.950615 aws_lambda_stream-1.2.1/LICENSE
--rw-r--r--   0        0        0      882 2023-07-20 01:42:51.651718 aws_lambda_stream-1.2.1/README.md
--rw-r--r--   0        0        0      747 2023-03-22 23:49:01.698319 aws_lambda_stream-1.2.1/aws_lambda_stream/__init__.py
--rw-r--r--   0        0        0      409 2023-03-23 15:58:19.551309 aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/__init__.py
--rw-r--r--   0        0        0      245 2024-04-05 05:09:27.902257 aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/cloudwatch.py
--rw-r--r--   0        0        0     3249 2024-04-05 05:09:30.949910 aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/dynamodb.py
--rw-r--r--   0        0        0     3509 2022-11-10 14:59:59.886154 aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/elasticsearch.py
--rw-r--r--   0        0        0      260 2024-04-05 05:06:54.782848 aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/eventbridge.py
--rw-r--r--   0        0        0      224 2024-04-05 05:09:42.303801 aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/lambda_.py
--rw-r--r--   0        0        0      950 2024-04-05 05:09:52.136330 aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/s3.py
--rw-r--r--   0        0        0      715 2024-04-05 05:07:56.740726 aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/sns.py
--rw-r--r--   0        0        0      603 2024-04-05 05:08:13.436957 aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/sqs.py
--rw-r--r--   0        0        0       70 2022-09-07 12:25:07.481058 aws_lambda_stream-1.2.1/aws_lambda_stream/events/__init__.py
--rw-r--r--   0        0        0     4891 2023-10-24 23:27:55.788628 aws_lambda_stream-1.2.1/aws_lambda_stream/events/dynamodb.py
--rw-r--r--   0        0        0     1151 2023-10-24 23:22:13.708172 aws_lambda_stream-1.2.1/aws_lambda_stream/events/kinesis.py
--rw-r--r--   0        0        0     2299 2023-03-23 19:20:35.970538 aws_lambda_stream-1.2.1/aws_lambda_stream/events/s3.py
--rw-r--r--   0        0        0     2073 2023-02-03 18:24:04.276592 aws_lambda_stream-1.2.1/aws_lambda_stream/events/sns.py
--rw-r--r--   0        0        0     1470 2023-02-03 18:24:04.277239 aws_lambda_stream-1.2.1/aws_lambda_stream/events/sqs.py
--rw-r--r--   0        0        0      172 2023-02-03 18:24:04.278143 aws_lambda_stream-1.2.1/aws_lambda_stream/filters/__init__.py
--rw-r--r--   0        0        0      204 2023-02-03 18:24:04.278452 aws_lambda_stream-1.2.1/aws_lambda_stream/filters/content.py
--rw-r--r--   0        0        0      639 2022-11-15 14:34:45.024830 aws_lambda_stream-1.2.1/aws_lambda_stream/filters/event_type.py
--rw-r--r--   0        0        0      754 2023-02-08 03:34:42.274970 aws_lambda_stream-1.2.1/aws_lambda_stream/filters/latch.py
--rw-r--r--   0        0        0      504 2023-02-03 18:24:04.278934 aws_lambda_stream-1.2.1/aws_lambda_stream/filters/skip.py
--rw-r--r--   0        0        0        0 2022-10-05 03:29:29.473147 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/__init__.py
--rw-r--r--   0        0        0     1033 2023-07-28 14:02:21.679238 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/cdc.py
--rw-r--r--   0        0        0     2487 2023-02-03 18:24:04.279800 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/collect.py
--rw-r--r--   0        0        0     2820 2023-02-03 18:24:04.280222 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/correlate.py
--rw-r--r--   0        0        0     1015 2023-07-28 14:02:21.679644 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/elasticsearch.py
--rw-r--r--   0        0        0     7265 2023-07-28 14:02:21.679983 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/evaluate.py
--rw-r--r--   0        0        0     1124 2023-06-20 04:55:40.314770 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/materialize.py
--rw-r--r--   0        0        0      992 2023-02-08 04:33:57.896213 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/s3.py
--rw-r--r--   0        0        0      896 2023-02-03 18:24:04.282923 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/sns.py
--rw-r--r--   0        0        0     2790 2023-07-28 14:02:21.680228 aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/task.py
--rw-r--r--   0        0        0     2791 2024-04-05 21:04:27.881136 aws_lambda_stream-1.2.1/aws_lambda_stream/pipelines/__init__.py
--rw-r--r--   0        0        0     3693 2023-04-06 14:36:11.361064 aws_lambda_stream-1.2.1/aws_lambda_stream/repositories/__init__.py
--rw-r--r--   0        0        0      436 2022-10-05 03:50:07.747050 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/__init__.py
--rw-r--r--   0        0        0     1361 2023-04-06 14:36:18.917107 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/apigateway.py
--rw-r--r--   0        0        0      140 2023-02-14 05:32:21.038521 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/aws.py
--rw-r--r--   0        0        0      153 2022-10-05 04:49:33.238263 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/batch.py
--rw-r--r--   0        0        0      538 2023-03-23 16:10:15.770876 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/cloudwatch.py
--rw-r--r--   0        0        0     1334 2023-06-21 01:32:44.777692 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/concurrency.py
--rw-r--r--   0        0        0      163 2022-10-05 04:43:54.856386 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/decorators.py
--rw-r--r--   0        0        0     5572 2023-04-10 01:56:19.355174 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/dynamodb.py
--rw-r--r--   0        0        0     2504 2023-07-28 14:02:21.681495 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/elasticsearch.py
--rw-r--r--   0        0        0     2439 2024-04-05 21:05:20.334856 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/eventbridge.py
--rw-r--r--   0        0        0     2660 2023-07-28 14:02:21.682559 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/faults.py
--rw-r--r--   0        0        0      413 2023-02-03 18:24:04.286668 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/filters.py
--rw-r--r--   0        0        0      333 2023-02-03 18:24:04.287082 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/json_encoder.py
--rw-r--r--   0        0        0      558 2023-03-01 04:10:54.251855 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/lambda_.py
--rw-r--r--   0        0        0      521 2024-04-05 21:06:15.853242 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/logger.py
--rw-r--r--   0        0        0     1982 2023-02-03 18:24:04.287769 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/operators.py
--rw-r--r--   0        0        0      253 2024-04-05 21:06:39.964257 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/opt.py
--rw-r--r--   0        0        0      345 2022-11-15 05:45:17.281224 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/pluralize.py
--rw-r--r--   0        0        0      646 2023-04-10 01:56:19.355426 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/retry.py
--rw-r--r--   0        0        0     2792 2023-03-22 23:47:26.627754 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/s3.py
--rw-r--r--   0        0        0      950 2023-03-03 19:53:38.454506 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/sns.py
--rw-r--r--   0        0        0      964 2023-02-09 19:19:31.634487 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/split.py
--rw-r--r--   0        0        0     1554 2024-04-05 21:06:58.476670 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/sqs.py
--rw-r--r--   0        0        0     1045 2023-09-23 16:57:24.696498 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/tags.py
--rw-r--r--   0        0        0      370 2023-02-03 18:24:04.288204 aws_lambda_stream-1.2.1/aws_lambda_stream/utils/time.py
--rw-r--r--   0        0        0      632 2024-04-05 21:08:46.479059 aws_lambda_stream-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 aws_lambda_stream-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-02-08 05:37:14.950615 aws_lambda_stream-1.2.2/LICENSE
+-rw-r--r--   0        0        0      882 2023-07-20 01:42:51.651718 aws_lambda_stream-1.2.2/README.md
+-rw-r--r--   0        0        0      747 2023-03-22 23:49:01.698319 aws_lambda_stream-1.2.2/aws_lambda_stream/__init__.py
+-rw-r--r--   0        0        0      409 2023-03-23 15:58:19.551309 aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/__init__.py
+-rw-r--r--   0        0        0      245 2024-04-05 05:09:27.902257 aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/cloudwatch.py
+-rw-r--r--   0        0        0     3249 2024-04-05 05:09:30.949910 aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/dynamodb.py
+-rw-r--r--   0        0        0     3509 2022-11-10 14:59:59.886154 aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/elasticsearch.py
+-rw-r--r--   0        0        0      260 2024-04-05 05:06:54.782848 aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/eventbridge.py
+-rw-r--r--   0        0        0      224 2024-04-05 05:09:42.303801 aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/lambda_.py
+-rw-r--r--   0        0        0      950 2024-04-05 05:09:52.136330 aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/s3.py
+-rw-r--r--   0        0        0      715 2024-04-05 05:07:56.740726 aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/sns.py
+-rw-r--r--   0        0        0      603 2024-04-05 05:08:13.436957 aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/sqs.py
+-rw-r--r--   0        0        0       70 2022-09-07 12:25:07.481058 aws_lambda_stream-1.2.2/aws_lambda_stream/events/__init__.py
+-rw-r--r--   0        0        0     4891 2023-10-24 23:27:55.788628 aws_lambda_stream-1.2.2/aws_lambda_stream/events/dynamodb.py
+-rw-r--r--   0        0        0     1151 2023-10-24 23:22:13.708172 aws_lambda_stream-1.2.2/aws_lambda_stream/events/kinesis.py
+-rw-r--r--   0        0        0     2299 2023-03-23 19:20:35.970538 aws_lambda_stream-1.2.2/aws_lambda_stream/events/s3.py
+-rw-r--r--   0        0        0     2073 2023-02-03 18:24:04.276592 aws_lambda_stream-1.2.2/aws_lambda_stream/events/sns.py
+-rw-r--r--   0        0        0     1470 2023-02-03 18:24:04.277239 aws_lambda_stream-1.2.2/aws_lambda_stream/events/sqs.py
+-rw-r--r--   0        0        0      172 2023-02-03 18:24:04.278143 aws_lambda_stream-1.2.2/aws_lambda_stream/filters/__init__.py
+-rw-r--r--   0        0        0      204 2023-02-03 18:24:04.278452 aws_lambda_stream-1.2.2/aws_lambda_stream/filters/content.py
+-rw-r--r--   0        0        0      639 2022-11-15 14:34:45.024830 aws_lambda_stream-1.2.2/aws_lambda_stream/filters/event_type.py
+-rw-r--r--   0        0        0      754 2023-02-08 03:34:42.274970 aws_lambda_stream-1.2.2/aws_lambda_stream/filters/latch.py
+-rw-r--r--   0        0        0      504 2023-02-03 18:24:04.278934 aws_lambda_stream-1.2.2/aws_lambda_stream/filters/skip.py
+-rw-r--r--   0        0        0        0 2022-10-05 03:29:29.473147 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/__init__.py
+-rw-r--r--   0        0        0     1033 2023-07-28 14:02:21.679238 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/cdc.py
+-rw-r--r--   0        0        0     2487 2023-02-03 18:24:04.279800 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/collect.py
+-rw-r--r--   0        0        0     2820 2023-02-03 18:24:04.280222 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/correlate.py
+-rw-r--r--   0        0        0     1015 2023-07-28 14:02:21.679644 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/elasticsearch.py
+-rw-r--r--   0        0        0     7265 2023-07-28 14:02:21.679983 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/evaluate.py
+-rw-r--r--   0        0        0     1124 2023-06-20 04:55:40.314770 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/materialize.py
+-rw-r--r--   0        0        0      992 2023-02-08 04:33:57.896213 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/s3.py
+-rw-r--r--   0        0        0      896 2023-02-03 18:24:04.282923 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/sns.py
+-rw-r--r--   0        0        0     2790 2023-07-28 14:02:21.680228 aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/task.py
+-rw-r--r--   0        0        0     2792 2024-05-24 04:12:42.514141 aws_lambda_stream-1.2.2/aws_lambda_stream/pipelines/__init__.py
+-rw-r--r--   0        0        0     3693 2023-04-06 14:36:11.361064 aws_lambda_stream-1.2.2/aws_lambda_stream/repositories/__init__.py
+-rw-r--r--   0        0        0      436 2022-10-05 03:50:07.747050 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/__init__.py
+-rw-r--r--   0        0        0     1361 2023-04-06 14:36:18.917107 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/apigateway.py
+-rw-r--r--   0        0        0      140 2023-02-14 05:32:21.038521 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/aws.py
+-rw-r--r--   0        0        0      153 2022-10-05 04:49:33.238263 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/batch.py
+-rw-r--r--   0        0        0      538 2023-03-23 16:10:15.770876 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/cloudwatch.py
+-rw-r--r--   0        0        0     1334 2023-06-21 01:32:44.777692 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/concurrency.py
+-rw-r--r--   0        0        0      163 2022-10-05 04:43:54.856386 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/decorators.py
+-rw-r--r--   0        0        0     5572 2023-04-10 01:56:19.355174 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/dynamodb.py
+-rw-r--r--   0        0        0     2504 2023-07-28 14:02:21.681495 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/elasticsearch.py
+-rw-r--r--   0        0        0     2439 2024-04-05 21:05:20.334856 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/eventbridge.py
+-rw-r--r--   0        0        0     2660 2023-07-28 14:02:21.682559 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/faults.py
+-rw-r--r--   0        0        0      413 2023-02-03 18:24:04.286668 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/filters.py
+-rw-r--r--   0        0        0      333 2023-02-03 18:24:04.287082 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/json_encoder.py
+-rw-r--r--   0        0        0      558 2023-03-01 04:10:54.251855 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/lambda_.py
+-rw-r--r--   0        0        0      521 2024-04-05 21:06:15.853242 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/logger.py
+-rw-r--r--   0        0        0     1982 2023-02-03 18:24:04.287769 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/operators.py
+-rw-r--r--   0        0        0      253 2024-04-05 21:06:39.964257 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/opt.py
+-rw-r--r--   0        0        0      345 2022-11-15 05:45:17.281224 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/pluralize.py
+-rw-r--r--   0        0        0      646 2023-04-10 01:56:19.355426 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/retry.py
+-rw-r--r--   0        0        0     2792 2023-03-22 23:47:26.627754 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/s3.py
+-rw-r--r--   0        0        0      950 2023-03-03 19:53:38.454506 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/sns.py
+-rw-r--r--   0        0        0      964 2023-02-09 19:19:31.634487 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/split.py
+-rw-r--r--   0        0        0     1554 2024-04-05 21:06:58.476670 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/sqs.py
+-rw-r--r--   0        0        0     1045 2023-09-23 16:57:24.696498 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/tags.py
+-rw-r--r--   0        0        0      370 2023-02-03 18:24:04.288204 aws_lambda_stream-1.2.2/aws_lambda_stream/utils/time.py
+-rw-r--r--   0        0        0      632 2024-05-24 04:01:34.321146 aws_lambda_stream-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 aws_lambda_stream-1.2.2/PKG-INFO
```

### Comparing `aws_lambda_stream-1.2.1/LICENSE` & `aws_lambda_stream-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/README.md` & `aws_lambda_stream-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/__init__.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/dynamodb.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/elasticsearch.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/s3.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/s3.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/sns.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/sns.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/connectors/sqs.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/connectors/sqs.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/events/dynamodb.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/events/dynamodb.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/events/kinesis.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/events/kinesis.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/events/s3.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/events/s3.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/events/sns.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/events/sns.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/events/sqs.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/events/sqs.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/filters/event_type.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/filters/event_type.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/filters/latch.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/filters/latch.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/cdc.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/cdc.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/collect.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/collect.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/correlate.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/correlate.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/elasticsearch.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/evaluate.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/evaluate.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/materialize.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/materialize.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/s3.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/s3.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/sns.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/sns.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/flavors/task.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/flavors/task.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/pipelines/__init__.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/pipelines/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
                     'pipeline': k,
                     **uow,
                 }),
                 self.the_pipelines[k](
                     {
                         'id': k,
                         'pipeline': copy.copy(k),
+                        'logger': logging.getLogger(k),
                         **self.opt,
-                        'logger': logging.getLogger(k)
                     }
                 )
             )
             p.id = k
             return p
 
         lines = list(map(make_lines, self.the_pipelines.keys()))
```

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/repositories/__init__.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/apigateway.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/apigateway.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/cloudwatch.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/concurrency.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/dynamodb.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/dynamodb.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/elasticsearch.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/eventbridge.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/eventbridge.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/faults.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/faults.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/lambda_.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/lambda_.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/logger.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/logger.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/operators.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/operators.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/retry.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/retry.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/s3.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/s3.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/sns.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/sns.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/split.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/split.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/sqs.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/sqs.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/aws_lambda_stream/utils/tags.py` & `aws_lambda_stream-1.2.2/aws_lambda_stream/utils/tags.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_stream-1.2.1/pyproject.toml` & `aws_lambda_stream-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws_lambda_stream"
-version = "1.2.1"
+version = "1.2.2"
 description = "Create stream processors with AWS Lambda functions"
 authors = ["Alejandro Hernández <clandro89@gmail.com>"]
 repository="https://github.com/clandro89/aws-lambda-stream"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `aws_lambda_stream-1.2.1/PKG-INFO` & `aws_lambda_stream-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_lambda_stream
-Version: 1.2.1
+Version: 1.2.2
 Summary: Create stream processors with AWS Lambda functions
 Home-page: https://github.com/clandro89/aws-lambda-stream
 Author: Alejandro Hernández
 Author-email: clandro89@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


# Comparing `tmp/osbot_aws-0.6.6.tar.gz` & `tmp/osbot_aws-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/osbot_aws-0.6.6.tar", last modified: Sat May 18 13:24:16 2019, max compression
+gzip compressed data, was "osbot_aws-2.5.0.tar", max compression
```

## Comparing `osbot_aws-0.6.6.tar` & `osbot_aws-2.5.0.tar`

### file list

```diff
@@ -1,64 +1,217 @@
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/
--rw-r--r--   0 dinis      (502) staff       (20)      509 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/PKG-INFO
--rw-r--r--   0 dinis      (502) staff       (20)       69 2019-04-07 09:13:27.000000 osbot_aws-0.6.6/README.md
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws/
--rw-r--r--   0 dinis      (502) staff       (20)      163 2019-04-11 14:38:57.000000 osbot_aws-0.6.6/osbot_aws/Globals.py
--rw-r--r--   0 dinis      (502) staff       (20)        0 2019-03-31 16:08:36.000000 osbot_aws-0.6.6/osbot_aws/__init__.py
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws/apis/
--rw-r--r--   0 dinis      (502) staff       (20)     2400 2019-04-10 22:38:50.000000 osbot_aws-0.6.6/osbot_aws/apis/Athena.py
--rw-r--r--   0 dinis      (502) staff       (20)      284 2019-04-06 14:27:18.000000 osbot_aws-0.6.6/osbot_aws/apis/Boto_Helpers.py
--rw-r--r--   0 dinis      (502) staff       (20)      780 2019-04-10 22:38:50.000000 osbot_aws-0.6.6/osbot_aws/apis/Cloud_Trail.py
--rw-r--r--   0 dinis      (502) staff       (20)      164 2019-04-10 22:38:50.000000 osbot_aws-0.6.6/osbot_aws/apis/Cloud_Watch.py
--rw-r--r--   0 dinis      (502) staff       (20)     3914 2019-04-10 22:41:28.000000 osbot_aws-0.6.6/osbot_aws/apis/CodeBuild.py
--rw-r--r--   0 dinis      (502) staff       (20)     5701 2019-04-13 17:07:48.000000 osbot_aws-0.6.6/osbot_aws/apis/Dynamo.py
--rw-r--r--   0 dinis      (502) staff       (20)     1507 2019-04-10 22:38:50.000000 osbot_aws-0.6.6/osbot_aws/apis/Ec2.py
--rw-r--r--   0 dinis      (502) staff       (20)     6695 2019-04-13 01:26:03.000000 osbot_aws-0.6.6/osbot_aws/apis/Fargate.py
--rw-r--r--   0 dinis      (502) staff       (20)     9822 2019-04-13 14:16:44.000000 osbot_aws-0.6.6/osbot_aws/apis/IAM.py
--rw-r--r--   0 dinis      (502) staff       (20)    11634 2019-05-18 13:23:26.000000 osbot_aws-0.6.6/osbot_aws/apis/Lambda.py
--rw-r--r--   0 dinis      (502) staff       (20)      642 2019-04-10 22:40:47.000000 osbot_aws-0.6.6/osbot_aws/apis/Lambdas.py
--rw-r--r--   0 dinis      (502) staff       (20)     4128 2019-04-13 15:25:36.000000 osbot_aws-0.6.6/osbot_aws/apis/Logs.py
--rw-r--r--   0 dinis      (502) staff       (20)     2094 2019-04-22 14:59:40.000000 osbot_aws-0.6.6/osbot_aws/apis/Parameter.py
--rw-r--r--   0 dinis      (502) staff       (20)     4615 2019-04-15 04:32:27.000000 osbot_aws-0.6.6/osbot_aws/apis/Queue.py
--rw-r--r--   0 dinis      (502) staff       (20)     8758 2019-04-15 04:43:15.000000 osbot_aws-0.6.6/osbot_aws/apis/S3.py
--rw-r--r--   0 dinis      (502) staff       (20)     2101 2019-04-13 11:04:39.000000 osbot_aws-0.6.6/osbot_aws/apis/Secrets.py
--rw-r--r--   0 dinis      (502) staff       (20)     1667 2019-04-15 04:06:41.000000 osbot_aws-0.6.6/osbot_aws/apis/Session.py
--rw-r--r--   0 dinis      (502) staff       (20)        0 2019-04-07 10:27:02.000000 osbot_aws-0.6.6/osbot_aws/apis/__init__.py
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws/apis/test_helpers/
--rw-r--r--   0 dinis      (502) staff       (20)      713 2019-04-22 15:03:22.000000 osbot_aws-0.6.6/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py
--rw-r--r--   0 dinis      (502) staff       (20)     2869 2019-04-13 11:57:32.000000 osbot_aws-0.6.6/osbot_aws/apis/test_helpers/Temp_Lambda.py
--rw-r--r--   0 dinis      (502) staff       (20)        0 2019-04-07 10:27:02.000000 osbot_aws-0.6.6/osbot_aws/apis/test_helpers/__init__.py
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws/helpers/
--rw-r--r--   0 dinis      (502) staff       (20)     2384 2019-04-10 22:38:50.000000 osbot_aws-0.6.6/osbot_aws/helpers/Aws_Cli.py
--rw-r--r--   0 dinis      (502) staff       (20)     1250 2019-04-07 10:26:45.000000 osbot_aws-0.6.6/osbot_aws/helpers/Aws_Utils.py
--rw-r--r--   0 dinis      (502) staff       (20)    10653 2019-04-12 03:42:19.000000 osbot_aws-0.6.6/osbot_aws/helpers/Create_Code_Build.py
--rw-r--r--   0 dinis      (502) staff       (20)      153 2019-04-07 18:05:40.000000 osbot_aws-0.6.6/osbot_aws/helpers/Fargate_Cluster.py
--rw-r--r--   0 dinis      (502) staff       (20)     1631 2019-04-13 14:04:41.000000 osbot_aws-0.6.6/osbot_aws/helpers/IAM_Policy.py
--rw-r--r--   0 dinis      (502) staff       (20)     1726 2019-04-08 13:22:03.000000 osbot_aws-0.6.6/osbot_aws/helpers/IAM_Role.py
--rw-r--r--   0 dinis      (502) staff       (20)     4295 2019-05-04 17:41:27.000000 osbot_aws-0.6.6/osbot_aws/helpers/Lambda_Package.py
--rw-r--r--   0 dinis      (502) staff       (20)        0 2019-04-07 10:26:51.000000 osbot_aws-0.6.6/osbot_aws/helpers/__init__.py
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws/lambdas/
--rw-r--r--   0 dinis      (502) staff       (20)        0 2019-03-31 16:08:36.000000 osbot_aws-0.6.6/osbot_aws/lambdas/__init__.py
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws/lambdas/dev/
--rw-r--r--   0 dinis      (502) staff       (20)        0 2019-03-31 16:08:36.000000 osbot_aws-0.6.6/osbot_aws/lambdas/dev/__init__.py
--rw-r--r--   0 dinis      (502) staff       (20)      118 2019-04-15 05:11:52.000000 osbot_aws-0.6.6/osbot_aws/lambdas/dev/check_aws_api.py
--rw-r--r--   0 dinis      (502) staff       (20)      147 2019-04-25 11:52:23.000000 osbot_aws-0.6.6/osbot_aws/lambdas/dev/check_python_utils.py
--rw-r--r--   0 dinis      (502) staff       (20)       91 2019-04-09 06:04:39.000000 osbot_aws-0.6.6/osbot_aws/lambdas/dev/hello_world.py
--rw-r--r--   0 dinis      (502) staff       (20)      326 2019-04-14 16:47:22.000000 osbot_aws-0.6.6/osbot_aws/lambdas/dev/write_cloud_watch_log.py
--rw-r--r--   0 dinis      (502) staff       (20)      210 2019-04-14 16:44:03.000000 osbot_aws-0.6.6/osbot_aws/lambdas/dev/write_queue.py
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws/lambdas/pocs/
--rw-r--r--   0 dinis      (502) staff       (20)        0 2019-03-31 16:08:36.000000 osbot_aws-0.6.6/osbot_aws/lambdas/pocs/__init__.py
--rw-r--r--   0 dinis      (502) staff       (20)      360 2019-04-14 18:09:10.000000 osbot_aws-0.6.6/osbot_aws/lambdas/pocs/confirm_process_stay_alive.py
--rw-r--r--   0 dinis      (502) staff       (20)      656 2019-04-14 17:11:13.000000 osbot_aws-0.6.6/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py
--rw-r--r--   0 dinis      (502) staff       (20)      215 2019-04-15 04:21:59.000000 osbot_aws-0.6.6/osbot_aws/lambdas/pocs/send_event_data_to_queue.py
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws/tmp_utils/
--rw-r--r--   0 dinis      (502) staff       (20)      336 2019-04-08 23:38:55.000000 osbot_aws-0.6.6/osbot_aws/tmp_utils/Temp_Assert.py
--rw-r--r--   0 dinis      (502) staff       (20)      181 2019-04-09 06:13:07.000000 osbot_aws-0.6.6/osbot_aws/tmp_utils/Temp_Files.py
--rw-r--r--   0 dinis      (502) staff       (20)     1006 2019-04-15 03:51:37.000000 osbot_aws-0.6.6/osbot_aws/tmp_utils/Temp_Misc.py
--rw-r--r--   0 dinis      (502) staff       (20)        0 2019-04-09 08:02:01.000000 osbot_aws-0.6.6/osbot_aws/tmp_utils/__init__.py
-drwxr-xr-x   0 dinis      (502) staff       (20)        0 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws.egg-info/
--rw-r--r--   0 dinis      (502) staff       (20)      509 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws.egg-info/PKG-INFO
--rw-r--r--   0 dinis      (502) staff       (20)     1636 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws.egg-info/SOURCES.txt
--rw-r--r--   0 dinis      (502) staff       (20)        1 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws.egg-info/dependency_links.txt
--rw-r--r--   0 dinis      (502) staff       (20)       10 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/osbot_aws.egg-info/top_level.txt
--rw-r--r--   0 dinis      (502) staff       (20)       38 2019-05-18 13:24:16.000000 osbot_aws-0.6.6/setup.cfg
--rw-r--r--   0 dinis      (502) staff       (20)      908 2019-05-18 13:23:50.000000 osbot_aws-0.6.6/setup.py
+-rw-r--r--   0        0        0    11357 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/LICENSE
+-rw-r--r--   0        0        0      623 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/README.md
+-rw-r--r--   0        0        0     4308 2024-05-23 23:32:44.127182 osbot_aws-2.5.0/osbot_aws/AWS_Config.py
+-rw-r--r--   0        0        0       92 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/Config.py
+-rw-r--r--   0        0        0     3424 2024-05-23 23:32:44.127567 osbot_aws-2.5.0/osbot_aws/Dependencies.py
+-rw-r--r--   0        0        0     2596 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/OSBot_Setup.py
+-rw-r--r--   0        0        0       16 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/__init__.py
+-rw-r--r--   0        0        0     1137 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/ACM.py
+-rw-r--r--   0        0        0    18486 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/API_Gateway.py
+-rw-r--r--   0        0        0     2400 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Athena.py
+-rw-r--r--   0        0        0      370 2024-02-25 00:25:50.759483 osbot_aws-2.5.0/osbot_aws/apis/Boto_Helpers.py
+-rw-r--r--   0        0        0     6902 2024-02-25 00:25:50.759781 osbot_aws-2.5.0/osbot_aws/apis/Cloud_Trail.py
+-rw-r--r--   0        0        0    14907 2024-04-14 17:42:52.634414 osbot_aws-2.5.0/osbot_aws/apis/Cloud_Watch.py
+-rw-r--r--   0        0        0     8632 2024-05-23 23:32:44.127991 osbot_aws-2.5.0/osbot_aws/apis/Cloud_Watch_Logs.py
+-rw-r--r--   0        0        0     3459 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/CodeBuild.py
+-rw-r--r--   0        0        0     6297 2024-05-23 23:32:44.128273 osbot_aws-2.5.0/osbot_aws/apis/Cognito_IDP.py
+-rw-r--r--   0        0        0    25047 2024-05-23 23:32:44.128631 osbot_aws-2.5.0/osbot_aws/apis/EC2.py
+-rw-r--r--   0        0        0     2904 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/ECR.py
+-rw-r--r--   0        0        0     5170 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Events.py
+-rw-r--r--   0        0        0     4033 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/Firehose.py
+-rw-r--r--   0        0        0      341 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Kinesis.py
+-rw-r--r--   0        0        0    22500 2024-05-23 23:32:44.128947 osbot_aws-2.5.0/osbot_aws/apis/Lambda.py
+-rw-r--r--   0        0        0      730 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Lambda_Docker.py
+-rw-r--r--   0        0        0    10392 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Lambda_Http.py
+-rw-r--r--   0        0        0     7751 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/apis/Lambda_Layer.py
+-rw-r--r--   0        0        0     8402 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/apis/Logs.py
+-rw-r--r--   0        0        0    16253 2024-05-23 23:32:44.129321 osbot_aws-2.5.0/osbot_aws/apis/S3.py
+-rw-r--r--   0        0        0     8568 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/SQS.py
+-rw-r--r--   0        0        0     1161 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/SSM.py
+-rw-r--r--   0        0        0     2785 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/Secrets.py
+-rw-r--r--   0        0        0     8807 2024-05-23 23:32:44.129489 osbot_aws-2.5.0/osbot_aws/apis/Session.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/__init__.py
+-rw-r--r--   0        0        0     2795 2024-05-23 23:32:44.129731 osbot_aws-2.5.0/osbot_aws/apis/shell/Lambda_Shell.py
+-rw-r--r--   0        0        0     3904 2024-05-23 23:32:44.129966 osbot_aws-2.5.0/osbot_aws/apis/shell/Shell_Client.py
+-rw-r--r--   0        0        0     2062 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/shell/Shell_Server.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/shell/__init__.py
+-rw-r--r--   0        0        0     1087 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py
+-rw-r--r--   0        0        0      623 2024-05-23 23:32:44.130208 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_EC2_Instance.py
+-rw-r--r--   0        0        0      559 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Event_Rule.py
+-rw-r--r--   0        0        0      984 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Event_Rule_To_SQS_Queue.py
+-rw-r--r--   0        0        0     1433 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Folder_With_Lambda_File.py
+-rw-r--r--   0        0        0      492 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_IAM_Role.py
+-rw-r--r--   0        0        0      404 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_IAM_User.py
+-rw-r--r--   0        0        0     3131 2024-04-14 17:42:52.634661 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Lambda.py
+-rw-r--r--   0        0        0     2956 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_S3_Zip_With_Lambda_File.py
+-rw-r--r--   0        0        0      868 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_SQS_Queue.py
+-rw-r--r--   0        0        0     2349 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_VPC.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-23 23:32:44.130429 osbot_aws-2.5.0/osbot_aws/aws/apigateway/API_Gateway_Management_API.py
+-rw-r--r--   0        0        0      919 2024-05-23 23:32:44.130698 osbot_aws-2.5.0/osbot_aws/aws/apigateway/API_Gateway_V2.py
+-rw-r--r--   0        0        0     1521 2024-05-23 23:32:44.130979 osbot_aws-2.5.0/osbot_aws/aws/apigateway/API_Gateway_V2__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.130999 osbot_aws-2.5.0/osbot_aws/aws/apigateway/__init__.py
+-rw-r--r--   0        0        0      945 2024-05-23 23:32:44.131326 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Connection.py
+-rw-r--r--   0        0        0     5209 2024-05-23 23:32:44.131561 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__DyDB.py
+-rw-r--r--   0        0        0     1219 2024-05-23 23:32:44.131784 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Events.py
+-rw-r--r--   0        0        0     1454 2024-05-23 23:32:44.131965 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Lambda.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.131990 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-23 23:32:44.132389 osbot_aws-2.5.0/osbot_aws/aws/apigateway/lambdas/Deploy__lambda_web_sockets.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.132409 osbot_aws-2.5.0/osbot_aws/aws/apigateway/lambdas/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-23 23:32:44.132623 osbot_aws-2.5.0/osbot_aws/aws/apigateway/lambdas/lambda_web_sockets.py
+-rw-r--r--   0        0        0     3698 2024-04-14 17:42:52.635198 osbot_aws-2.5.0/osbot_aws/aws/bedrock/Bedrock.py
+-rw-r--r--   0        0        0     2026 2024-04-14 17:42:52.635414 osbot_aws-2.5.0/osbot_aws/aws/bedrock/Bedrock__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-02-25 00:25:50.760793 osbot_aws-2.5.0/osbot_aws/aws/bedrock/__init__.py
+-rw-r--r--   0        0        0     4050 2024-05-23 23:32:44.132983 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/Bedrock__Cache.py
+-rw-r--r--   0        0        0      608 2024-04-14 17:42:52.636051 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/Sqlite__Bedrock__Row.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.636072 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/__init__.py
+-rw-r--r--   0        0        0     2547 2024-04-14 17:42:52.636500 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html.py
+-rw-r--r--   0        0        0     8447 2024-04-14 17:42:52.636787 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_Table.py
+-rw-r--r--   0        0        0     6263 2024-04-14 17:42:52.636970 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_With_Images.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.636991 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-25 00:25:50.760856 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/__init__.py
+-rw-r--r--   0        0        0      774 2024-04-14 17:42:52.637228 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2.py
+-rw-r--r--   0        0        0      181 2024-04-14 17:42:52.637392 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Mid.py
+-rw-r--r--   0        0        0      185 2024-04-14 17:42:52.637584 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Ultra.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.637604 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/ai21/__init__.py
+-rw-r--r--   0        0        0     1116 2024-04-14 17:42:52.637707 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Instant_V1.py
+-rw-r--r--   0        0        0     1020 2024-04-14 17:42:52.637966 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Messages_API.py
+-rw-r--r--   0        0        0      205 2024-04-14 17:42:52.638255 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_0.py
+-rw-r--r--   0        0        0      207 2024-04-14 17:42:52.638516 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_1.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.638563 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/__init__.py
+-rw-r--r--   0        0        0     1318 2024-04-14 17:42:52.638968 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/command/Cohere_Command.py
+-rw-r--r--   0        0        0      186 2024-04-14 17:42:52.639127 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Light_Text_V14.py
+-rw-r--r--   0        0        0      174 2024-04-14 17:42:52.639265 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Text_V14.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.639289 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/command/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-14 17:42:52.639630 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion.py
+-rw-r--r--   0        0        0      676 2024-04-14 17:42:52.639839 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V0.py
+-rw-r--r--   0        0        0     2293 2024-04-14 17:42:52.640125 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1.py
+-rw-r--r--   0        0        0     1396 2024-04-14 17:42:52.640417 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Image_To_Image.py
+-rw-r--r--   0        0        0      738 2024-04-14 17:42:52.640680 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Text_To_Image.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.640707 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-14 17:42:52.640935 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2.py
+-rw-r--r--   0        0        0      164 2024-04-14 17:42:52.641059 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_13b_chat_v1.py
+-rw-r--r--   0        0        0      164 2024-04-14 17:42:52.641277 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_70b_chat_v1.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.641301 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/llama2/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-14 17:42:52.641619 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI.py
+-rw-r--r--   0        0        0      175 2024-04-14 17:42:52.641785 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_7b_Instruct_v0_2.py
+-rw-r--r--   0        0        0      179 2024-04-14 17:42:52.641977 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_8x7b_Instruct_v0_1.py
+-rw-r--r--   0        0        0      173 2024-04-14 17:42:52.642180 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_Large_2402_v1_0.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.642201 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/__init__.py
+-rw-r--r--   0        0        0     3739 2024-04-14 17:42:52.642531 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Image_Generator_V1.py
+-rw-r--r--   0        0        0      348 2024-04-14 17:42:52.642642 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Express_V1.py
+-rw-r--r--   0        0        0      342 2024-04-14 17:42:52.642768 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Lite_V1.py
+-rw-r--r--   0        0        0      318 2024-04-14 17:42:52.642896 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Tg1_Large.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.642916 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/__init__.py
+-rw-r--r--   0        0        0     1011 2024-04-14 17:42:52.643133 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/base_classes/Amazon_Titan__Text.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.643153 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/base_classes/__init__.py
+-rw-r--r--   0        0        0     1712 2024-05-23 23:32:44.133281 osbot_aws-2.5.0/osbot_aws/aws/boto3/Cache_Boto3_Requests.py
+-rw-r--r--   0        0        0     2844 2024-04-14 17:42:52.643536 osbot_aws-2.5.0/osbot_aws/aws/boto3/Capture_Boto3_Error.py
+-rw-r--r--   0        0        0     5978 2024-02-25 00:25:50.762274 osbot_aws-2.5.0/osbot_aws/aws/boto3/View_Boto3_Rest_Calls.py
+-rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/boto3/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-23 23:32:44.133523 osbot_aws-2.5.0/osbot_aws/aws/cloud_front/Cloud_Front.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.133549 osbot_aws-2.5.0/osbot_aws/aws/cloud_front/__init__.py
+-rw-r--r--   0        0        0    13036 2024-05-23 23:32:44.133756 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB.py
+-rw-r--r--   0        0        0     1412 2024-02-25 00:25:50.762750 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Record.py
+-rw-r--r--   0        0        0      280 2024-05-23 23:32:44.134071 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Streams.py
+-rw-r--r--   0        0        0     6960 2024-05-23 23:32:44.134304 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Table.py
+-rw-r--r--   0        0        0     1294 2024-05-23 23:32:44.134643 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__with_temp_role.py
+-rw-r--r--   0        0        0     4040 2024-02-25 00:25:50.763161 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py
+-rw-r--r--   0        0        0        0 2024-02-25 00:25:50.763184 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/__init__.py
+-rw-r--r--   0        0        0     7015 2024-05-23 23:32:44.134885 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table.py
+-rw-r--r--   0        0        0     2217 2024-05-23 23:32:44.135057 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_GSI.py
+-rw-r--r--   0        0        0     4556 2024-05-23 23:32:44.135322 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_Timestamp.py
+-rw-r--r--   0        0        0     1084 2024-05-23 23:32:44.135598 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table__Resources.py
+-rw-r--r--   0        0        0     5693 2024-05-23 23:32:44.135789 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Timeseries.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.135813 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/__init__.py
+-rw-r--r--   0        0        0     7645 2024-05-23 23:32:44.136044 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/DyDB__Document.py
+-rw-r--r--   0        0        0     9656 2024-05-23 23:32:44.136231 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/DyDB__Query__Builder.py
+-rw-r--r--   0        0        0      313 2024-05-23 23:32:44.136412 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/DyDB__Resource.py
+-rw-r--r--   0        0        0      303 2024-05-23 23:32:44.136561 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/Resource__Config.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.136586 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/__init__.py
+-rw-r--r--   0        0        0    21575 2024-05-23 23:32:44.136922 osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS.py
+-rw-r--r--   0        0        0      733 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS_Actions.py
+-rw-r--r--   0        0        0      270 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS_Cluster.py
+-rw-r--r--   0        0        0     7074 2024-05-23 23:32:44.137182 osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS_Fargate_Task.py
+-rw-r--r--   0        0        0      631 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/ecs/Temp_ECS_Fargate_Task.py
+-rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/ecs/__init__.py
+-rw-r--r--   0        0        0     2398 2024-02-25 00:25:50.763337 osbot_aws-2.5.0/osbot_aws/aws/iam/Capture_IAM_Exception.py
+-rw-r--r--   0        0        0    21766 2024-05-23 23:32:44.137504 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM.py
+-rw-r--r--   0        0        0     9963 2024-05-23 23:32:44.137860 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Assume_Role.py
+-rw-r--r--   0        0        0     1831 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Policy.py
+-rw-r--r--   0        0        0     4700 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Role.py
+-rw-r--r--   0        0        0     1328 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Role_With_Policy.py
+-rw-r--r--   0        0        0     3041 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_User.py
+-rw-r--r--   0        0        0      964 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Utils.py
+-rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/__init__.py
+-rw-r--r--   0        0        0     2029 2024-05-23 23:32:44.137977 osbot_aws-2.5.0/osbot_aws/aws/lambda_/Lambda__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.137999 osbot_aws-2.5.0/osbot_aws/aws/lambda_/__init__.py
+-rw-r--r--   0        0        0     5975 2024-05-23 23:32:44.138252 osbot_aws-2.5.0/osbot_aws/aws/route_53/Route_53.py
+-rw-r--r--   0        0        0     2226 2024-05-23 23:32:44.138424 osbot_aws-2.5.0/osbot_aws/aws/route_53/Route_53__Hosted_Zone.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.138445 osbot_aws-2.5.0/osbot_aws/aws/route_53/__init__.py
+-rw-r--r--   0        0        0     1458 2024-05-23 23:32:44.138582 osbot_aws-2.5.0/osbot_aws/aws/s3/S3__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.138606 osbot_aws-2.5.0/osbot_aws/aws/s3/__init__.py
+-rw-r--r--   0        0        0     4849 2024-05-23 23:32:44.138710 osbot_aws-2.5.0/osbot_aws/aws/sts/STS.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:32:44.138729 osbot_aws-2.5.0/osbot_aws/aws/sts/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      808 2024-05-23 23:32:44.139074 osbot_aws-2.5.0/osbot_aws/decorators/aws_inject.py
+-rw-r--r--   0        0        0      942 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/decorators/aws_retry.py
+-rw-r--r--   0        0        0     2913 2024-05-23 23:32:44.139253 osbot_aws-2.5.0/osbot_aws/decorators/enforce_type_safety.py
+-rw-r--r--   0        0        0      686 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/decorators/lambda_save_event.py
+-rw-r--r--   0        0        0     4865 2024-05-23 23:32:44.139496 osbot_aws-2.5.0/osbot_aws/deploy/Deploy_Lambda.py
+-rw-r--r--   0        0        0     1367 2024-05-23 23:32:44.139753 osbot_aws-2.5.0/osbot_aws/deploy/TestCase__Lambda__Deploy.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/deploy/__init__.py
+-rw-r--r--   0        0        0      948 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/exceptions/Session_Bad_Credentials.py
+-rw-r--r--   0        0        0      330 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/exceptions/Session_Client_Creation_Fail.py
+-rw-r--r--   0        0        0      610 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/exceptions/Session_No_Credentials.py
+-rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/exceptions/__init__.py
+-rw-r--r--   0        0        0      959 2024-05-23 23:32:44.139975 osbot_aws-2.5.0/osbot_aws/helpers/AMI.py
+-rw-r--r--   0        0        0     2595 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/Aws_Cli.py
+-rw-r--r--   0        0        0    11778 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Create_Code_Build.py
+-rw-r--r--   0        0        0     2920 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Create_Image_ECR.py
+-rw-r--r--   0        0        0     2038 2024-05-23 23:32:44.140289 osbot_aws-2.5.0/osbot_aws/helpers/EC_Instance.py
+-rw-r--r--   0        0        0     2544 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/Event_Rule.py
+-rw-r--r--   0        0        0       61 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_From_S3.py
+-rw-r--r--   0        0        0     1771 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Helpers.py
+-rw-r--r--   0        0        0     6311 2024-05-23 23:32:44.140523 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Layer_Create.py
+-rw-r--r--   0        0        0      494 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Layers_Local.py
+-rw-r--r--   0        0        0     2845 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Layers_OSBot.py
+-rw-r--r--   0        0        0     8284 2024-05-23 23:32:44.140788 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Package.py
+-rw-r--r--   0        0        0     2001 2024-05-23 23:32:44.141011 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_SSH.py
+-rw-r--r--   0        0        0     1247 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_SSH_Kubectl.py
+-rw-r--r--   0        0        0     1338 2024-05-23 23:32:44.141238 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Upload_Package.py
+-rw-r--r--   0        0        0     2154 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/Parameter.py
+-rw-r--r--   0        0        0     4127 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Rest_API.py
+-rw-r--r--   0        0        0     1497 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/S3_Zip_From_Files.py
+-rw-r--r--   0        0        0     5565 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/SQS_Queue.py
+-rw-r--r--   0        0        0     1562 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Test_Helper.py
+-rw-r--r--   0        0        0     2181 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/VPC.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/__init__.py
+-rw-r--r--   0        0        0      127 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/check_aws_api.py
+-rw-r--r--   0        0        0      139 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/check_python_utils.py
+-rw-r--r--   0        0        0       87 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/hello_world.py
+-rw-r--r--   0        0        0      137 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/lambda_layer.py
+-rw-r--r--   0        0        0      326 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/write_cloud_watch_log.py
+-rw-r--r--   0        0        0      221 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/write_queue.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/pocs/__init__.py
+-rw-r--r--   0        0        0      353 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/pocs/confirm_process_stay_alive.py
+-rw-r--r--   0        0        0      648 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py
+-rw-r--r--   0        0        0      230 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/lambdas/pocs/send_event_data_to_queue.py
+-rw-r--r--   0        0        0     1916 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/server_ssh.py
+-rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/shell/__init__.py
+-rw-r--r--   0        0        0      138 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/shell/lambda_shell.py
+-rw-r--r--   0        0        0      129 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/shell/shell_server.py
+-rw-r--r--   0        0        0      575 2024-05-23 23:32:44.141344 osbot_aws-2.5.0/osbot_aws/testing/TestCase__API_Gateway_V2.py
+-rw-r--r--   0        0        0      973 2024-05-23 23:32:44.141654 osbot_aws-2.5.0/osbot_aws/testing/TestCase__Bedrock.py
+-rw-r--r--   0        0        0      431 2024-05-23 23:32:44.141813 osbot_aws-2.5.0/osbot_aws/testing/TestCase__Boto3_Cache.py
+-rw-r--r--   0        0        0      525 2024-05-23 23:32:44.142025 osbot_aws-2.5.0/osbot_aws/testing/TestCase__Dynamo_DB.py
+-rw-r--r--   0        0        0     1707 2024-05-23 23:32:44.142128 osbot_aws-2.5.0/osbot_aws/testing/TestCase__Lambda.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:42:52.645306 osbot_aws-2.5.0/osbot_aws/testing/__init__.py
+-rw-r--r--   0        0        0       91 2024-05-23 23:32:44.142381 osbot_aws-2.5.0/osbot_aws/utils/Execution_Env.py
+-rw-r--r--   0        0        0      458 2024-05-23 23:32:44.142603 osbot_aws-2.5.0/osbot_aws/utils/Version.py
+-rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/utils/__init__.py
+-rw-r--r--   0        0        0        7 2024-05-23 23:35:39.958222 osbot_aws-2.5.0/osbot_aws/version
+-rw-r--r--   0        0        0      677 2024-05-23 23:32:44.143272 osbot_aws-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 osbot_aws-2.5.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `osbot_aws-0.6.6/osbot_aws/apis/Athena.py` & `osbot_aws-2.5.0/osbot_aws/apis/Athena.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-0.6.6/osbot_aws/apis/CodeBuild.py` & `osbot_aws-2.5.0/osbot_aws/apis/CodeBuild.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import  boto3
 from    time                                import sleep
-
-from    osbot_aws.apis.IAM                  import IAM
-from    pbx_gs_python_utils.utils.Dev       import Dev
-from    pbx_gs_python_utils.utils.Misc      import Misc
-
 from osbot_aws.apis.Session import Session
+from osbot_aws.aws.iam.IAM import IAM
+from osbot_utils.utils import Misc
+from osbot_utils.utils.Dev import Dev
 
 
 class CodeBuild:
 
     def __init__(self, project_name, role_name):
         self.codebuild    = Session().client('codebuild')
         self.iam          = IAM(role_name=role_name)
@@ -44,23 +42,16 @@
                 Dev.pprint("[{0}] {1} {2}".format(i,build_status,current_phase))
             if build_status != 'IN_PROGRESS':
                 return build_info
             sleep(sleep_for)
         return None
 
 
-    def policies_create(self, policies):                        # does not update, only add new ones
-        policies_arns = []
-        role_policies = list(self.iam.role_policies().keys())
-        for base_name, policy in policies.items():
-            policy_name = "{0}_{1}".format(base_name, self.project_name)
-            if policy_name in role_policies:
-                continue
-            policies_arns.append(self.iam.policy_create(policy_name,policy).get('policy_arn'))
-        return policies_arns
+    def policies_create(self, policies):
+        return self.iam.policies_create(policies, self.project_name)
 
     def project_builds(self,ids):
         return self.codebuild.batch_get_builds(ids=ids)
 
     def project_create(self, project_repo, service_role):
 
         kvargs = {
```

### Comparing `osbot_aws-0.6.6/osbot_aws/apis/Dynamo.py` & `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,20 @@
-import boto3
-from   boto3    import resource
-from pbx_gs_python_utils.utils.Misc import Misc
-
-from osbot_aws.apis.Session import Session
-
-
-class Dynamo:
-    def __init__(self):
-        self.resource   = resource('dynamodb')
-        self._dynamo    = None
-        self._streams   = None
-
-    # helpers
-
-    def dynamo(self):
-        if self._dynamo is None:
-            self._dynamo = Session().client('dynamodb')
-        return self._dynamo
-
-    def dynamo_streams(self):
-        if self._streams is None:
-            self._streams = Session().client('dynamodbstreams')
-        return self._streams
-    # main methods
-
-    def create(self, table_name, key, with_streams=False):
-        keySchema             = [ {'AttributeName'    : key        , 'KeyType'           : 'HASH' } ]
-        attributeDefinitions  = [ {'AttributeName'    : key        , 'AttributeType'     : 'S'    } ]
-        provisionedThroughput = { 'ReadCapacityUnits' : 5          , 'WriteCapacityUnits': 5      }
-        kwargs   = { 'TableName'            : table_name           ,
-                     'KeySchema'            : keySchema            ,
-                     'AttributeDefinitions' : attributeDefinitions ,
-                     'ProvisionedThroughput': provisionedThroughput }
-        if with_streams:
-            kwargs['StreamSpecification'] = {'StreamEnabled': True, 'StreamViewType': 'NEW_IMAGE' }
-        self.dynamo().create_table( **kwargs)
-
-        self.dynamo().get_waiter('table_exists') \
-            .wait(TableName=table_name, WaiterConfig={'Delay': 5, 'MaxAttempts': 10})
-        return self
-
-    def delete(self, table_name):
-        self.dynamo().delete_table(TableName = table_name)
-        self.dynamo().get_waiter('table_not_exists')      \
-                   .wait(TableName=table_name, WaiterConfig={'Delay': 10, 'MaxAttempts':10 })
-        return self
+from boto3 import resource
 
-    def list(self):
-        return self.dynamo().list_tables()['TableNames']
+from osbot_aws.aws.dynamo_db.Dynamo_DB import Dynamo_DB
+from osbot_utils.utils.Lists import array_pop
+from osbot_utils.utils.Objects import get_value
 
-    def streams(self):
-        return self.dynamo_streams().list_streams().get('Streams')
-
-class Dynamo_Table:
+# todo: see if we can remove this class once the new Dynamo_DB__Table is implemented
+class Dynamo_Table__Resource:
     def __init__(self,table_name, key):
         self.table_name = table_name
         self.key        = key
-        self.dynamo     = Dynamo()
-        self.resource   = self.dynamo.resource
+        self.dynamo     = Dynamo_DB()
+        self.resource   = resource('dynamodb')          # this has quite a lot of weird performance implications
         self.table      = self.resource.Table(self.table_name)
         self.chuck_size = 100
 
         self._keys      = None
 
     def add(self,row):
         self.table.put_item(Item=row)
@@ -99,15 +52,15 @@
             for key in chunck:
                 request_items.append({self.key:  key })
             response = self.resource.batch_get_item(RequestItems={self.table_name: {'Keys': request_items}})
             yield response['Responses'][self.table_name]
 
     def info(self):
         try:
-            return self.dynamo.dynamo().describe_table(TableName = self.table_name)
+            return self.dynamo.client().describe_table(TableName = self.table_name)
         except:
             return None
 
     def keys(self, use_cache=True):
         if self._keys and use_cache:
             return self._keys
         def get_scan_batch (start_key):
@@ -130,26 +83,26 @@
             map_Items(response['Items'])                                # map items
 
         self._keys = keys
 
         return keys
 
     def stream_arn(self):
-        streams   = self.dynamo.dynamo_streams().list_streams(TableName=self.table_name).get('Streams')
-        first_one = Misc.array_pop(streams,0)
-        return Misc.get_value(first_one,'StreamArn')
+        streams   = self.dynamo.client__dynamo_streams().list_streams(TableName=self.table_name).get('Streams')
+        first_one = array_pop(streams,0)
+        return get_value(first_one,'StreamArn')
 
     def stream_info(self):
         stream_arn = self.stream_arn()
         if stream_arn:
-            return self.dynamo.dynamo_streams().describe_stream(StreamArn=stream_arn).get('StreamDescription')
+            return self.dynamo.client__dynamo_streams().describe_stream(StreamArn=stream_arn).get('StreamDescription')
 
     def stream_get_data_latest(self):
         stream_info    = self.stream_info()
         shard_id       = stream_info.get('Shards').pop(0).get('ShardId')
-        shard_iterator = self.dynamo.dynamo_streams().get_shard_iterator(StreamArn=self.stream_arn(), ShardId=shard_id, ShardIteratorType='LATEST').get('ShardIterator')
-        return           self.dynamo.dynamo_streams().get_records(ShardIterator=shard_iterator)
+        shard_iterator = self.dynamo.client__dynamo_streams().get_shard_iterator(StreamArn=self.stream_arn(), ShardId=shard_id, ShardIteratorType='LATEST').get('ShardIterator')
+        return           self.dynamo.client__dynamo_streams().get_records(ShardIterator=shard_iterator)
 
         #shard_iterator = get_shard_iterator
 
     def status(self):
         return self.info()['Table']['TableStatus']
```

### Comparing `osbot_aws-0.6.6/osbot_aws/apis/Ec2.py` & `osbot_aws-2.5.0/osbot_aws/helpers/EC_Instance.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,59 @@
-import boto3
+from osbot_aws.apis.EC2 import EC2
+from osbot_utils.base_classes.Kwargs_To_Self import Kwargs_To_Self
+from osbot_utils.helpers.SSH import SSH
+from osbot_utils.utils.Dev import pprint
+from osbot_utils.utils.Misc import random_string
 
-from osbot_aws.apis.Session import Session
+from osbot_aws.helpers.AMI import AMI
 
 
-class Ec2:
-    def __init__(self):
-        self.ec2          = Session().client('ec2')
-        self.ec2_resource = boto3.resource('ec2')
+class EC2_Instance(Kwargs_To_Self):
+    instance_id   : str
+    create_kwargs : dict
+    ec2           : EC2
+    # def __init__(self, instance_id=None, create_kwargs=None):
+    #     self.create_kwargs = create_kwargs
+    #     self.instance_id   = instance_id
+    #     self.ec2           = EC2()
 
+    def create(self):
+        kwargs = self.create_kwargs
+        random_name = random_string(prefix='test_ec2_with_ssh_support')
+        if not kwargs.get('image_id'     ): kwargs['image_id'     ] = AMI().amazon_linux_2()
+        if not kwargs.get('instance_type'): kwargs['instance_type'] = 't2.nano'
+        if not kwargs.get('name'         ): kwargs['name'         ] = random_name
+        if not kwargs.get('tags'         ): kwargs['tags'         ] = {'Type': 'EC2_Instance'}
 
+        self.instance_id = self.ec2.instance_create(**kwargs)
+        return self.instance_id
 
-    def instances_details(self):
-        instances = {}
-        for instance in self.ec2_resource.instances.all():
-            instance_id = instance.instance_id
-            instances[instance_id] = { 'cpus'         : instance.cpu_options['CoreCount']     ,
-                                       'image_id'     : instance.image_id                     ,
-                                       'instance_type': instance.instance_type                ,
-                                       'public_ip'    : instance.public_ip_address            ,
-                                       'state'        : instance.state                        ,
-                                       'tags'         : instance.tags                         }
-
-        return instances
-
-    def security_groups(self):
-        groups={}
-        for group in self.ec2.describe_security_groups().get('SecurityGroups'):
-            groups[group.get('GroupId')] = group
-        return groups
-
-    def subnets(self):
-        subnets = {}
-        for subnet in self.ec2.describe_subnets().get('Subnets'):
-            subnets[subnet.get('SubnetId')] = subnet
-        return subnets
-
-    def vpcs(self):
-        vpcs = {}
-        for vpc in self.ec2.describe_vpcs().get('Vpcs'):
-            vpcs[vpc.get('VpcId')] = vpc
-        return vpcs
+    def delete(self):
+        return self.ec2.instance_delete(instance_id=self.instance_id)
+
+    def exists(self):
+        return self.ec2.instance_exists(instance_id=self.instance_id)
+
+    def info(self):
+        return self.ec2.instance_details(instance_id=self.instance_id)
+
+    def print_info(self):
+        pprint(self.info())
+
+    def ip_address(self):
+        return self.info().get('public_ip')
+
+    def start(self):
+        return self.ec2.instance_start(instance_id=self.instance_id)
+
+    def stop(self):
+        return self.ec2.instance_terminate(instance_id=self.instance_id)
+
+    def ssh(self, ssh_key_file, ssh_key_user):
+        ip_address = self.ip_address()
+        return SSH(ssh_host=ip_address, ssh_key_file=ssh_key_file, ssh_key_user=ssh_key_user)
+
+    def state(self):
+        return self.info().get('state')
+
+    def tags(self):
+        return self.info().get('tags')
```

### Comparing `osbot_aws-0.6.6/osbot_aws/apis/Parameter.py` & `osbot_aws-2.5.0/osbot_aws/helpers/Parameter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
-from pbx_gs_python_utils.utils.Misc import Misc
+from osbot_utils.utils import Misc
 
 from osbot_aws.apis.Session import Session
 
 
-class Parameter:
+class Parameter:                                # todo refactor main methods to SSM class
     def __init__(self, name=None):
         self._ssm = None
         self.name = name
 
     # helpers
     def ssm(self):
         if self._ssm is None:
```

### Comparing `osbot_aws-0.6.6/osbot_aws/apis/Queue.py` & `osbot_aws-2.5.0/osbot_aws/helpers/SQS_Queue.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,139 +1,133 @@
 import json
 
-from pbx_gs_python_utils.utils.Misc import Misc
+from osbot_utils.decorators.methods.cache_on_self import cache_on_self
+from osbot_utils.utils.Misc import random_string
 
-from osbot_aws.apis.Session import Session
+from osbot_utils.utils.Json import json_dumps, json_loads
+from osbot_aws.apis.SQS import SQS
 
+class SQS_Queue:                                        # todo refactor main methods to SSM class
+    def __init__(self, queue_name=None, queue_url=None, fifo_message_group_id=False):
+        self.queue_name            = queue_name
+        self.queue_url             = queue_url
+        self.fifo_message_group_id = fifo_message_group_id or random_string(prefix="message_group_id-")
 
-class Queue:
-    def __init__(self, queue_name=None, url=None):
-        self._url       = url
-        self._sqs       = None
-        self.queue_name = queue_name
-
-    # helper methods
+    @cache_on_self
     def sqs(self):
-        if self._sqs is None:
-            self._sqs = Session().client('sqs')
-        return self._sqs
-
-    def url(self):
-        if self._url is None:
-            self._url =  self.sqs().get_queue_url(QueueName=self.queue_name).get('QueueUrl')
-        return self._url
-
+        return SQS()
 
     # main methods
 
-    def add(self, body, attributes=None):
-        self.message_send(body,attributes)
+    def add(self, body, message_group_id=None, attributes_data=None):
+        self.message_send(body=body, message_group_id=message_group_id, attributes_data=attributes_data)
+        return self
+
+    def add_fifo(self, body, fifo_message_group_id=None, attributes_data=None):
+        self.message_send_fifo(body=body, fifo_message_group_id=fifo_message_group_id, attributes_data=attributes_data)
         return self
 
     def arn(self):
         return self.attributes().get('QueueArn')
 
-    def attributes(self):
-        try:
-            return self.sqs().get_queue_attributes(QueueUrl=self.url(),AttributeNames=['All']).get('Attributes')
-        except:
-            return None
+    def attributes(self, attribute_names='All'):
+        return self.sqs().queue_attributes(queue_url=self.url(),attribute_names=attribute_names)
 
     def attributes_update(self, new_attributes):
-        return self.sqs().set_queue_attributes(QueueUrl=self.url(), Attributes=new_attributes)
+        return self.sqs().queue_attributes_update(queue_url=self.url(), new_attributes=new_attributes)
 
+    def create(self, attributes=None):
+        return self.sqs().queue_create(queue_name=self.queue_name, attributes=attributes)
 
-    def create_raw(self,attributes=None):
-        if attributes is None: attributes = {}
-        return self.sqs().create_queue(QueueName=self.queue_name,Attributes=attributes).get('QueueUrl')
-
-    def create(self,attributes=None):
-        queue_url = self.create_raw(attributes)
-        if queue_url:
-            return self
-        return None
+    def create_fifo(self, attributes=None):
+        return self.sqs().queue_create_fifo(queue_name=self.queue_name, attributes=attributes)
 
     def delete(self):
-        if self.exists() is False: return False
-        self.sqs().delete_queue(QueueUrl=self.url())
-        return self.exists() is False
+        return self.sqs().queue_delete(queue_url=self.url())
 
     def exists(self):
-        return self.attributes() is not None
+        return self.sqs().queue_exists(queue_url=self.url())
 
     def get_message(self, delete_message=True):
-        message = self.message_raw()
-        if message:
-            body = message.get('Body')
-            receipt_handle = message.get('ReceiptHandle')
-            if delete_message:
-                self.message_delete(receipt_handle)
-            return body
+        return self.sqs().queue_message_get(queue_url=self.url(), delete_message=delete_message)
 
     def get_message_with_attributes(self, delete_message=True):
-        message = self.message_raw()
-        if message:
-            body            = message.get('Body')
-            attributes      = message.get('MessageAttributes')
-            receipt_handle  = message.get('ReceiptHandle')
-            attributes_data = {}
-            if attributes:
-                for key,value in attributes.items():
-                    attributes_data[key] = value.get('StringValue')
-            if delete_message:
-                self.message_delete(receipt_handle)
-            return body, attributes_data
-
-    def get_n_message(self, n, delete_message=True):
-        messages = []
-        for i in range(0,n):
-            message = self.get_message(delete_message)
-            if message:
-                messages.append(message)
-            else:
-                break
-        return messages
+        return self.sqs().queue_message_get_with_attributes(queue_url=self.url(), delete_message=delete_message)
 
-    def list(self):
-        return self.sqs().list_queues().get('QueueUrls')
+    def get_many(self, count=1, delete_message=True):
+        return self.sqs().queue_messages_get_n(queue_url=self.url(), n=count, delete_message=delete_message)
 
+    def info(self):                         # consistent method with similar classes like Lambda
+        return self.sqs().queue_info(queue_url=self.url())
+
+    def fifo(self):
+        return self.info().get('FifoQueue') == 'true'
 
     def message_raw(self):
-        messages = self.sqs().receive_message(QueueUrl=self.url(), MessageAttributeNames=['All']).get('Messages')
-        return Misc.array_pop(messages,0)
+        return self.sqs().queue_message_get_raw(queue_url=self.url())
 
     def message_delete(self, receipt_handle):
-        return self.sqs().delete_message(QueueUrl=self.url(), ReceiptHandle=receipt_handle)
-
+        return self.sqs().queue_message_delete(queue_url=self.url(), receipt_handle=receipt_handle)
 
-    #def add(self, message, attributes=None): return self.message_send(message,attributes)
+    def message_send(self, body, message_group_id=None, attributes_data=None):
+        return self.sqs().queue_message_send(queue_url=self.url(), body=body, message_group_id=message_group_id, attributes_data=attributes_data)
 
-    def message_send(self,body,attributes_data=None):
-        if attributes_data is None:
-            return self.sqs().send_message(QueueUrl=self.url(), MessageBody=body).get('MessageId')
-        else:
-            attributes = {}
-            for key,value in attributes_data.items():
-                attributes[key] = { 'StringValue': value , 'DataType': 'String'}
-            return self.sqs().send_message(QueueUrl=self.url(),MessageBody=body, MessageAttributes=attributes).get('MessageId')
+    def message_send_fifo(self,body, fifo_message_group_id=None, attributes_data=None):
+        message_group_id = fifo_message_group_id or self.fifo_message_group_id  # allow this value to be overwritten per request
+        return self.message_send(body=body, message_group_id= message_group_id, attributes_data=attributes_data)
 
     def messages_in_queue(self):
-        return int(self.attributes().get('ApproximateNumberOfMessages'))
+        return self.sqs().queue_messages_count(queue_url=self.url())
 
     def messages_not_visible(self):
-        return int(self.attributes().get('ApproximateNumberOfMessagesNotVisible'))
+        return self.sqs().queue_messages_count_not_visible(queue_url=self.url())
+
+    def name(self):
+        return self.queue_name
 
-    def push(self, data):
+    def permission_add(self, label, aws_account_ids, actions):
+        return self.sqs().permission_add(queue_url=self.url(), label=label, aws_account_ids=aws_account_ids, actions=actions)
+
+    def permission_add_for_service(self, source_arn, service, resource):
+        return self.sqs().permission_add_for_service(queue_url=self.url(), service=service, source_arn=source_arn, resource=resource)
+
+    def permission_delete(self, label):
+        return self.sqs().permission_delete(queue_url=self.url(), label=label)
+
+    def permissions(self):
+        return self.sqs().permissions(queue_url=self.url())
+
+    def policy(self):
+        return self.sqs().policy(queue_url=self.url())
+
+    def push(self, data, message_group_id=None, attributes_data=None):
         if data:
-            self.message_send(json.dumps(data))
+            if type(data) is not str:
+                body = json_dumps(data)
+            else:
+                body = data
+            self.message_send(body=body, message_group_id=message_group_id, attributes_data=attributes_data)
         return self
 
-    def pull(self, delete_message=True):
+    def push_fifo(self, data, fifo_message_group_id=None, attributes_data=None):
+        if data:
+            if type(data) is not str:
+                body = json_dumps(data)
+            else:
+                body = data
+            self.message_send_fifo(body=body, fifo_message_group_id=fifo_message_group_id,attributes_data=attributes_data)
+        return self
+
+    def pop(self, delete_message=True):
         data_json = self.get_message(delete_message=delete_message)
         if data_json:
-            return json.loads(data_json)
+            return json_loads(data_json)
         return None
 
-    def set_queue_name(self, queue_name):
-        self.queue_name = queue_name
-        self._url       = None          # need to reset this value or the old value will still be used
-        return self
+    def url(self):
+        if self.queue_url  is None:
+            self.queue_url = self.sqs().queue_url(queue_name=self.queue_name)
+        return self.queue_url
+
+SQS_Queue.next = SQS_Queue.pop
+SQS_Queue.pull = SQS_Queue.pop
+SQS_Queue.size = SQS_Queue.messages_in_queue
```

### Comparing `osbot_aws-0.6.6/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py` & `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,27 @@
-from osbot_aws.apis.IAM         import IAM
-from osbot_aws.helpers.IAM_Role import IAM_Role
+from osbot_aws.AWS_Config import AWS_Config
+from osbot_aws.aws.iam.IAM_Role import IAM_Role
+
 
 class Temp_Aws_Roles:
     def __init__(self):
         self.temp_prefix                      = 'temp_role_'
-        self.role_name__for_lambda_invocation = self.temp_prefix + 'for_lambda_invocation'
+        self.role_name__for_lambda_invocation = self.temp_prefix + 'for_lambda_invocation' # todo: improve this logic
         pass
 
-    def create__for_lambda_invocation(self, delete_existing=False):
+    def for_lambda_invocation__create(self, delete_existing=False):
         iam_role = IAM_Role(self.role_name__for_lambda_invocation)
         if delete_existing:
             iam_role.iam.role_delete()
         return iam_role.create_for__lambda().get('role_arn')
 
-    def for_lambda_invocation(self):
-        return 'arn:aws:iam::{0}:role/{1}'.format(IAM().account_id(),self.role_name__for_lambda_invocation)
+    def for_lambda_invocation__not_exists(self):
+        return self.for_lambda_invocation_exists() is False
+
+    def for_lambda_invocation_exists(self):
+        iam_role = IAM_Role(self.role_name__for_lambda_invocation)
+        return iam_role.iam.role_exists()
+
+    def for_lambda_invocation__role_arn(self):
+        account_id = AWS_Config().aws_session_account_id()
+        role_name  = self.role_name__for_lambda_invocation
+        return f"arn:aws:iam::{account_id}:role/{role_name}"
```

### Comparing `osbot_aws-0.6.6/osbot_aws/helpers/Create_Code_Build.py` & `osbot_aws-2.5.0/osbot_aws/helpers/Create_Code_Build.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,89 @@
-from time import sleep
-
 from osbot_aws.apis.CodeBuild import CodeBuild
+from osbot_aws.aws.iam.IAM import IAM
+
 
 #todo: add Create_Code_Build tests from gs-docker-codebuild project
 class Create_Code_Build:
 
-    def __init__(self,account_id,project_name):
-        self.account_id         = account_id
+    def __init__(self, project_name, github_org='owasp-sbot', source_version='master', build_spec='buildspec.yml', docker_type='LINUX_CONTAINER',docker_image='aws/codebuild/docker:18.09.0',compute_type='BUILD_GENERAL1_SMALL'):
+        self.iam                = IAM()
+        self.build_spec         = build_spec
+        self.github_org         = github_org
+        self.source_version     = source_version
+        self.docker_type        = docker_type
+        self.docker_image       = docker_image
+        self.compute_type       = compute_type
         self.project_name       = project_name
-        self.project_repo       = 'https://github.com/pbx-gs/{0}'.format(self.project_name)
-        self.service_role       = 'arn:aws:iam::{0}:role/{1}'                  .format(self.account_id, self.project_name)
-        self.project_arn        = 'arn:aws:codebuild:eu-west-2:{0}:project/{1}'.format(self.account_id, self.project_name     )
+        self.account_id         = self.iam.account_id()
+        self.region             = self.iam.region()
+        self.project_repo       = f'https://github.com/{self.github_org}/{self.project_name}'
+        self.service_role       = f'arn:aws:iam::{self.account_id}:role/{self.project_name}'
+        self.project_arn        = f'arn:aws:codebuild:{self.region}:{self.account_id}:project/{self.project_name}'
         self.assume_policy      = {'Statement': [{'Action'   : 'sts:AssumeRole'                     ,
                                                   'Effect'   : 'Allow'                              ,
                                                   'Principal': {'Service': 'codebuild.amazonaws.com'}}]}
 
         self.code_build = CodeBuild(role_name=self.project_name, project_name=self.project_name)
 
     def create_role_and_policies(self, policies):
         self.code_build.iam.role_create(self.assume_policy)
         policies_arn = self.code_build.policies_create(policies)
         self.code_build.iam.role_policies_attach(policies_arn)
         return self
 
     def create_project_with_container__docker(self):
         kvargs = {
-            'name'        : self.project_name,
-            'source'      : { 'type'         : 'GITHUB',
-                              'location'     : self.project_repo                 },
-            'artifacts'   : {'type'          : 'NO_ARTIFACTS'                    },
-            'environment' : {'type'          : 'LINUX_CONTAINER'                  ,
-                            'image'          : 'aws/codebuild/docker:18.09.0'     ,
-                            'computeType'    : 'BUILD_GENERAL1_LARGE'            },
-            'serviceRole' : self.service_role
+            'name'         : self.project_name,
+            'source'       : { 'type'         : 'GITHUB',
+                               'location'     : self.project_repo                  ,
+                               'buildspec'    : self.build_spec                   },
+            'sourceVersion': self.source_version                                   ,
+            'artifacts'    : {'type'          : 'NO_ARTIFACTS'                    },
+            'environment'  : {'type'          : self.docker_type                   ,
+                              'image'         : self.docker_image                  ,
+                              'computeType'   : self.compute_type                  },
+            'serviceRole'  : self.service_role
         }
 
         return self.code_build.codebuild.create_project(**kvargs)
 
     def create_project_with_container__gs_docker_codebuild(self):
         kvargs = {
-            'name'        : self.project_name,
-            'source'      : { 'type'                   : 'GITHUB',
-                           'location'                  : self.project_repo                 },
-            'artifacts'   : {'type'                    : 'NO_ARTIFACTS'                    },
-            'environment' : {'type'                    : 'LINUX_CONTAINER'                  ,
-                            'image'                    : '{0}.dkr.ecr.eu-west-2.amazonaws.com/gs-docker-codebuild:latest'.format(self.account_id)     ,
-                            'computeType'              : 'BUILD_GENERAL1_LARGE'            ,
-                            'imagePullCredentialsType' : 'SERVICE_ROLE'                    },
-            'serviceRole' : self.service_role
+            'name'         : self.project_name,
+            'source'       : { 'type'                   : 'GITHUB',
+                               'location'               : self.project_repo                  ,
+                               'buildspec'              : self.build_spec                   },
+            'sourceVersion': self.source_version                                             ,
+            'artifacts'    : {'type'                    : 'NO_ARTIFACTS'                    },
+            'environment'  : {'type'                    : self.docker_type                   ,
+                             'image'                    : f'{self.account_id}.dkr.ecr.{self.region}.amazonaws.com/{self.project_name}:latest'.lower(),
+                             'computeType'              : self.compute_type                  ,
+                             'imagePullCredentialsType' : 'SERVICE_ROLE'                    },
+            'serviceRole'  : self.service_role
         }
         return self.code_build.codebuild.create_project(**kvargs)
 
     def policies__for_docker_build(self):
-        cloud_watch_arn = "arn:aws:logs:eu-west-2:{0}:log-group:/aws/codebuild/{1}:log-stream:*".format(self.account_id, self.project_name)
+        cloud_watch_arn = f"arn:aws:logs:{self.region}:{self.account_id}:log-group:/aws/codebuild/{self.project_name}:log-stream:*"
         policies = {"Cloud-Watch-Policy": {"Version": "2012-10-17",
                                            "Statement": [{"Sid": "GsBotPolicy",
                                                           "Effect": "Allow",
                                                           "Action": ["logs:CreateLogGroup",
                                                                      "logs:CreateLogStream",
                                                                      "logs:PutLogEvents"],
-                                                          "Resource": [cloud_watch_arn]}]},
+                                                          "Resource": [ cloud_watch_arn ]}]},
                     "Secret-Manager": {
                         "Version": "2012-10-17",
                         "Statement": [{"Sid": "GsBotPolicy",
                                        "Effect": "Allow",
                                        "Action": ["secretsmanager:GetSecretValue", "secretsmanager:DescribeSecret"],
                                        "Resource": [
-                                           "arn:aws:secretsmanager:eu-west-2:244560807427:secret:slack-gs-bot-*",
-                                           "arn:aws:secretsmanager:eu-west-2:244560807427:secret:elastic_gsuite_data-*"]}]},
+                                           f"arn:aws:secretsmanager:{self.region}:{self.account_id}:secret:slack-gs-bot-*",
+                                           f"arn:aws:secretsmanager:{self.region}:{self.account_id}:secret:gw-elastic-server-*"]}]},  # todo: refactor
                     "Create-Docker-Image": {
                         "Version": "2012-10-17",
                         "Statement": [{"Effect": "Allow",
                                        "Action": ["ecr:BatchCheckLayerAvailability",
                                                   "ecr:CompleteLayerUpload",
                                                   "ecr:GetAuthorizationToken",
                                                   "ecr:InitiateLayerUpload",
@@ -82,15 +94,15 @@
                         "Version": "2012-10-17",
                         "Statement": [{"Effect": "Allow",
                                        "Action": ["ecr:CreateRepository"],
                                        "Resource": "*"}]}}
         return policies
 
     def policies__with_ecr(self):
-        cloud_watch_arn = "arn:aws:logs:eu-west-2:{0}:log-group:/aws/codebuild/{1}:log-stream:*".format(self.account_id,self.project_name)
+        cloud_watch_arn = f"arn:aws:logs:{self.region}:{self.account_id}:log-group:/aws/codebuild/{self.project_name}:log-stream:*"
         policies = {"Cloud-Watch-Policy"     : { "Version": "2012-10-17",
                                                  "Statement": [{   "Effect": "Allow",
                                                                    "Action": [ "logs:CreateLogGroup"  ,
                                                                                "logs:CreateLogStream" ,
                                                                                "logs:PutLogEvents"   ],
                                                                    "Resource": [ cloud_watch_arn ]}]},
                     "Download_Image"         : { "Version": "2012-10-17",
@@ -103,15 +115,15 @@
                                                                                  "ecr:ListImages",
                                                                                  "ecr:DescribeImages",
                                                                                  "ecr:BatchGetImage"],
                                                                    "Resource": "*"}]}}
         return policies
 
     def policies__with_ecr_and_3_secrets(self):
-        cloud_watch_arn = "arn:aws:logs:eu-west-2:{0}:log-group:/aws/codebuild/{1}:log-stream:*".format(self.account_id,self.project_name)
+        cloud_watch_arn = f"arn:aws:logs:{self.region}:{self.account_id}:log-group:/aws/codebuild/{self.project_name}:log-stream:*"
         policies = {"Cloud-Watch-Policy"     : { "Version": "2012-10-17",
                                                  "Statement": [{   "Sid": "GsBotPolicy",
                                                                    "Effect": "Allow",
                                                                    "Action": [ "logs:CreateLogGroup"  ,
                                                                                "logs:CreateLogStream" ,
                                                                                "logs:PutLogEvents"   ],
                                                                    "Resource": [ cloud_watch_arn ]}]},
@@ -124,18 +136,19 @@
                                                                                  "ecr:DescribeRepositories",
                                                                                  "ecr:ListImages",
                                                                                  "ecr:DescribeImages",
                                                                                  "ecr:BatchGetImage"],
                                                                    "Resource": "*"}]},
                     "Secret-Manager"        : { "Version"  : "2012-10-17",
                                                 "Statement": [{   "Effect"  : "Allow",
-                                                                  "Action"  : [ "secretsmanager:GetSecretValue","secretsmanager:DescribeSecret"          ],
-                                                                  "Resource": [ "arn:aws:secretsmanager:eu-west-2:244560807427:secret:slack-gs-bot-*"     ,
-                                                                                "arn:aws:secretsmanager:eu-west-2:244560807427:secret:elastic*"           ,
-                                                                                "arn:aws:secretsmanager:eu-west-2:244560807427:secret:gsuite*"        ]}]}}
+                                                                  "Action"  : [  "secretsmanager:GetSecretValue","secretsmanager:DescribeSecret"          ],
+                                                                  "Resource": [ f"arn:aws:secretsmanager:{self.region}:{self.account_id}:secret:slack-gs-bot-*"     ,
+                                                                                f"arn:aws:secretsmanager:{self.region}:{self.account_id}:secret:gw-elastic*"        ,
+                                                                                f"arn:aws:secretsmanager:{self.region}:{self.account_id}:secret:gsuite*"            ,
+                                                                                f"arn:aws:secretsmanager:{self.region}:{self.account_id}:secret:git__*"         ]}]}}
         return policies
 
 
     def delete_project_role_and_policies(self):
         if self.code_build.iam.role_exists():
             policies_arns = list(self.code_build.iam.role_policies().values())
             self.code_build.iam.role_policies_detach(policies_arns)                 # first detach policies
```

### Comparing `osbot_aws-0.6.6/osbot_aws/helpers/IAM_Policy.py` & `osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Policy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from osbot_aws.apis.IAM import IAM
+from osbot_utils.utils.Dev import pformat
+
+from osbot_aws.aws.iam.IAM import IAM
 
 
 class IAM_Policy:
-    def __init__(self, policy_name=None, policy_path=None, account_id=None):
+    def __init__(self, policy_name=None, statements=None, policy_path=None, policy_arn=None):
         self.iam         = IAM()
         self.policy_name = policy_name
         self.version     = "2012-10-17"
-        self.statements  = []
+        self.statements  = statements or []
         self.policy_path = policy_path
-        self.account_id  = account_id
+        self.account_id  = self.iam.account_id()
+        self.policy_arn  = policy_arn or self.iam.policy_arn(self.policy_name, self.policy_path, self.account_id)
 
     def add_cloud_watch(self, resource_arn):
         return self.add_statement_allow(["logs:CreateLogGroup","logs:CreateLogStream","logs:PutLogEvents"], [resource_arn])
 
     def add_statement(self, effect, actions, resources):
         self.statements.append({"Effect"   : effect    ,
                                 "Action"   : actions   ,
@@ -24,21 +27,20 @@
 
     def create(self,delete_before_create=False):
         if self.policy_name is None:
             return {'status':'error', 'data':'policy name is None'}
         return self.iam.policy_create(self.policy_name, self.statement(), delete_before_create=delete_before_create)
 
     def delete(self):
-        return self.iam.policy_delete(self.policy_arn())
+        return self.iam.policy_delete(self.policy_arn)
 
     def exists(self):
-        return self.iam.policy_exists(self.policy_arn())
-
-    def policy_arn(self):
-        return self.iam.policy_arn(self.policy_name, self.policy_path, self.account_id)
+        return self.iam.policy_exists(self.policy_arn)
 
     def statement(self):
         return { 'Version' : self.version , 'Statement': self.statements}
 
     def statement_from_aws(self):
-        return self.iam.policy_statement(self.policy_arn())
+        return self.iam.policy_statement(self.policy_arn)
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}: {self.policy_name} \n { pformat(self.statements)}"
```

### Comparing `osbot_aws-0.6.6/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py` & `osbot_aws-2.5.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pbx_gs_python_utils.utils.Files import Files
+from osbot_utils.utils.Files import Files
 
 
 def run(event, context):
     file_name = event.get('file_name')                                           # get file_name from lambda params
     tmp_path  = '/tmp'                                                           # location of lambda temp folder
     tmp_file  = Files.path_combine(tmp_path,file_name)                           # create file name (in temp folder)
```


# Comparing `tmp/osbot_aws-2.5.0.tar.gz` & `tmp/osbot_aws-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osbot_aws-2.5.0.tar", max compression
+gzip compressed data, was "osbot_aws-2.6.0.tar", max compression
```

## Comparing `osbot_aws-2.5.0.tar` & `osbot_aws-2.6.0.tar`

### file list

```diff
@@ -1,217 +1,217 @@
--rw-r--r--   0        0        0    11357 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/LICENSE
--rw-r--r--   0        0        0      623 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/README.md
--rw-r--r--   0        0        0     4308 2024-05-23 23:32:44.127182 osbot_aws-2.5.0/osbot_aws/AWS_Config.py
--rw-r--r--   0        0        0       92 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/Config.py
--rw-r--r--   0        0        0     3424 2024-05-23 23:32:44.127567 osbot_aws-2.5.0/osbot_aws/Dependencies.py
--rw-r--r--   0        0        0     2596 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/OSBot_Setup.py
--rw-r--r--   0        0        0       16 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/__init__.py
--rw-r--r--   0        0        0     1137 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/ACM.py
--rw-r--r--   0        0        0    18486 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/API_Gateway.py
--rw-r--r--   0        0        0     2400 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Athena.py
--rw-r--r--   0        0        0      370 2024-02-25 00:25:50.759483 osbot_aws-2.5.0/osbot_aws/apis/Boto_Helpers.py
--rw-r--r--   0        0        0     6902 2024-02-25 00:25:50.759781 osbot_aws-2.5.0/osbot_aws/apis/Cloud_Trail.py
--rw-r--r--   0        0        0    14907 2024-04-14 17:42:52.634414 osbot_aws-2.5.0/osbot_aws/apis/Cloud_Watch.py
--rw-r--r--   0        0        0     8632 2024-05-23 23:32:44.127991 osbot_aws-2.5.0/osbot_aws/apis/Cloud_Watch_Logs.py
--rw-r--r--   0        0        0     3459 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/CodeBuild.py
--rw-r--r--   0        0        0     6297 2024-05-23 23:32:44.128273 osbot_aws-2.5.0/osbot_aws/apis/Cognito_IDP.py
--rw-r--r--   0        0        0    25047 2024-05-23 23:32:44.128631 osbot_aws-2.5.0/osbot_aws/apis/EC2.py
--rw-r--r--   0        0        0     2904 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/ECR.py
--rw-r--r--   0        0        0     5170 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Events.py
--rw-r--r--   0        0        0     4033 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/Firehose.py
--rw-r--r--   0        0        0      341 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Kinesis.py
--rw-r--r--   0        0        0    22500 2024-05-23 23:32:44.128947 osbot_aws-2.5.0/osbot_aws/apis/Lambda.py
--rw-r--r--   0        0        0      730 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Lambda_Docker.py
--rw-r--r--   0        0        0    10392 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/Lambda_Http.py
--rw-r--r--   0        0        0     7751 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/apis/Lambda_Layer.py
--rw-r--r--   0        0        0     8402 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/apis/Logs.py
--rw-r--r--   0        0        0    16253 2024-05-23 23:32:44.129321 osbot_aws-2.5.0/osbot_aws/apis/S3.py
--rw-r--r--   0        0        0     8568 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/SQS.py
--rw-r--r--   0        0        0     1161 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/SSM.py
--rw-r--r--   0        0        0     2785 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/Secrets.py
--rw-r--r--   0        0        0     8807 2024-05-23 23:32:44.129489 osbot_aws-2.5.0/osbot_aws/apis/Session.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/__init__.py
--rw-r--r--   0        0        0     2795 2024-05-23 23:32:44.129731 osbot_aws-2.5.0/osbot_aws/apis/shell/Lambda_Shell.py
--rw-r--r--   0        0        0     3904 2024-05-23 23:32:44.129966 osbot_aws-2.5.0/osbot_aws/apis/shell/Shell_Client.py
--rw-r--r--   0        0        0     2062 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/shell/Shell_Server.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/shell/__init__.py
--rw-r--r--   0        0        0     1087 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py
--rw-r--r--   0        0        0      623 2024-05-23 23:32:44.130208 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_EC2_Instance.py
--rw-r--r--   0        0        0      559 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Event_Rule.py
--rw-r--r--   0        0        0      984 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Event_Rule_To_SQS_Queue.py
--rw-r--r--   0        0        0     1433 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Folder_With_Lambda_File.py
--rw-r--r--   0        0        0      492 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_IAM_Role.py
--rw-r--r--   0        0        0      404 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_IAM_User.py
--rw-r--r--   0        0        0     3131 2024-04-14 17:42:52.634661 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Lambda.py
--rw-r--r--   0        0        0     2956 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_S3_Zip_With_Lambda_File.py
--rw-r--r--   0        0        0      868 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_SQS_Queue.py
--rw-r--r--   0        0        0     2349 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_VPC.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/apis/test_helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/__init__.py
--rw-r--r--   0        0        0     1005 2024-05-23 23:32:44.130429 osbot_aws-2.5.0/osbot_aws/aws/apigateway/API_Gateway_Management_API.py
--rw-r--r--   0        0        0      919 2024-05-23 23:32:44.130698 osbot_aws-2.5.0/osbot_aws/aws/apigateway/API_Gateway_V2.py
--rw-r--r--   0        0        0     1521 2024-05-23 23:32:44.130979 osbot_aws-2.5.0/osbot_aws/aws/apigateway/API_Gateway_V2__with_temp_role.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.130999 osbot_aws-2.5.0/osbot_aws/aws/apigateway/__init__.py
--rw-r--r--   0        0        0      945 2024-05-23 23:32:44.131326 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Connection.py
--rw-r--r--   0        0        0     5209 2024-05-23 23:32:44.131561 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__DyDB.py
--rw-r--r--   0        0        0     1219 2024-05-23 23:32:44.131784 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Events.py
--rw-r--r--   0        0        0     1454 2024-05-23 23:32:44.131965 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Lambda.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.131990 osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/__init__.py
--rw-r--r--   0        0        0      481 2024-05-23 23:32:44.132389 osbot_aws-2.5.0/osbot_aws/aws/apigateway/lambdas/Deploy__lambda_web_sockets.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.132409 osbot_aws-2.5.0/osbot_aws/aws/apigateway/lambdas/__init__.py
--rw-r--r--   0        0        0      209 2024-05-23 23:32:44.132623 osbot_aws-2.5.0/osbot_aws/aws/apigateway/lambdas/lambda_web_sockets.py
--rw-r--r--   0        0        0     3698 2024-04-14 17:42:52.635198 osbot_aws-2.5.0/osbot_aws/aws/bedrock/Bedrock.py
--rw-r--r--   0        0        0     2026 2024-04-14 17:42:52.635414 osbot_aws-2.5.0/osbot_aws/aws/bedrock/Bedrock__with_temp_role.py
--rw-r--r--   0        0        0        0 2024-02-25 00:25:50.760793 osbot_aws-2.5.0/osbot_aws/aws/bedrock/__init__.py
--rw-r--r--   0        0        0     4050 2024-05-23 23:32:44.132983 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/Bedrock__Cache.py
--rw-r--r--   0        0        0      608 2024-04-14 17:42:52.636051 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/Sqlite__Bedrock__Row.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.636072 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/__init__.py
--rw-r--r--   0        0        0     2547 2024-04-14 17:42:52.636500 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html.py
--rw-r--r--   0        0        0     8447 2024-04-14 17:42:52.636787 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_Table.py
--rw-r--r--   0        0        0     6263 2024-04-14 17:42:52.636970 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_With_Images.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.636991 osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 00:25:50.760856 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/__init__.py
--rw-r--r--   0        0        0      774 2024-04-14 17:42:52.637228 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2.py
--rw-r--r--   0        0        0      181 2024-04-14 17:42:52.637392 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Mid.py
--rw-r--r--   0        0        0      185 2024-04-14 17:42:52.637584 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Ultra.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.637604 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/ai21/__init__.py
--rw-r--r--   0        0        0     1116 2024-04-14 17:42:52.637707 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Instant_V1.py
--rw-r--r--   0        0        0     1020 2024-04-14 17:42:52.637966 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Messages_API.py
--rw-r--r--   0        0        0      205 2024-04-14 17:42:52.638255 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_0.py
--rw-r--r--   0        0        0      207 2024-04-14 17:42:52.638516 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_1.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.638563 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/__init__.py
--rw-r--r--   0        0        0     1318 2024-04-14 17:42:52.638968 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/command/Cohere_Command.py
--rw-r--r--   0        0        0      186 2024-04-14 17:42:52.639127 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Light_Text_V14.py
--rw-r--r--   0        0        0      174 2024-04-14 17:42:52.639265 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Text_V14.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.639289 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/command/__init__.py
--rw-r--r--   0        0        0      798 2024-04-14 17:42:52.639630 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion.py
--rw-r--r--   0        0        0      676 2024-04-14 17:42:52.639839 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V0.py
--rw-r--r--   0        0        0     2293 2024-04-14 17:42:52.640125 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1.py
--rw-r--r--   0        0        0     1396 2024-04-14 17:42:52.640417 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Image_To_Image.py
--rw-r--r--   0        0        0      738 2024-04-14 17:42:52.640680 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Text_To_Image.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.640707 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/__init__.py
--rw-r--r--   0        0        0      518 2024-04-14 17:42:52.640935 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2.py
--rw-r--r--   0        0        0      164 2024-04-14 17:42:52.641059 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_13b_chat_v1.py
--rw-r--r--   0        0        0      164 2024-04-14 17:42:52.641277 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_70b_chat_v1.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.641301 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/llama2/__init__.py
--rw-r--r--   0        0        0      714 2024-04-14 17:42:52.641619 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI.py
--rw-r--r--   0        0        0      175 2024-04-14 17:42:52.641785 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_7b_Instruct_v0_2.py
--rw-r--r--   0        0        0      179 2024-04-14 17:42:52.641977 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_8x7b_Instruct_v0_1.py
--rw-r--r--   0        0        0      173 2024-04-14 17:42:52.642180 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_Large_2402_v1_0.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.642201 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/__init__.py
--rw-r--r--   0        0        0     3739 2024-04-14 17:42:52.642531 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Image_Generator_V1.py
--rw-r--r--   0        0        0      348 2024-04-14 17:42:52.642642 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Express_V1.py
--rw-r--r--   0        0        0      342 2024-04-14 17:42:52.642768 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Lite_V1.py
--rw-r--r--   0        0        0      318 2024-04-14 17:42:52.642896 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Tg1_Large.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.642916 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/__init__.py
--rw-r--r--   0        0        0     1011 2024-04-14 17:42:52.643133 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/base_classes/Amazon_Titan__Text.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.643153 osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/base_classes/__init__.py
--rw-r--r--   0        0        0     1712 2024-05-23 23:32:44.133281 osbot_aws-2.5.0/osbot_aws/aws/boto3/Cache_Boto3_Requests.py
--rw-r--r--   0        0        0     2844 2024-04-14 17:42:52.643536 osbot_aws-2.5.0/osbot_aws/aws/boto3/Capture_Boto3_Error.py
--rw-r--r--   0        0        0     5978 2024-02-25 00:25:50.762274 osbot_aws-2.5.0/osbot_aws/aws/boto3/View_Boto3_Rest_Calls.py
--rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/boto3/__init__.py
--rw-r--r--   0        0        0      481 2024-05-23 23:32:44.133523 osbot_aws-2.5.0/osbot_aws/aws/cloud_front/Cloud_Front.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.133549 osbot_aws-2.5.0/osbot_aws/aws/cloud_front/__init__.py
--rw-r--r--   0        0        0    13036 2024-05-23 23:32:44.133756 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB.py
--rw-r--r--   0        0        0     1412 2024-02-25 00:25:50.762750 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Record.py
--rw-r--r--   0        0        0      280 2024-05-23 23:32:44.134071 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Streams.py
--rw-r--r--   0        0        0     6960 2024-05-23 23:32:44.134304 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Table.py
--rw-r--r--   0        0        0     1294 2024-05-23 23:32:44.134643 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__with_temp_role.py
--rw-r--r--   0        0        0     4040 2024-02-25 00:25:50.763161 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py
--rw-r--r--   0        0        0        0 2024-02-25 00:25:50.763184 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/__init__.py
--rw-r--r--   0        0        0     7015 2024-05-23 23:32:44.134885 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table.py
--rw-r--r--   0        0        0     2217 2024-05-23 23:32:44.135057 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_GSI.py
--rw-r--r--   0        0        0     4556 2024-05-23 23:32:44.135322 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_Timestamp.py
--rw-r--r--   0        0        0     1084 2024-05-23 23:32:44.135598 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table__Resources.py
--rw-r--r--   0        0        0     5693 2024-05-23 23:32:44.135789 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Timeseries.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.135813 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/__init__.py
--rw-r--r--   0        0        0     7645 2024-05-23 23:32:44.136044 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/DyDB__Document.py
--rw-r--r--   0        0        0     9656 2024-05-23 23:32:44.136231 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/DyDB__Query__Builder.py
--rw-r--r--   0        0        0      313 2024-05-23 23:32:44.136412 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/DyDB__Resource.py
--rw-r--r--   0        0        0      303 2024-05-23 23:32:44.136561 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/Resource__Config.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.136586 osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/__init__.py
--rw-r--r--   0        0        0    21575 2024-05-23 23:32:44.136922 osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS.py
--rw-r--r--   0        0        0      733 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS_Actions.py
--rw-r--r--   0        0        0      270 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS_Cluster.py
--rw-r--r--   0        0        0     7074 2024-05-23 23:32:44.137182 osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS_Fargate_Task.py
--rw-r--r--   0        0        0      631 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/ecs/Temp_ECS_Fargate_Task.py
--rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/ecs/__init__.py
--rw-r--r--   0        0        0     2398 2024-02-25 00:25:50.763337 osbot_aws-2.5.0/osbot_aws/aws/iam/Capture_IAM_Exception.py
--rw-r--r--   0        0        0    21766 2024-05-23 23:32:44.137504 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM.py
--rw-r--r--   0        0        0     9963 2024-05-23 23:32:44.137860 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Assume_Role.py
--rw-r--r--   0        0        0     1831 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Policy.py
--rw-r--r--   0        0        0     4700 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Role.py
--rw-r--r--   0        0        0     1328 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Role_With_Policy.py
--rw-r--r--   0        0        0     3041 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_User.py
--rw-r--r--   0        0        0      964 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Utils.py
--rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/aws/iam/__init__.py
--rw-r--r--   0        0        0     2029 2024-05-23 23:32:44.137977 osbot_aws-2.5.0/osbot_aws/aws/lambda_/Lambda__with_temp_role.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.137999 osbot_aws-2.5.0/osbot_aws/aws/lambda_/__init__.py
--rw-r--r--   0        0        0     5975 2024-05-23 23:32:44.138252 osbot_aws-2.5.0/osbot_aws/aws/route_53/Route_53.py
--rw-r--r--   0        0        0     2226 2024-05-23 23:32:44.138424 osbot_aws-2.5.0/osbot_aws/aws/route_53/Route_53__Hosted_Zone.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.138445 osbot_aws-2.5.0/osbot_aws/aws/route_53/__init__.py
--rw-r--r--   0        0        0     1458 2024-05-23 23:32:44.138582 osbot_aws-2.5.0/osbot_aws/aws/s3/S3__with_temp_role.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.138606 osbot_aws-2.5.0/osbot_aws/aws/s3/__init__.py
--rw-r--r--   0        0        0     4849 2024-05-23 23:32:44.138710 osbot_aws-2.5.0/osbot_aws/aws/sts/STS.py
--rw-r--r--   0        0        0        0 2024-05-23 23:32:44.138729 osbot_aws-2.5.0/osbot_aws/aws/sts/__init__.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/decorators/__init__.py
--rw-r--r--   0        0        0      808 2024-05-23 23:32:44.139074 osbot_aws-2.5.0/osbot_aws/decorators/aws_inject.py
--rw-r--r--   0        0        0      942 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/decorators/aws_retry.py
--rw-r--r--   0        0        0     2913 2024-05-23 23:32:44.139253 osbot_aws-2.5.0/osbot_aws/decorators/enforce_type_safety.py
--rw-r--r--   0        0        0      686 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/decorators/lambda_save_event.py
--rw-r--r--   0        0        0     4865 2024-05-23 23:32:44.139496 osbot_aws-2.5.0/osbot_aws/deploy/Deploy_Lambda.py
--rw-r--r--   0        0        0     1367 2024-05-23 23:32:44.139753 osbot_aws-2.5.0/osbot_aws/deploy/TestCase__Lambda__Deploy.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/deploy/__init__.py
--rw-r--r--   0        0        0      948 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/exceptions/Session_Bad_Credentials.py
--rw-r--r--   0        0        0      330 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/exceptions/Session_Client_Creation_Fail.py
--rw-r--r--   0        0        0      610 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/exceptions/Session_No_Credentials.py
--rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/exceptions/__init__.py
--rw-r--r--   0        0        0      959 2024-05-23 23:32:44.139975 osbot_aws-2.5.0/osbot_aws/helpers/AMI.py
--rw-r--r--   0        0        0     2595 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/Aws_Cli.py
--rw-r--r--   0        0        0    11778 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Create_Code_Build.py
--rw-r--r--   0        0        0     2920 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Create_Image_ECR.py
--rw-r--r--   0        0        0     2038 2024-05-23 23:32:44.140289 osbot_aws-2.5.0/osbot_aws/helpers/EC_Instance.py
--rw-r--r--   0        0        0     2544 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/Event_Rule.py
--rw-r--r--   0        0        0       61 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_From_S3.py
--rw-r--r--   0        0        0     1771 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Helpers.py
--rw-r--r--   0        0        0     6311 2024-05-23 23:32:44.140523 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Layer_Create.py
--rw-r--r--   0        0        0      494 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Layers_Local.py
--rw-r--r--   0        0        0     2845 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Layers_OSBot.py
--rw-r--r--   0        0        0     8284 2024-05-23 23:32:44.140788 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Package.py
--rw-r--r--   0        0        0     2001 2024-05-23 23:32:44.141011 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_SSH.py
--rw-r--r--   0        0        0     1247 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_SSH_Kubectl.py
--rw-r--r--   0        0        0     1338 2024-05-23 23:32:44.141238 osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Upload_Package.py
--rw-r--r--   0        0        0     2154 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/Parameter.py
--rw-r--r--   0        0        0     4127 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Rest_API.py
--rw-r--r--   0        0        0     1497 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/helpers/S3_Zip_From_Files.py
--rw-r--r--   0        0        0     5565 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/SQS_Queue.py
--rw-r--r--   0        0        0     1562 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/helpers/Test_Helper.py
--rw-r--r--   0        0        0     2181 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/VPC.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/__init__.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/__init__.py
--rw-r--r--   0        0        0      127 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/check_aws_api.py
--rw-r--r--   0        0        0      139 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/check_python_utils.py
--rw-r--r--   0        0        0       87 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/hello_world.py
--rw-r--r--   0        0        0      137 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/lambda_layer.py
--rw-r--r--   0        0        0      326 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/write_cloud_watch_log.py
--rw-r--r--   0        0        0      221 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/dev/write_queue.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/pocs/__init__.py
--rw-r--r--   0        0        0      353 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/pocs/confirm_process_stay_alive.py
--rw-r--r--   0        0        0      648 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py
--rw-r--r--   0        0        0      230 2023-12-30 21:56:08.000000 osbot_aws-2.5.0/osbot_aws/lambdas/pocs/send_event_data_to_queue.py
--rw-r--r--   0        0        0     1916 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/server_ssh.py
--rw-r--r--   0        0        0        0 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/shell/__init__.py
--rw-r--r--   0        0        0      138 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/shell/lambda_shell.py
--rw-r--r--   0        0        0      129 2023-12-30 19:01:04.000000 osbot_aws-2.5.0/osbot_aws/lambdas/shell/shell_server.py
--rw-r--r--   0        0        0      575 2024-05-23 23:32:44.141344 osbot_aws-2.5.0/osbot_aws/testing/TestCase__API_Gateway_V2.py
--rw-r--r--   0        0        0      973 2024-05-23 23:32:44.141654 osbot_aws-2.5.0/osbot_aws/testing/TestCase__Bedrock.py
--rw-r--r--   0        0        0      431 2024-05-23 23:32:44.141813 osbot_aws-2.5.0/osbot_aws/testing/TestCase__Boto3_Cache.py
--rw-r--r--   0        0        0      525 2024-05-23 23:32:44.142025 osbot_aws-2.5.0/osbot_aws/testing/TestCase__Dynamo_DB.py
--rw-r--r--   0        0        0     1707 2024-05-23 23:32:44.142128 osbot_aws-2.5.0/osbot_aws/testing/TestCase__Lambda.py
--rw-r--r--   0        0        0        0 2024-04-14 17:42:52.645306 osbot_aws-2.5.0/osbot_aws/testing/__init__.py
--rw-r--r--   0        0        0       91 2024-05-23 23:32:44.142381 osbot_aws-2.5.0/osbot_aws/utils/Execution_Env.py
--rw-r--r--   0        0        0      458 2024-05-23 23:32:44.142603 osbot_aws-2.5.0/osbot_aws/utils/Version.py
--rw-r--r--   0        0        0        0 2024-02-15 10:53:20.000000 osbot_aws-2.5.0/osbot_aws/utils/__init__.py
--rw-r--r--   0        0        0        7 2024-05-23 23:35:39.958222 osbot_aws-2.5.0/osbot_aws/version
--rw-r--r--   0        0        0      677 2024-05-23 23:32:44.143272 osbot_aws-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 osbot_aws-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/LICENSE
+-rw-r--r--   0        0        0      636 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/README.md
+-rw-r--r--   0        0        0     4308 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/AWS_Config.py
+-rw-r--r--   0        0        0       92 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/Config.py
+-rw-r--r--   0        0        0     3424 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/Dependencies.py
+-rw-r--r--   0        0        0     2596 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/OSBot_Setup.py
+-rw-r--r--   0        0        0       16 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/__init__.py
+-rw-r--r--   0        0        0     1137 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/ACM.py
+-rw-r--r--   0        0        0    18486 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/API_Gateway.py
+-rw-r--r--   0        0        0     2400 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/Athena.py
+-rw-r--r--   0        0        0      370 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/Boto_Helpers.py
+-rw-r--r--   0        0        0     6902 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/Cloud_Trail.py
+-rw-r--r--   0        0        0    14907 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/Cloud_Watch.py
+-rw-r--r--   0        0        0     8632 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/Cloud_Watch_Logs.py
+-rw-r--r--   0        0        0     3459 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/CodeBuild.py
+-rw-r--r--   0        0        0     6297 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/Cognito_IDP.py
+-rw-r--r--   0        0        0    25047 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/EC2.py
+-rw-r--r--   0        0        0     2904 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/ECR.py
+-rw-r--r--   0        0        0     5170 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/Events.py
+-rw-r--r--   0        0        0     4033 2024-05-24 09:45:45.954514 osbot_aws-2.6.0/osbot_aws/apis/Firehose.py
+-rw-r--r--   0        0        0      341 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/Kinesis.py
+-rw-r--r--   0        0        0    22500 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/Lambda.py
+-rw-r--r--   0        0        0      730 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/Lambda_Docker.py
+-rw-r--r--   0        0        0    10392 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/Lambda_Http.py
+-rw-r--r--   0        0        0     7751 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/Lambda_Layer.py
+-rw-r--r--   0        0        0     8402 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/Logs.py
+-rw-r--r--   0        0        0    16253 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/S3.py
+-rw-r--r--   0        0        0     8568 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/SQS.py
+-rw-r--r--   0        0        0     1161 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/SSM.py
+-rw-r--r--   0        0        0     2785 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/Secrets.py
+-rw-r--r--   0        0        0     8807 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/Session.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/__init__.py
+-rw-r--r--   0        0        0     2795 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/shell/Lambda_Shell.py
+-rw-r--r--   0        0        0     3904 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/shell/Shell_Client.py
+-rw-r--r--   0        0        0     2062 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/shell/Shell_Server.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/shell/__init__.py
+-rw-r--r--   0        0        0     1087 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py
+-rw-r--r--   0        0        0      623 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_EC2_Instance.py
+-rw-r--r--   0        0        0      559 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Event_Rule.py
+-rw-r--r--   0        0        0      984 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Event_Rule_To_SQS_Queue.py
+-rw-r--r--   0        0        0     1433 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Folder_With_Lambda_File.py
+-rw-r--r--   0        0        0      492 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_IAM_Role.py
+-rw-r--r--   0        0        0      404 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_IAM_User.py
+-rw-r--r--   0        0        0     3131 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Lambda.py
+-rw-r--r--   0        0        0     2956 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_S3_Zip_With_Lambda_File.py
+-rw-r--r--   0        0        0      868 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_SQS_Queue.py
+-rw-r--r--   0        0        0     2349 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_VPC.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/apis/test_helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/API_Gateway_Management_API.py
+-rw-r--r--   0        0        0      919 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/API_Gateway_V2.py
+-rw-r--r--   0        0        0     1521 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/API_Gateway_V2__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/__init__.py
+-rw-r--r--   0        0        0      945 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Connection.py
+-rw-r--r--   0        0        0     5209 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/apigw_dydb/WS__DyDB.py
+-rw-r--r--   0        0        0     1219 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Events.py
+-rw-r--r--   0        0        0     1454 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Lambda.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/apigw_dydb/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/lambdas/Deploy__lambda_web_sockets.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/lambdas/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/apigateway/lambdas/lambda_web_sockets.py
+-rw-r--r--   0        0        0     3698 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/Bedrock.py
+-rw-r--r--   0        0        0     2026 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/Bedrock__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/__init__.py
+-rw-r--r--   0        0        0     4050 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/Bedrock__Cache.py
+-rw-r--r--   0        0        0      608 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/Sqlite__Bedrock__Row.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/__init__.py
+-rw-r--r--   0        0        0     2547 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html.py
+-rw-r--r--   0        0        0     8447 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_Table.py
+-rw-r--r--   0        0        0     6263 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_With_Images.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/html/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2.py
+-rw-r--r--   0        0        0      181 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Mid.py
+-rw-r--r--   0        0        0      185 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2_Ultra.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/ai21/__init__.py
+-rw-r--r--   0        0        0     1116 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Instant_V1.py
+-rw-r--r--   0        0        0     1020 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Messages_API.py
+-rw-r--r--   0        0        0      205 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_0.py
+-rw-r--r--   0        0        0      207 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_V2_1.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/claude/__init__.py
+-rw-r--r--   0        0        0     1318 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/command/Cohere_Command.py
+-rw-r--r--   0        0        0      186 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Light_Text_V14.py
+-rw-r--r--   0        0        0      174 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/command/Cohere_Command_Text_V14.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/command/__init__.py
+-rw-r--r--   0        0        0      798 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion.py
+-rw-r--r--   0        0        0      676 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V0.py
+-rw-r--r--   0        0        0     2293 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1.py
+-rw-r--r--   0        0        0     1396 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Image_To_Image.py
+-rw-r--r--   0        0        0      738 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Text_To_Image.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/__init__.py
+-rw-r--r--   0        0        0      518 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2.py
+-rw-r--r--   0        0        0      164 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_13b_chat_v1.py
+-rw-r--r--   0        0        0      164 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2_70b_chat_v1.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/llama2/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI.py
+-rw-r--r--   0        0        0      175 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_7b_Instruct_v0_2.py
+-rw-r--r--   0        0        0      179 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_8x7b_Instruct_v0_1.py
+-rw-r--r--   0        0        0      173 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI_Large_2402_v1_0.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/mistral/__init__.py
+-rw-r--r--   0        0        0     3739 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Image_Generator_V1.py
+-rw-r--r--   0        0        0      348 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Express_V1.py
+-rw-r--r--   0        0        0      342 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Text_Lite_V1.py
+-rw-r--r--   0        0        0      318 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Tg1_Large.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/titan/__init__.py
+-rw-r--r--   0        0        0     1011 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/titan/base_classes/Amazon_Titan__Text.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/titan/base_classes/__init__.py
+-rw-r--r--   0        0        0     1712 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/boto3/Cache_Boto3_Requests.py
+-rw-r--r--   0        0        0     2844 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/boto3/Capture_Boto3_Error.py
+-rw-r--r--   0        0        0     5978 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/boto3/View_Boto3_Rest_Calls.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/boto3/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/cloud_front/Cloud_Front.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.958514 osbot_aws-2.6.0/osbot_aws/aws/cloud_front/__init__.py
+-rw-r--r--   0        0        0    13036 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_DB.py
+-rw-r--r--   0        0        0     1412 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Record.py
+-rw-r--r--   0        0        0      280 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Streams.py
+-rw-r--r--   0        0        0     6960 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Table.py
+-rw-r--r--   0        0        0     1294 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_DB__with_temp_role.py
+-rw-r--r--   0        0        0     4040 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/__init__.py
+-rw-r--r--   0        0        0     7015 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table.py
+-rw-r--r--   0        0        0     2217 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_GSI.py
+-rw-r--r--   0        0        0     4556 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_Timestamp.py
+-rw-r--r--   0        0        0     1084 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table__Resources.py
+-rw-r--r--   0        0        0     5693 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Timeseries.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/__init__.py
+-rw-r--r--   0        0        0     7645 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/models/DyDB__Document.py
+-rw-r--r--   0        0        0     9656 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/models/DyDB__Query__Builder.py
+-rw-r--r--   0        0        0      313 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/models/DyDB__Resource.py
+-rw-r--r--   0        0        0      303 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/models/Resource__Config.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/models/__init__.py
+-rw-r--r--   0        0        0    21575 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/ecs/ECS.py
+-rw-r--r--   0        0        0      733 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/ecs/ECS_Actions.py
+-rw-r--r--   0        0        0      270 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/ecs/ECS_Cluster.py
+-rw-r--r--   0        0        0     7074 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/ecs/ECS_Fargate_Task.py
+-rw-r--r--   0        0        0      631 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/ecs/Temp_ECS_Fargate_Task.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/ecs/__init__.py
+-rw-r--r--   0        0        0     2398 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/iam/Capture_IAM_Exception.py
+-rw-r--r--   0        0        0    21766 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/iam/IAM.py
+-rw-r--r--   0        0        0     9963 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Assume_Role.py
+-rw-r--r--   0        0        0     1831 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Policy.py
+-rw-r--r--   0        0        0     4700 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Role.py
+-rw-r--r--   0        0        0     1328 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Role_With_Policy.py
+-rw-r--r--   0        0        0     3041 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_User.py
+-rw-r--r--   0        0        0      964 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Utils.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/iam/__init__.py
+-rw-r--r--   0        0        0     2029 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/lambda_/Lambda__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/lambda_/__init__.py
+-rw-r--r--   0        0        0     5975 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/route_53/Route_53.py
+-rw-r--r--   0        0        0     2226 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/route_53/Route_53__Hosted_Zone.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/route_53/__init__.py
+-rw-r--r--   0        0        0     1458 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/s3/S3__with_temp_role.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/s3/__init__.py
+-rw-r--r--   0        0        0     4849 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/sts/STS.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/aws/sts/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      808 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/decorators/aws_inject.py
+-rw-r--r--   0        0        0      942 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/decorators/aws_retry.py
+-rw-r--r--   0        0        0     2913 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/decorators/enforce_type_safety.py
+-rw-r--r--   0        0        0      686 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/decorators/lambda_save_event.py
+-rw-r--r--   0        0        0     4865 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/deploy/Deploy_Lambda.py
+-rw-r--r--   0        0        0     1367 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/deploy/TestCase__Lambda__Deploy.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/deploy/__init__.py
+-rw-r--r--   0        0        0      948 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/exceptions/Session_Bad_Credentials.py
+-rw-r--r--   0        0        0      330 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/exceptions/Session_Client_Creation_Fail.py
+-rw-r--r--   0        0        0      610 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/exceptions/Session_No_Credentials.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/exceptions/__init__.py
+-rw-r--r--   0        0        0      959 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/AMI.py
+-rw-r--r--   0        0        0     2595 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Aws_Cli.py
+-rw-r--r--   0        0        0    11778 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Create_Code_Build.py
+-rw-r--r--   0        0        0     2920 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Create_Image_ECR.py
+-rw-r--r--   0        0        0     2038 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/EC_Instance.py
+-rw-r--r--   0        0        0     2544 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Event_Rule.py
+-rw-r--r--   0        0        0       61 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Lambda_From_S3.py
+-rw-r--r--   0        0        0     1771 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Helpers.py
+-rw-r--r--   0        0        0     6311 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Layer_Create.py
+-rw-r--r--   0        0        0      494 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Layers_Local.py
+-rw-r--r--   0        0        0     2845 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Layers_OSBot.py
+-rw-r--r--   0        0        0     8284 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Package.py
+-rw-r--r--   0        0        0     2001 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Lambda_SSH.py
+-rw-r--r--   0        0        0     1247 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Lambda_SSH_Kubectl.py
+-rw-r--r--   0        0        0     1338 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Upload_Package.py
+-rw-r--r--   0        0        0     2154 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Parameter.py
+-rw-r--r--   0        0        0     4127 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Rest_API.py
+-rw-r--r--   0        0        0     1497 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/S3_Zip_From_Files.py
+-rw-r--r--   0        0        0     5565 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/SQS_Queue.py
+-rw-r--r--   0        0        0     1562 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/Test_Helper.py
+-rw-r--r--   0        0        0     2181 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/VPC.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/dev/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/dev/check_aws_api.py
+-rw-r--r--   0        0        0      139 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/dev/check_python_utils.py
+-rw-r--r--   0        0        0       87 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/dev/hello_world.py
+-rw-r--r--   0        0        0      137 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/dev/lambda_layer.py
+-rw-r--r--   0        0        0      326 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/dev/write_cloud_watch_log.py
+-rw-r--r--   0        0        0      221 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/dev/write_queue.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/pocs/__init__.py
+-rw-r--r--   0        0        0      353 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/pocs/confirm_process_stay_alive.py
+-rw-r--r--   0        0        0      648 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py
+-rw-r--r--   0        0        0      230 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/pocs/send_event_data_to_queue.py
+-rw-r--r--   0        0        0     1916 2024-05-24 09:45:45.962514 osbot_aws-2.6.0/osbot_aws/lambdas/server_ssh.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/lambdas/shell/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/lambdas/shell/lambda_shell.py
+-rw-r--r--   0        0        0      129 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/lambdas/shell/shell_server.py
+-rw-r--r--   0        0        0      575 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/testing/TestCase__API_Gateway_V2.py
+-rw-r--r--   0        0        0      973 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/testing/TestCase__Bedrock.py
+-rw-r--r--   0        0        0      431 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/testing/TestCase__Boto3_Cache.py
+-rw-r--r--   0        0        0      525 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/testing/TestCase__Dynamo_DB.py
+-rw-r--r--   0        0        0     1707 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/testing/TestCase__Lambda.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/testing/__init__.py
+-rw-r--r--   0        0        0       91 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/utils/Execution_Env.py
+-rw-r--r--   0        0        0      458 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/utils/Version.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/utils/__init__.py
+-rw-r--r--   0        0        0        7 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/osbot_aws/version
+-rw-r--r--   0        0        0      677 2024-05-24 09:45:45.966514 osbot_aws-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1277 1970-01-01 00:00:00.000000 osbot_aws-2.6.0/PKG-INFO
```

### Comparing `osbot_aws-2.5.0/LICENSE` & `osbot_aws-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/README.md` & `osbot_aws-2.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # OSBot-AWS
-Large number of AWS apis and utils from the OWASP Security Bot (OSBot) which make
-the use of AWS's boto3 library easier and more intuitive.
 
-### Install
+![Current Release](https://img.shields.io/badge/release-v2.6.0-blue)
 
-Current stable release is v1.0.0 and is available here 
-
-https://github.com/owasp-sbot/OSBot-AWS/releases/tag/v1.0.0
+Large number of AWS apis and utils from the OWASP Security Bot (OSBot) which make
+the use of AWS's boto3 library easier and more intuitive.
 
-## curent dev version is 2.x.x 
+## Current version is 2.x.x 
 
 This version has a number of breaking changes, mainly on the location of the apis, 
-since we are moving into a spefici folder per service (e.g. S3, SQS, etc)
+since we are moving into a specific folder per service (e.g. S3, SQS, etc)
 
 ### Install from PyPi
 
-There is a version in PyPi (which is not the latest version)
-
 `pip3 install osbot-aws`
 
 https://pypi.org/project/osbot-aws/
+
+### Previous release
+
+Previous stable release is v1.0.0 and is available at https://github.com/owasp-sbot/OSBot-AWS/releases/tag/v1.0.0
```

### Comparing `osbot_aws-2.5.0/osbot_aws/AWS_Config.py` & `osbot_aws-2.6.0/osbot_aws/AWS_Config.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/Dependencies.py` & `osbot_aws-2.6.0/osbot_aws/Dependencies.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/OSBot_Setup.py` & `osbot_aws-2.6.0/osbot_aws/OSBot_Setup.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/ACM.py` & `osbot_aws-2.6.0/osbot_aws/apis/ACM.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/API_Gateway.py` & `osbot_aws-2.6.0/osbot_aws/apis/API_Gateway.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Athena.py` & `osbot_aws-2.6.0/osbot_aws/apis/Athena.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Cloud_Trail.py` & `osbot_aws-2.6.0/osbot_aws/apis/Cloud_Trail.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Cloud_Watch.py` & `osbot_aws-2.6.0/osbot_aws/apis/Cloud_Watch.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Cloud_Watch_Logs.py` & `osbot_aws-2.6.0/osbot_aws/apis/Cloud_Watch_Logs.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/CodeBuild.py` & `osbot_aws-2.6.0/osbot_aws/apis/CodeBuild.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Cognito_IDP.py` & `osbot_aws-2.6.0/osbot_aws/apis/Cognito_IDP.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/EC2.py` & `osbot_aws-2.6.0/osbot_aws/apis/EC2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/ECR.py` & `osbot_aws-2.6.0/osbot_aws/apis/ECR.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Events.py` & `osbot_aws-2.6.0/osbot_aws/apis/Events.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Firehose.py` & `osbot_aws-2.6.0/osbot_aws/apis/Firehose.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Lambda.py` & `osbot_aws-2.6.0/osbot_aws/apis/Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Lambda_Docker.py` & `osbot_aws-2.6.0/osbot_aws/apis/Lambda_Docker.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Lambda_Http.py` & `osbot_aws-2.6.0/osbot_aws/apis/Lambda_Http.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Lambda_Layer.py` & `osbot_aws-2.6.0/osbot_aws/apis/Lambda_Layer.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Logs.py` & `osbot_aws-2.6.0/osbot_aws/apis/Logs.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/S3.py` & `osbot_aws-2.6.0/osbot_aws/apis/S3.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/SQS.py` & `osbot_aws-2.6.0/osbot_aws/apis/SQS.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/SSM.py` & `osbot_aws-2.6.0/osbot_aws/apis/SSM.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Secrets.py` & `osbot_aws-2.6.0/osbot_aws/apis/Secrets.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/Session.py` & `osbot_aws-2.6.0/osbot_aws/apis/Session.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/shell/Lambda_Shell.py` & `osbot_aws-2.6.0/osbot_aws/apis/shell/Lambda_Shell.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/shell/Shell_Client.py` & `osbot_aws-2.6.0/osbot_aws/apis/shell/Shell_Client.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/shell/Shell_Server.py` & `osbot_aws-2.6.0/osbot_aws/apis/shell/Shell_Server.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py` & `osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Aws_Roles.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_EC2_Instance.py` & `osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_EC2_Instance.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Event_Rule.py` & `osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Event_Rule.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Event_Rule_To_SQS_Queue.py` & `osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Event_Rule_To_SQS_Queue.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Folder_With_Lambda_File.py` & `osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Folder_With_Lambda_File.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_Lambda.py` & `osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_S3_Zip_With_Lambda_File.py` & `osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_S3_Zip_With_Lambda_File.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_SQS_Queue.py` & `osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_SQS_Queue.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/apis/test_helpers/Temp_VPC.py` & `osbot_aws-2.6.0/osbot_aws/apis/test_helpers/Temp_VPC.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/apigateway/API_Gateway_Management_API.py` & `osbot_aws-2.6.0/osbot_aws/aws/apigateway/API_Gateway_Management_API.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/apigateway/API_Gateway_V2.py` & `osbot_aws-2.6.0/osbot_aws/aws/apigateway/API_Gateway_V2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/apigateway/API_Gateway_V2__with_temp_role.py` & `osbot_aws-2.6.0/osbot_aws/aws/apigateway/API_Gateway_V2__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Connection.py` & `osbot_aws-2.6.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Connection.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__DyDB.py` & `osbot_aws-2.6.0/osbot_aws/aws/apigateway/apigw_dydb/WS__DyDB.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Events.py` & `osbot_aws-2.6.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Events.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Lambda.py` & `osbot_aws-2.6.0/osbot_aws/aws/apigateway/apigw_dydb/WS__Handle_Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/Bedrock.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/Bedrock.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/Bedrock__with_temp_role.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/Bedrock__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/Bedrock__Cache.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/Bedrock__Cache.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/Sqlite__Bedrock__Row.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/Sqlite__Bedrock__Row.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_Table.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_Table.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_With_Images.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/cache/html/Bedrock_Cache__Html_With_Images.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/ai21/AI21_Labs_Jurassic_2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Instant_V1.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Instant_V1.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Messages_API.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/claude/Anthropic__Claude_Messages_API.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/command/Cohere_Command.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/command/Cohere_Command.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V0.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V0.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Image_To_Image.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Image_To_Image.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Text_To_Image.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/diffusion/Stability_Stable_Diffusion_XL_V1__Text_To_Image.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/llama2/Meta_Llama2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/mistral/Mistral_AI.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Image_Generator_V1.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/titan/Amazon_Titan_Image_Generator_V1.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/bedrock/models/titan/base_classes/Amazon_Titan__Text.py` & `osbot_aws-2.6.0/osbot_aws/aws/bedrock/models/titan/base_classes/Amazon_Titan__Text.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/boto3/Cache_Boto3_Requests.py` & `osbot_aws-2.6.0/osbot_aws/aws/boto3/Cache_Boto3_Requests.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/boto3/Capture_Boto3_Error.py` & `osbot_aws-2.6.0/osbot_aws/aws/boto3/Capture_Boto3_Error.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/boto3/View_Boto3_Rest_Calls.py` & `osbot_aws-2.6.0/osbot_aws/aws/boto3/View_Boto3_Rest_Calls.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_DB.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Record.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Record.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Table.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_DB__Table.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_DB__with_temp_role.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_DB__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/Dynamo_Table__Resource.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_GSI.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_GSI.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_Timestamp.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table_With_Timestamp.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table__Resources.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Table__Resources.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/domains/DyDB__Timeseries.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/domains/DyDB__Timeseries.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/DyDB__Document.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/models/DyDB__Document.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/dynamo_db/models/DyDB__Query__Builder.py` & `osbot_aws-2.6.0/osbot_aws/aws/dynamo_db/models/DyDB__Query__Builder.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS.py` & `osbot_aws-2.6.0/osbot_aws/aws/ecs/ECS.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS_Actions.py` & `osbot_aws-2.6.0/osbot_aws/aws/ecs/ECS_Actions.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/ecs/ECS_Fargate_Task.py` & `osbot_aws-2.6.0/osbot_aws/aws/ecs/ECS_Fargate_Task.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/ecs/Temp_ECS_Fargate_Task.py` & `osbot_aws-2.6.0/osbot_aws/aws/ecs/Temp_ECS_Fargate_Task.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/iam/Capture_IAM_Exception.py` & `osbot_aws-2.6.0/osbot_aws/aws/iam/Capture_IAM_Exception.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/iam/IAM.py` & `osbot_aws-2.6.0/osbot_aws/aws/iam/IAM.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Assume_Role.py` & `osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Assume_Role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Policy.py` & `osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Policy.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Role.py` & `osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Role_With_Policy.py` & `osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Role_With_Policy.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_User.py` & `osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_User.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/iam/IAM_Utils.py` & `osbot_aws-2.6.0/osbot_aws/aws/iam/IAM_Utils.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/lambda_/Lambda__with_temp_role.py` & `osbot_aws-2.6.0/osbot_aws/aws/lambda_/Lambda__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/route_53/Route_53.py` & `osbot_aws-2.6.0/osbot_aws/aws/route_53/Route_53.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/route_53/Route_53__Hosted_Zone.py` & `osbot_aws-2.6.0/osbot_aws/aws/route_53/Route_53__Hosted_Zone.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/s3/S3__with_temp_role.py` & `osbot_aws-2.6.0/osbot_aws/aws/s3/S3__with_temp_role.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/aws/sts/STS.py` & `osbot_aws-2.6.0/osbot_aws/aws/sts/STS.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/decorators/aws_inject.py` & `osbot_aws-2.6.0/osbot_aws/decorators/aws_inject.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/decorators/aws_retry.py` & `osbot_aws-2.6.0/osbot_aws/decorators/aws_retry.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/decorators/enforce_type_safety.py` & `osbot_aws-2.6.0/osbot_aws/decorators/enforce_type_safety.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/decorators/lambda_save_event.py` & `osbot_aws-2.6.0/osbot_aws/decorators/lambda_save_event.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/deploy/Deploy_Lambda.py` & `osbot_aws-2.6.0/osbot_aws/deploy/Deploy_Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/deploy/TestCase__Lambda__Deploy.py` & `osbot_aws-2.6.0/osbot_aws/deploy/TestCase__Lambda__Deploy.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/exceptions/Session_Bad_Credentials.py` & `osbot_aws-2.6.0/osbot_aws/exceptions/Session_Bad_Credentials.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/exceptions/Session_No_Credentials.py` & `osbot_aws-2.6.0/osbot_aws/exceptions/Session_No_Credentials.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/AMI.py` & `osbot_aws-2.6.0/osbot_aws/helpers/AMI.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Aws_Cli.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Aws_Cli.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Create_Code_Build.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Create_Code_Build.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Create_Image_ECR.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Create_Image_ECR.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/EC_Instance.py` & `osbot_aws-2.6.0/osbot_aws/helpers/EC_Instance.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Event_Rule.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Event_Rule.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Helpers.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Helpers.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Layer_Create.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Layer_Create.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Layers_OSBot.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Layers_OSBot.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Package.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Package.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Lambda_SSH.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Lambda_SSH.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Lambda_SSH_Kubectl.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Lambda_SSH_Kubectl.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Lambda_Upload_Package.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Lambda_Upload_Package.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Parameter.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Parameter.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Rest_API.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Rest_API.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/S3_Zip_From_Files.py` & `osbot_aws-2.6.0/osbot_aws/helpers/S3_Zip_From_Files.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/SQS_Queue.py` & `osbot_aws-2.6.0/osbot_aws/helpers/SQS_Queue.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/Test_Helper.py` & `osbot_aws-2.6.0/osbot_aws/helpers/Test_Helper.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/helpers/VPC.py` & `osbot_aws-2.6.0/osbot_aws/helpers/VPC.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py` & `osbot_aws-2.6.0/osbot_aws/lambdas/pocs/confirm_tmp_reuse.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/lambdas/server_ssh.py` & `osbot_aws-2.6.0/osbot_aws/lambdas/server_ssh.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/testing/TestCase__API_Gateway_V2.py` & `osbot_aws-2.6.0/osbot_aws/testing/TestCase__API_Gateway_V2.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/testing/TestCase__Bedrock.py` & `osbot_aws-2.6.0/osbot_aws/testing/TestCase__Bedrock.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/testing/TestCase__Dynamo_DB.py` & `osbot_aws-2.6.0/osbot_aws/testing/TestCase__Dynamo_DB.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/osbot_aws/testing/TestCase__Lambda.py` & `osbot_aws-2.6.0/osbot_aws/testing/TestCase__Lambda.py`

 * *Files identical despite different names*

### Comparing `osbot_aws-2.5.0/pyproject.toml` & `osbot_aws-2.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name        = "osbot_aws"
-version     = "v2.5.0"
+version     = "v2.6.0"
 description = "OWASP Security Bot - AWS"
 authors     = ["Dinis Cruz <dinis.cruz@owasp.org>"]
 license     = "MIT"
 readme      = "README.md"
 homepage    = "https://github.com/owasp-sbot/OSBot-AWS"
 repository  = "https://github.com/owasp-sbot/OSBot-AWS"
```

### Comparing `osbot_aws-2.5.0/PKG-INFO` & `osbot_aws-2.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osbot_aws
-Version: 2.5.0
+Version: 2.6.0
 Summary: OWASP Security Bot - AWS
 Home-page: https://github.com/owasp-sbot/OSBot-AWS
 License: MIT
 Author: Dinis Cruz
 Author-email: dinis.cruz@owasp.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,29 +15,28 @@
 Requires-Dist: osbot-utils
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Project-URL: Repository, https://github.com/owasp-sbot/OSBot-AWS
 Description-Content-Type: text/markdown
 
 # OSBot-AWS
-Large number of AWS apis and utils from the OWASP Security Bot (OSBot) which make
-the use of AWS's boto3 library easier and more intuitive.
 
-### Install
+![Current Release](https://img.shields.io/badge/release-v2.6.0-blue)
 
-Current stable release is v1.0.0 and is available here 
-
-https://github.com/owasp-sbot/OSBot-AWS/releases/tag/v1.0.0
+Large number of AWS apis and utils from the OWASP Security Bot (OSBot) which make
+the use of AWS's boto3 library easier and more intuitive.
 
-## curent dev version is 2.x.x 
+## Current version is 2.x.x 
 
 This version has a number of breaking changes, mainly on the location of the apis, 
-since we are moving into a spefici folder per service (e.g. S3, SQS, etc)
+since we are moving into a specific folder per service (e.g. S3, SQS, etc)
 
 ### Install from PyPi
 
-There is a version in PyPi (which is not the latest version)
-
 `pip3 install osbot-aws`
 
 https://pypi.org/project/osbot-aws/
 
+### Previous release
+
+Previous stable release is v1.0.0 and is available at https://github.com/owasp-sbot/OSBot-AWS/releases/tag/v1.0.0
+
```


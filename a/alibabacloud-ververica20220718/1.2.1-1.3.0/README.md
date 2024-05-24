# Comparing `tmp/alibabacloud_ververica20220718-1.2.1.tar.gz` & `tmp/alibabacloud_ververica20220718-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ververica20220718-1.2.1.tar", last modified: Mon Nov 13 17:16:18 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ververica20220718-1.3.0.tar", last modified: Fri May 24 17:09:03 2024, max compression
```

## Comparing `alibabacloud_ververica20220718-1.2.1.tar` & `alibabacloud_ververica20220718-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      216 2023-11-13 17:16:17.000000 alibabacloud_ververica20220718-1.2.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-11-13 17:16:17.000000 alibabacloud_ververica20220718-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-11-13 17:16:17.000000 alibabacloud_ververica20220718-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-11-13 17:16:17.000000 alibabacloud_ververica20220718-1.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-11-13 17:16:17.000000 alibabacloud_ververica20220718-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718/
--rw-r--r--   0 root         (0) root         (0)       21 2023-11-13 17:16:17.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718/__init__.py
--rw-r--r--   0 root         (0) root         (0)   103255 2023-11-13 17:16:17.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718/client.py
--rw-r--r--   0 root         (0) root         (0)   195874 2023-11-13 17:16:17.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-11-13 17:16:18.000000 alibabacloud_ververica20220718-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2641 2023-11-13 17:16:17.000000 alibabacloud_ververica20220718-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      288 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   132115 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718/client.py
+-rw-r--r--   0 root         (0) root         (0)   212237 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2641 2024-05-24 17:09:03.000000 alibabacloud_ververica20220718-1.3.0/setup.py
```

### Comparing `alibabacloud_ververica20220718-1.2.1/LICENSE` & `alibabacloud_ververica20220718-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ververica20220718-1.2.1/PKG-INFO` & `alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_ververica20220718
-Version: 1.2.1
+Name: alibabacloud-ververica20220718
+Version: 1.3.0
 Summary: Alibaba Cloud ververica (20220718) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ververica-20220718/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_ververica20220718-1.2.1/README-CN.md` & `alibabacloud_ververica20220718-1.3.0/README-CN.md`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ververica-20220718/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_ververica20220718-1.2.1/README.md` & `alibabacloud_ververica20220718-1.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ververica-20220718/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718/client.py` & `alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,14 +44,22 @@
     def create_deployment_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateDeploymentRequest,
         headers: ververica_20220718_models.CreateDeploymentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.CreateDeploymentResponse:
+        """
+        @summary create a deployment
+        
+        @param request: CreateDeploymentRequest
+        @param headers: CreateDeploymentHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDeploymentResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -77,14 +85,22 @@
     async def create_deployment_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateDeploymentRequest,
         headers: ververica_20220718_models.CreateDeploymentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.CreateDeploymentResponse:
+        """
+        @summary create a deployment
+        
+        @param request: CreateDeploymentRequest
+        @param headers: CreateDeploymentHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDeploymentResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -108,34 +124,54 @@
         )
 
     def create_deployment(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateDeploymentRequest,
     ) -> ververica_20220718_models.CreateDeploymentResponse:
+        """
+        @summary create a deployment
+        
+        @param request: CreateDeploymentRequest
+        @return: CreateDeploymentResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.CreateDeploymentHeaders()
         return self.create_deployment_with_options(namespace, request, headers, runtime)
 
     async def create_deployment_async(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateDeploymentRequest,
     ) -> ververica_20220718_models.CreateDeploymentResponse:
+        """
+        @summary create a deployment
+        
+        @param request: CreateDeploymentRequest
+        @return: CreateDeploymentResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.CreateDeploymentHeaders()
         return await self.create_deployment_with_options_async(namespace, request, headers, runtime)
 
     def create_member_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateMemberRequest,
         headers: ververica_20220718_models.CreateMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.CreateMemberResponse:
+        """
+        @summary 调用CreateMember创建成员。
+        
+        @param request: CreateMemberRequest
+        @param headers: CreateMemberHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMemberResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -161,14 +197,22 @@
     async def create_member_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateMemberRequest,
         headers: ververica_20220718_models.CreateMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.CreateMemberResponse:
+        """
+        @summary 调用CreateMember创建成员。
+        
+        @param request: CreateMemberRequest
+        @param headers: CreateMemberHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMemberResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -192,34 +236,54 @@
         )
 
     def create_member(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateMemberRequest,
     ) -> ververica_20220718_models.CreateMemberResponse:
+        """
+        @summary 调用CreateMember创建成员。
+        
+        @param request: CreateMemberRequest
+        @return: CreateMemberResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.CreateMemberHeaders()
         return self.create_member_with_options(namespace, request, headers, runtime)
 
     async def create_member_async(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateMemberRequest,
     ) -> ververica_20220718_models.CreateMemberResponse:
+        """
+        @summary 调用CreateMember创建成员。
+        
+        @param request: CreateMemberRequest
+        @return: CreateMemberResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.CreateMemberHeaders()
         return await self.create_member_with_options_async(namespace, request, headers, runtime)
 
     def create_savepoint_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateSavepointRequest,
         headers: ververica_20220718_models.CreateSavepointHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.CreateSavepointResponse:
+        """
+        @summary 调用CreateSavepoint触发一次savepoint。
+        
+        @param request: CreateSavepointRequest
+        @param headers: CreateSavepointHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateSavepointResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.deployment_id):
             body['deploymentId'] = request.deployment_id
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.native_format):
@@ -252,14 +316,22 @@
     async def create_savepoint_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateSavepointRequest,
         headers: ververica_20220718_models.CreateSavepointHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.CreateSavepointResponse:
+        """
+        @summary 调用CreateSavepoint触发一次savepoint。
+        
+        @param request: CreateSavepointRequest
+        @param headers: CreateSavepointHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateSavepointResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.deployment_id):
             body['deploymentId'] = request.deployment_id
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.native_format):
@@ -290,34 +362,54 @@
         )
 
     def create_savepoint(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateSavepointRequest,
     ) -> ververica_20220718_models.CreateSavepointResponse:
+        """
+        @summary 调用CreateSavepoint触发一次savepoint。
+        
+        @param request: CreateSavepointRequest
+        @return: CreateSavepointResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.CreateSavepointHeaders()
         return self.create_savepoint_with_options(namespace, request, headers, runtime)
 
     async def create_savepoint_async(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateSavepointRequest,
     ) -> ververica_20220718_models.CreateSavepointResponse:
+        """
+        @summary 调用CreateSavepoint触发一次savepoint。
+        
+        @param request: CreateSavepointRequest
+        @return: CreateSavepointResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.CreateSavepointHeaders()
         return await self.create_savepoint_with_options_async(namespace, request, headers, runtime)
 
     def create_variable_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateVariableRequest,
         headers: ververica_20220718_models.CreateVariableHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.CreateVariableResponse:
+        """
+        @summary 调用CreateVariable创建变量。
+        
+        @param request: CreateVariableRequest
+        @param headers: CreateVariableHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateVariableResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -343,14 +435,22 @@
     async def create_variable_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateVariableRequest,
         headers: ververica_20220718_models.CreateVariableHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.CreateVariableResponse:
+        """
+        @summary 调用CreateVariable创建变量。
+        
+        @param request: CreateVariableRequest
+        @param headers: CreateVariableHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateVariableResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -374,34 +474,53 @@
         )
 
     def create_variable(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateVariableRequest,
     ) -> ververica_20220718_models.CreateVariableResponse:
+        """
+        @summary 调用CreateVariable创建变量。
+        
+        @param request: CreateVariableRequest
+        @return: CreateVariableResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.CreateVariableHeaders()
         return self.create_variable_with_options(namespace, request, headers, runtime)
 
     async def create_variable_async(
         self,
         namespace: str,
         request: ververica_20220718_models.CreateVariableRequest,
     ) -> ververica_20220718_models.CreateVariableResponse:
+        """
+        @summary 调用CreateVariable创建变量。
+        
+        @param request: CreateVariableRequest
+        @return: CreateVariableResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.CreateVariableHeaders()
         return await self.create_variable_with_options_async(namespace, request, headers, runtime)
 
     def delete_deployment_with_options(
         self,
         namespace: str,
         deployment_id: str,
         headers: ververica_20220718_models.DeleteDeploymentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteDeploymentResponse:
+        """
+        @summary delete deployment
+        
+        @param headers: DeleteDeploymentHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDeploymentResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -425,14 +544,21 @@
     async def delete_deployment_with_options_async(
         self,
         namespace: str,
         deployment_id: str,
         headers: ververica_20220718_models.DeleteDeploymentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteDeploymentResponse:
+        """
+        @summary delete deployment
+        
+        @param headers: DeleteDeploymentHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDeploymentResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -454,34 +580,51 @@
         )
 
     def delete_deployment(
         self,
         namespace: str,
         deployment_id: str,
     ) -> ververica_20220718_models.DeleteDeploymentResponse:
+        """
+        @summary delete deployment
+        
+        @return: DeleteDeploymentResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteDeploymentHeaders()
         return self.delete_deployment_with_options(namespace, deployment_id, headers, runtime)
 
     async def delete_deployment_async(
         self,
         namespace: str,
         deployment_id: str,
     ) -> ververica_20220718_models.DeleteDeploymentResponse:
+        """
+        @summary delete deployment
+        
+        @return: DeleteDeploymentResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteDeploymentHeaders()
         return await self.delete_deployment_with_options_async(namespace, deployment_id, headers, runtime)
 
     def delete_job_with_options(
         self,
         namespace: str,
         job_id: str,
         headers: ververica_20220718_models.DeleteJobHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteJobResponse:
+        """
+        @summary delete job
+        
+        @param headers: DeleteJobHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteJobResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -505,14 +648,21 @@
     async def delete_job_with_options_async(
         self,
         namespace: str,
         job_id: str,
         headers: ververica_20220718_models.DeleteJobHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteJobResponse:
+        """
+        @summary delete job
+        
+        @param headers: DeleteJobHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteJobResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -534,34 +684,51 @@
         )
 
     def delete_job(
         self,
         namespace: str,
         job_id: str,
     ) -> ververica_20220718_models.DeleteJobResponse:
+        """
+        @summary delete job
+        
+        @return: DeleteJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteJobHeaders()
         return self.delete_job_with_options(namespace, job_id, headers, runtime)
 
     async def delete_job_async(
         self,
         namespace: str,
         job_id: str,
     ) -> ververica_20220718_models.DeleteJobResponse:
+        """
+        @summary delete job
+        
+        @return: DeleteJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteJobHeaders()
         return await self.delete_job_with_options_async(namespace, job_id, headers, runtime)
 
     def delete_member_with_options(
         self,
         namespace: str,
         member: str,
         headers: ververica_20220718_models.DeleteMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteMemberResponse:
+        """
+        @summary 调用DeleteMember删除成员。
+        
+        @param headers: DeleteMemberHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMemberResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -585,14 +752,21 @@
     async def delete_member_with_options_async(
         self,
         namespace: str,
         member: str,
         headers: ververica_20220718_models.DeleteMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteMemberResponse:
+        """
+        @summary 调用DeleteMember删除成员。
+        
+        @param headers: DeleteMemberHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMemberResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -614,34 +788,51 @@
         )
 
     def delete_member(
         self,
         namespace: str,
         member: str,
     ) -> ververica_20220718_models.DeleteMemberResponse:
+        """
+        @summary 调用DeleteMember删除成员。
+        
+        @return: DeleteMemberResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteMemberHeaders()
         return self.delete_member_with_options(namespace, member, headers, runtime)
 
     async def delete_member_async(
         self,
         namespace: str,
         member: str,
     ) -> ververica_20220718_models.DeleteMemberResponse:
+        """
+        @summary 调用DeleteMember删除成员。
+        
+        @return: DeleteMemberResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteMemberHeaders()
         return await self.delete_member_with_options_async(namespace, member, headers, runtime)
 
     def delete_savepoint_with_options(
         self,
         namespace: str,
         savepoint_id: str,
         headers: ververica_20220718_models.DeleteSavepointHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteSavepointResponse:
+        """
+        @summary 调用DeleteSavepoint删除savepoint。
+        
+        @param headers: DeleteSavepointHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteSavepointResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -665,14 +856,21 @@
     async def delete_savepoint_with_options_async(
         self,
         namespace: str,
         savepoint_id: str,
         headers: ververica_20220718_models.DeleteSavepointHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteSavepointResponse:
+        """
+        @summary 调用DeleteSavepoint删除savepoint。
+        
+        @param headers: DeleteSavepointHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteSavepointResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -694,34 +892,51 @@
         )
 
     def delete_savepoint(
         self,
         namespace: str,
         savepoint_id: str,
     ) -> ververica_20220718_models.DeleteSavepointResponse:
+        """
+        @summary 调用DeleteSavepoint删除savepoint。
+        
+        @return: DeleteSavepointResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteSavepointHeaders()
         return self.delete_savepoint_with_options(namespace, savepoint_id, headers, runtime)
 
     async def delete_savepoint_async(
         self,
         namespace: str,
         savepoint_id: str,
     ) -> ververica_20220718_models.DeleteSavepointResponse:
+        """
+        @summary 调用DeleteSavepoint删除savepoint。
+        
+        @return: DeleteSavepointResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteSavepointHeaders()
         return await self.delete_savepoint_with_options_async(namespace, savepoint_id, headers, runtime)
 
     def delete_variable_with_options(
         self,
         namespace: str,
         name: str,
         headers: ververica_20220718_models.DeleteVariableHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteVariableResponse:
+        """
+        @summary deleta variable
+        
+        @param headers: DeleteVariableHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteVariableResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -745,14 +960,21 @@
     async def delete_variable_with_options_async(
         self,
         namespace: str,
         name: str,
         headers: ververica_20220718_models.DeleteVariableHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.DeleteVariableResponse:
+        """
+        @summary deleta variable
+        
+        @param headers: DeleteVariableHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteVariableResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -774,33 +996,51 @@
         )
 
     def delete_variable(
         self,
         namespace: str,
         name: str,
     ) -> ververica_20220718_models.DeleteVariableResponse:
+        """
+        @summary deleta variable
+        
+        @return: DeleteVariableResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteVariableHeaders()
         return self.delete_variable_with_options(namespace, name, headers, runtime)
 
     async def delete_variable_async(
         self,
         namespace: str,
         name: str,
     ) -> ververica_20220718_models.DeleteVariableResponse:
+        """
+        @summary deleta variable
+        
+        @return: DeleteVariableResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.DeleteVariableHeaders()
         return await self.delete_variable_with_options_async(namespace, name, headers, runtime)
 
     def flink_api_proxy_with_options(
         self,
         request: ververica_20220718_models.FlinkApiProxyRequest,
         headers: ververica_20220718_models.FlinkApiProxyHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.FlinkApiProxyResponse:
+        """
+        @summary 调用FlinkApiProxy代理Flink请求。
+        
+        @param request: FlinkApiProxyRequest
+        @param headers: FlinkApiProxyHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: FlinkApiProxyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.flink_api_path):
             query['flinkApiPath'] = request.flink_api_path
         if not UtilClient.is_unset(request.namespace):
             query['namespace'] = request.namespace
         if not UtilClient.is_unset(request.resource_id):
@@ -834,14 +1074,22 @@
 
     async def flink_api_proxy_with_options_async(
         self,
         request: ververica_20220718_models.FlinkApiProxyRequest,
         headers: ververica_20220718_models.FlinkApiProxyHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.FlinkApiProxyResponse:
+        """
+        @summary 调用FlinkApiProxy代理Flink请求。
+        
+        @param request: FlinkApiProxyRequest
+        @param headers: FlinkApiProxyHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: FlinkApiProxyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.flink_api_path):
             query['flinkApiPath'] = request.flink_api_path
         if not UtilClient.is_unset(request.namespace):
             query['namespace'] = request.namespace
         if not UtilClient.is_unset(request.resource_id):
@@ -873,34 +1121,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def flink_api_proxy(
         self,
         request: ververica_20220718_models.FlinkApiProxyRequest,
     ) -> ververica_20220718_models.FlinkApiProxyResponse:
+        """
+        @summary 调用FlinkApiProxy代理Flink请求。
+        
+        @param request: FlinkApiProxyRequest
+        @return: FlinkApiProxyResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.FlinkApiProxyHeaders()
         return self.flink_api_proxy_with_options(request, headers, runtime)
 
     async def flink_api_proxy_async(
         self,
         request: ververica_20220718_models.FlinkApiProxyRequest,
     ) -> ververica_20220718_models.FlinkApiProxyResponse:
+        """
+        @summary 调用FlinkApiProxy代理Flink请求。
+        
+        @param request: FlinkApiProxyRequest
+        @return: FlinkApiProxyResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.FlinkApiProxyHeaders()
         return await self.flink_api_proxy_with_options_async(request, headers, runtime)
 
     def generate_resource_plan_with_flink_conf_async_with_options(
         self,
         namespace: str,
         deployment_id: str,
         request: ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncRequest,
         headers: ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncResponse:
+        """
+        @summary generate resource plan with flink conf async.
+        
+        @param request: GenerateResourcePlanWithFlinkConfAsyncRequest
+        @param headers: GenerateResourcePlanWithFlinkConfAsyncHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateResourcePlanWithFlinkConfAsyncResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -927,14 +1195,22 @@
         self,
         namespace: str,
         deployment_id: str,
         request: ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncRequest,
         headers: ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncResponse:
+        """
+        @summary generate resource plan with flink conf async.
+        
+        @param request: GenerateResourcePlanWithFlinkConfAsyncRequest
+        @param headers: GenerateResourcePlanWithFlinkConfAsyncHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GenerateResourcePlanWithFlinkConfAsyncResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -959,35 +1235,54 @@
 
     def generate_resource_plan_with_flink_conf_async(
         self,
         namespace: str,
         deployment_id: str,
         request: ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncRequest,
     ) -> ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncResponse:
+        """
+        @summary generate resource plan with flink conf async.
+        
+        @param request: GenerateResourcePlanWithFlinkConfAsyncRequest
+        @return: GenerateResourcePlanWithFlinkConfAsyncResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncHeaders()
         return self.generate_resource_plan_with_flink_conf_async_with_options(namespace, deployment_id, request, headers, runtime)
 
     async def generate_resource_plan_with_flink_conf_async_async(
         self,
         namespace: str,
         deployment_id: str,
         request: ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncRequest,
     ) -> ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncResponse:
+        """
+        @summary generate resource plan with flink conf async.
+        
+        @param request: GenerateResourcePlanWithFlinkConfAsyncRequest
+        @return: GenerateResourcePlanWithFlinkConfAsyncResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GenerateResourcePlanWithFlinkConfAsyncHeaders()
         return await self.generate_resource_plan_with_flink_conf_async_with_options_async(namespace, deployment_id, request, headers, runtime)
 
     def get_deployment_with_options(
         self,
         namespace: str,
         deployment_id: str,
         headers: ververica_20220718_models.GetDeploymentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetDeploymentResponse:
+        """
+        @summary get a deployment
+        
+        @param headers: GetDeploymentHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDeploymentResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1011,14 +1306,21 @@
     async def get_deployment_with_options_async(
         self,
         namespace: str,
         deployment_id: str,
         headers: ververica_20220718_models.GetDeploymentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetDeploymentResponse:
+        """
+        @summary get a deployment
+        
+        @param headers: GetDeploymentHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDeploymentResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1040,34 +1342,51 @@
         )
 
     def get_deployment(
         self,
         namespace: str,
         deployment_id: str,
     ) -> ververica_20220718_models.GetDeploymentResponse:
+        """
+        @summary get a deployment
+        
+        @return: GetDeploymentResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetDeploymentHeaders()
         return self.get_deployment_with_options(namespace, deployment_id, headers, runtime)
 
     async def get_deployment_async(
         self,
         namespace: str,
         deployment_id: str,
     ) -> ververica_20220718_models.GetDeploymentResponse:
+        """
+        @summary get a deployment
+        
+        @return: GetDeploymentResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetDeploymentHeaders()
         return await self.get_deployment_with_options_async(namespace, deployment_id, headers, runtime)
 
     def get_generate_resource_plan_result_with_options(
         self,
         namespace: str,
         ticket_id: str,
         headers: ververica_20220718_models.GetGenerateResourcePlanResultHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetGenerateResourcePlanResultResponse:
+        """
+        @summary 获取生成ResourcePlan异步操作的结果。
+        
+        @param headers: GetGenerateResourcePlanResultHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetGenerateResourcePlanResultResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1091,14 +1410,21 @@
     async def get_generate_resource_plan_result_with_options_async(
         self,
         namespace: str,
         ticket_id: str,
         headers: ververica_20220718_models.GetGenerateResourcePlanResultHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetGenerateResourcePlanResultResponse:
+        """
+        @summary 获取生成ResourcePlan异步操作的结果。
+        
+        @param headers: GetGenerateResourcePlanResultHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetGenerateResourcePlanResultResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1120,34 +1446,51 @@
         )
 
     def get_generate_resource_plan_result(
         self,
         namespace: str,
         ticket_id: str,
     ) -> ververica_20220718_models.GetGenerateResourcePlanResultResponse:
+        """
+        @summary 获取生成ResourcePlan异步操作的结果。
+        
+        @return: GetGenerateResourcePlanResultResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetGenerateResourcePlanResultHeaders()
         return self.get_generate_resource_plan_result_with_options(namespace, ticket_id, headers, runtime)
 
     async def get_generate_resource_plan_result_async(
         self,
         namespace: str,
         ticket_id: str,
     ) -> ververica_20220718_models.GetGenerateResourcePlanResultResponse:
+        """
+        @summary 获取生成ResourcePlan异步操作的结果。
+        
+        @return: GetGenerateResourcePlanResultResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetGenerateResourcePlanResultHeaders()
         return await self.get_generate_resource_plan_result_with_options_async(namespace, ticket_id, headers, runtime)
 
     def get_job_with_options(
         self,
         namespace: str,
         job_id: str,
         headers: ververica_20220718_models.GetJobHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetJobResponse:
+        """
+        @summary get job
+        
+        @param headers: GetJobHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetJobResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1171,14 +1514,21 @@
     async def get_job_with_options_async(
         self,
         namespace: str,
         job_id: str,
         headers: ververica_20220718_models.GetJobHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetJobResponse:
+        """
+        @summary get job
+        
+        @param headers: GetJobHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetJobResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1200,34 +1550,51 @@
         )
 
     def get_job(
         self,
         namespace: str,
         job_id: str,
     ) -> ververica_20220718_models.GetJobResponse:
+        """
+        @summary get job
+        
+        @return: GetJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetJobHeaders()
         return self.get_job_with_options(namespace, job_id, headers, runtime)
 
     async def get_job_async(
         self,
         namespace: str,
         job_id: str,
     ) -> ververica_20220718_models.GetJobResponse:
+        """
+        @summary get job
+        
+        @return: GetJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetJobHeaders()
         return await self.get_job_with_options_async(namespace, job_id, headers, runtime)
 
     def get_member_with_options(
         self,
         namespace: str,
         member: str,
         headers: ververica_20220718_models.GetMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetMemberResponse:
+        """
+        @summary 调用GetMember获取成员。
+        
+        @param headers: GetMemberHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMemberResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1251,14 +1618,21 @@
     async def get_member_with_options_async(
         self,
         namespace: str,
         member: str,
         headers: ververica_20220718_models.GetMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetMemberResponse:
+        """
+        @summary 调用GetMember获取成员。
+        
+        @param headers: GetMemberHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMemberResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1280,34 +1654,51 @@
         )
 
     def get_member(
         self,
         namespace: str,
         member: str,
     ) -> ververica_20220718_models.GetMemberResponse:
+        """
+        @summary 调用GetMember获取成员。
+        
+        @return: GetMemberResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetMemberHeaders()
         return self.get_member_with_options(namespace, member, headers, runtime)
 
     async def get_member_async(
         self,
         namespace: str,
         member: str,
     ) -> ververica_20220718_models.GetMemberResponse:
+        """
+        @summary 调用GetMember获取成员。
+        
+        @return: GetMemberResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetMemberHeaders()
         return await self.get_member_with_options_async(namespace, member, headers, runtime)
 
     def get_savepoint_with_options(
         self,
         namespace: str,
         savepoint_id: str,
         headers: ververica_20220718_models.GetSavepointHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetSavepointResponse:
+        """
+        @summary 调用GetSavepoint获取savepoint信息。
+        
+        @param headers: GetSavepointHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSavepointResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1331,14 +1722,21 @@
     async def get_savepoint_with_options_async(
         self,
         namespace: str,
         savepoint_id: str,
         headers: ververica_20220718_models.GetSavepointHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.GetSavepointResponse:
+        """
+        @summary 调用GetSavepoint获取savepoint信息。
+        
+        @param headers: GetSavepointHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSavepointResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1360,34 +1758,52 @@
         )
 
     def get_savepoint(
         self,
         namespace: str,
         savepoint_id: str,
     ) -> ververica_20220718_models.GetSavepointResponse:
+        """
+        @summary 调用GetSavepoint获取savepoint信息。
+        
+        @return: GetSavepointResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetSavepointHeaders()
         return self.get_savepoint_with_options(namespace, savepoint_id, headers, runtime)
 
     async def get_savepoint_async(
         self,
         namespace: str,
         savepoint_id: str,
     ) -> ververica_20220718_models.GetSavepointResponse:
+        """
+        @summary 调用GetSavepoint获取savepoint信息。
+        
+        @return: GetSavepointResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.GetSavepointHeaders()
         return await self.get_savepoint_with_options_async(namespace, savepoint_id, headers, runtime)
 
     def list_deployment_targets_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.ListDeploymentTargetsRequest,
         headers: ververica_20220718_models.ListDeploymentTargetsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListDeploymentTargetsResponse:
+        """
+        @summary list deployment targets
+        
+        @param request: ListDeploymentTargetsRequest
+        @param headers: ListDeploymentTargetsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDeploymentTargetsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         real_headers = {}
@@ -1418,14 +1834,22 @@
     async def list_deployment_targets_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListDeploymentTargetsRequest,
         headers: ververica_20220718_models.ListDeploymentTargetsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListDeploymentTargetsResponse:
+        """
+        @summary list deployment targets
+        
+        @param request: ListDeploymentTargetsRequest
+        @param headers: ListDeploymentTargetsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDeploymentTargetsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         real_headers = {}
@@ -1454,44 +1878,74 @@
         )
 
     def list_deployment_targets(
         self,
         namespace: str,
         request: ververica_20220718_models.ListDeploymentTargetsRequest,
     ) -> ververica_20220718_models.ListDeploymentTargetsResponse:
+        """
+        @summary list deployment targets
+        
+        @param request: ListDeploymentTargetsRequest
+        @return: ListDeploymentTargetsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListDeploymentTargetsHeaders()
         return self.list_deployment_targets_with_options(namespace, request, headers, runtime)
 
     async def list_deployment_targets_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListDeploymentTargetsRequest,
     ) -> ververica_20220718_models.ListDeploymentTargetsResponse:
+        """
+        @summary list deployment targets
+        
+        @param request: ListDeploymentTargetsRequest
+        @return: ListDeploymentTargetsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListDeploymentTargetsHeaders()
         return await self.list_deployment_targets_with_options_async(namespace, request, headers, runtime)
 
     def list_deployments_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.ListDeploymentsRequest,
         headers: ververica_20220718_models.ListDeploymentsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListDeploymentsResponse:
+        """
+        @summary list deployments
+        
+        @param request: ListDeploymentsRequest
+        @param headers: ListDeploymentsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDeploymentsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.creator):
+            query['creator'] = request.creator
         if not UtilClient.is_unset(request.execution_mode):
             query['executionMode'] = request.execution_mode
+        if not UtilClient.is_unset(request.label_key):
+            query['labelKey'] = request.label_key
+        if not UtilClient.is_unset(request.label_value_array):
+            query['labelValueArray'] = request.label_value_array
+        if not UtilClient.is_unset(request.modifier):
+            query['modifier'] = request.modifier
         if not UtilClient.is_unset(request.name):
             query['name'] = request.name
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.status):
+            query['status'] = request.status
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -1516,24 +1970,42 @@
     async def list_deployments_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListDeploymentsRequest,
         headers: ververica_20220718_models.ListDeploymentsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListDeploymentsResponse:
+        """
+        @summary list deployments
+        
+        @param request: ListDeploymentsRequest
+        @param headers: ListDeploymentsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDeploymentsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.creator):
+            query['creator'] = request.creator
         if not UtilClient.is_unset(request.execution_mode):
             query['executionMode'] = request.execution_mode
+        if not UtilClient.is_unset(request.label_key):
+            query['labelKey'] = request.label_key
+        if not UtilClient.is_unset(request.label_value_array):
+            query['labelValueArray'] = request.label_value_array
+        if not UtilClient.is_unset(request.modifier):
+            query['modifier'] = request.modifier
         if not UtilClient.is_unset(request.name):
             query['name'] = request.name
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.status):
+            query['status'] = request.status
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -1556,32 +2028,171 @@
         )
 
     def list_deployments(
         self,
         namespace: str,
         request: ververica_20220718_models.ListDeploymentsRequest,
     ) -> ververica_20220718_models.ListDeploymentsResponse:
+        """
+        @summary list deployments
+        
+        @param request: ListDeploymentsRequest
+        @return: ListDeploymentsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListDeploymentsHeaders()
         return self.list_deployments_with_options(namespace, request, headers, runtime)
 
     async def list_deployments_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListDeploymentsRequest,
     ) -> ververica_20220718_models.ListDeploymentsResponse:
+        """
+        @summary list deployments
+        
+        @param request: ListDeploymentsRequest
+        @return: ListDeploymentsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListDeploymentsHeaders()
         return await self.list_deployments_with_options_async(namespace, request, headers, runtime)
 
+    def list_editable_namespace_with_options(
+        self,
+        request: ververica_20220718_models.ListEditableNamespaceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ververica_20220718_models.ListEditableNamespaceResponse:
+        """
+        @summary 列出有编辑权限的项目空间。
+        
+        @param request: ListEditableNamespaceRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListEditableNamespaceResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.namespace):
+            query['namespace'] = request.namespace
+        if not UtilClient.is_unset(request.page_index):
+            query['pageIndex'] = request.page_index
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        if not UtilClient.is_unset(request.workspace_id):
+            query['workspaceId'] = request.workspace_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListEditableNamespace',
+            version='2022-07-18',
+            protocol='HTTPS',
+            pathname=f'/gateway/v2/namespaces/editable',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ververica_20220718_models.ListEditableNamespaceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_editable_namespace_with_options_async(
+        self,
+        request: ververica_20220718_models.ListEditableNamespaceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ververica_20220718_models.ListEditableNamespaceResponse:
+        """
+        @summary 列出有编辑权限的项目空间。
+        
+        @param request: ListEditableNamespaceRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListEditableNamespaceResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.namespace):
+            query['namespace'] = request.namespace
+        if not UtilClient.is_unset(request.page_index):
+            query['pageIndex'] = request.page_index
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        if not UtilClient.is_unset(request.workspace_id):
+            query['workspaceId'] = request.workspace_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListEditableNamespace',
+            version='2022-07-18',
+            protocol='HTTPS',
+            pathname=f'/gateway/v2/namespaces/editable',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ververica_20220718_models.ListEditableNamespaceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_editable_namespace(
+        self,
+        request: ververica_20220718_models.ListEditableNamespaceRequest,
+    ) -> ververica_20220718_models.ListEditableNamespaceResponse:
+        """
+        @summary 列出有编辑权限的项目空间。
+        
+        @param request: ListEditableNamespaceRequest
+        @return: ListEditableNamespaceResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_editable_namespace_with_options(request, headers, runtime)
+
+    async def list_editable_namespace_async(
+        self,
+        request: ververica_20220718_models.ListEditableNamespaceRequest,
+    ) -> ververica_20220718_models.ListEditableNamespaceResponse:
+        """
+        @summary 列出有编辑权限的项目空间。
+        
+        @param request: ListEditableNamespaceRequest
+        @return: ListEditableNamespaceResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_editable_namespace_with_options_async(request, headers, runtime)
+
     def list_engine_version_metadata_with_options(
         self,
         headers: ververica_20220718_models.ListEngineVersionMetadataHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListEngineVersionMetadataResponse:
+        """
+        @summary 获取系统支持的引擎版本信息。
+        
+        @param headers: ListEngineVersionMetadataHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListEngineVersionMetadataResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1603,14 +2214,21 @@
         )
 
     async def list_engine_version_metadata_with_options_async(
         self,
         headers: ververica_20220718_models.ListEngineVersionMetadataHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListEngineVersionMetadataResponse:
+        """
+        @summary 获取系统支持的引擎版本信息。
+        
+        @param headers: ListEngineVersionMetadataHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListEngineVersionMetadataResponse
+        """
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers
@@ -1628,38 +2246,58 @@
         )
         return TeaCore.from_map(
             ververica_20220718_models.ListEngineVersionMetadataResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_engine_version_metadata(self) -> ververica_20220718_models.ListEngineVersionMetadataResponse:
+        """
+        @summary 获取系统支持的引擎版本信息。
+        
+        @return: ListEngineVersionMetadataResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListEngineVersionMetadataHeaders()
         return self.list_engine_version_metadata_with_options(headers, runtime)
 
     async def list_engine_version_metadata_async(self) -> ververica_20220718_models.ListEngineVersionMetadataResponse:
+        """
+        @summary 获取系统支持的引擎版本信息。
+        
+        @return: ListEngineVersionMetadataResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListEngineVersionMetadataHeaders()
         return await self.list_engine_version_metadata_with_options_async(headers, runtime)
 
     def list_jobs_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.ListJobsRequest,
         headers: ververica_20220718_models.ListJobsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListJobsResponse:
+        """
+        @summary list jobs
+        
+        @param request: ListJobsRequest
+        @param headers: ListJobsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.deployment_id):
             query['deploymentId'] = request.deployment_id
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.sort_name):
+            query['sortName'] = request.sort_name
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -1684,22 +2322,32 @@
     async def list_jobs_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListJobsRequest,
         headers: ververica_20220718_models.ListJobsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListJobsResponse:
+        """
+        @summary list jobs
+        
+        @param request: ListJobsRequest
+        @param headers: ListJobsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.deployment_id):
             query['deploymentId'] = request.deployment_id
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.sort_name):
+            query['sortName'] = request.sort_name
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -1722,34 +2370,54 @@
         )
 
     def list_jobs(
         self,
         namespace: str,
         request: ververica_20220718_models.ListJobsRequest,
     ) -> ververica_20220718_models.ListJobsResponse:
+        """
+        @summary list jobs
+        
+        @param request: ListJobsRequest
+        @return: ListJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListJobsHeaders()
         return self.list_jobs_with_options(namespace, request, headers, runtime)
 
     async def list_jobs_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListJobsRequest,
     ) -> ververica_20220718_models.ListJobsResponse:
+        """
+        @summary list jobs
+        
+        @param request: ListJobsRequest
+        @return: ListJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListJobsHeaders()
         return await self.list_jobs_with_options_async(namespace, request, headers, runtime)
 
     def list_members_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.ListMembersRequest,
         headers: ververica_20220718_models.ListMembersHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListMembersResponse:
+        """
+        @summary 调用ListMembers接口获取成员列表。
+        
+        @param request: ListMembersRequest
+        @param headers: ListMembersHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMembersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         real_headers = {}
@@ -1780,14 +2448,22 @@
     async def list_members_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListMembersRequest,
         headers: ververica_20220718_models.ListMembersHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListMembersResponse:
+        """
+        @summary 调用ListMembers接口获取成员列表。
+        
+        @param request: ListMembersRequest
+        @param headers: ListMembersHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMembersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         real_headers = {}
@@ -1816,34 +2492,54 @@
         )
 
     def list_members(
         self,
         namespace: str,
         request: ververica_20220718_models.ListMembersRequest,
     ) -> ververica_20220718_models.ListMembersResponse:
+        """
+        @summary 调用ListMembers接口获取成员列表。
+        
+        @param request: ListMembersRequest
+        @return: ListMembersResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListMembersHeaders()
         return self.list_members_with_options(namespace, request, headers, runtime)
 
     async def list_members_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListMembersRequest,
     ) -> ververica_20220718_models.ListMembersResponse:
+        """
+        @summary 调用ListMembers接口获取成员列表。
+        
+        @param request: ListMembersRequest
+        @return: ListMembersResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListMembersHeaders()
         return await self.list_members_with_options_async(namespace, request, headers, runtime)
 
     def list_savepoints_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.ListSavepointsRequest,
         headers: ververica_20220718_models.ListSavepointsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListSavepointsResponse:
+        """
+        @summary 调用ListSavepoints获取满足查询条件的savepoint列表。
+        
+        @param request: ListSavepointsRequest
+        @param headers: ListSavepointsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSavepointsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.deployment_id):
             query['deploymentId'] = request.deployment_id
         if not UtilClient.is_unset(request.job_id):
             query['jobId'] = request.job_id
         if not UtilClient.is_unset(request.page_index):
@@ -1878,14 +2574,22 @@
     async def list_savepoints_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListSavepointsRequest,
         headers: ververica_20220718_models.ListSavepointsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListSavepointsResponse:
+        """
+        @summary 调用ListSavepoints获取满足查询条件的savepoint列表。
+        
+        @param request: ListSavepointsRequest
+        @param headers: ListSavepointsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSavepointsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.deployment_id):
             query['deploymentId'] = request.deployment_id
         if not UtilClient.is_unset(request.job_id):
             query['jobId'] = request.job_id
         if not UtilClient.is_unset(request.page_index):
@@ -1918,34 +2622,54 @@
         )
 
     def list_savepoints(
         self,
         namespace: str,
         request: ververica_20220718_models.ListSavepointsRequest,
     ) -> ververica_20220718_models.ListSavepointsResponse:
+        """
+        @summary 调用ListSavepoints获取满足查询条件的savepoint列表。
+        
+        @param request: ListSavepointsRequest
+        @return: ListSavepointsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListSavepointsHeaders()
         return self.list_savepoints_with_options(namespace, request, headers, runtime)
 
     async def list_savepoints_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListSavepointsRequest,
     ) -> ververica_20220718_models.ListSavepointsResponse:
+        """
+        @summary 调用ListSavepoints获取满足查询条件的savepoint列表。
+        
+        @param request: ListSavepointsRequest
+        @return: ListSavepointsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListSavepointsHeaders()
         return await self.list_savepoints_with_options_async(namespace, request, headers, runtime)
 
     def list_variables_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.ListVariablesRequest,
         headers: ververica_20220718_models.ListVariablesHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListVariablesResponse:
+        """
+        @summary list variables
+        
+        @param request: ListVariablesRequest
+        @param headers: ListVariablesHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListVariablesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         real_headers = {}
@@ -1976,14 +2700,22 @@
     async def list_variables_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListVariablesRequest,
         headers: ververica_20220718_models.ListVariablesHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.ListVariablesResponse:
+        """
+        @summary list variables
+        
+        @param request: ListVariablesRequest
+        @param headers: ListVariablesHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListVariablesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_index):
             query['pageIndex'] = request.page_index
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         real_headers = {}
@@ -2012,36 +2744,50 @@
         )
 
     def list_variables(
         self,
         namespace: str,
         request: ververica_20220718_models.ListVariablesRequest,
     ) -> ververica_20220718_models.ListVariablesResponse:
+        """
+        @summary list variables
+        
+        @param request: ListVariablesRequest
+        @return: ListVariablesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListVariablesHeaders()
         return self.list_variables_with_options(namespace, request, headers, runtime)
 
     async def list_variables_async(
         self,
         namespace: str,
         request: ververica_20220718_models.ListVariablesRequest,
     ) -> ververica_20220718_models.ListVariablesResponse:
+        """
+        @summary list variables
+        
+        @param request: ListVariablesRequest
+        @return: ListVariablesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.ListVariablesHeaders()
         return await self.list_variables_with_options_async(namespace, request, headers, runtime)
 
     def start_job_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.StartJobRequest,
         headers: ververica_20220718_models.StartJobHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.StartJobResponse:
         """
-        @deprecated
+        @deprecated OpenAPI StartJob is deprecated
+        
+        @summary start job
         
         @param request: StartJobRequest
         @param headers: StartJobHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartJobResponse
         Deprecated
         """
@@ -2075,15 +2821,17 @@
         self,
         namespace: str,
         request: ververica_20220718_models.StartJobRequest,
         headers: ververica_20220718_models.StartJobHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.StartJobResponse:
         """
-        @deprecated
+        @deprecated OpenAPI StartJob is deprecated
+        
+        @summary start job
         
         @param request: StartJobRequest
         @param headers: StartJobHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartJobResponse
         Deprecated
         """
@@ -2115,15 +2863,17 @@
 
     def start_job(
         self,
         namespace: str,
         request: ververica_20220718_models.StartJobRequest,
     ) -> ververica_20220718_models.StartJobResponse:
         """
-        @deprecated
+        @deprecated OpenAPI StartJob is deprecated
+        
+        @summary start job
         
         @param request: StartJobRequest
         @return: StartJobResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.StartJobHeaders()
@@ -2131,15 +2881,17 @@
 
     async def start_job_async(
         self,
         namespace: str,
         request: ververica_20220718_models.StartJobRequest,
     ) -> ververica_20220718_models.StartJobResponse:
         """
-        @deprecated
+        @deprecated OpenAPI StartJob is deprecated
+        
+        @summary start job
         
         @param request: StartJobRequest
         @return: StartJobResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.StartJobHeaders()
@@ -2148,14 +2900,22 @@
     def start_job_with_params_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.StartJobWithParamsRequest,
         headers: ververica_20220718_models.StartJobWithParamsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.StartJobWithParamsResponse:
+        """
+        @summary 启动作业实例。
+        
+        @param request: StartJobWithParamsRequest
+        @param headers: StartJobWithParamsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartJobWithParamsResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -2181,14 +2941,22 @@
     async def start_job_with_params_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.StartJobWithParamsRequest,
         headers: ververica_20220718_models.StartJobWithParamsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.StartJobWithParamsResponse:
+        """
+        @summary 启动作业实例。
+        
+        @param request: StartJobWithParamsRequest
+        @param headers: StartJobWithParamsHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartJobWithParamsResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -2212,35 +2980,55 @@
         )
 
     def start_job_with_params(
         self,
         namespace: str,
         request: ververica_20220718_models.StartJobWithParamsRequest,
     ) -> ververica_20220718_models.StartJobWithParamsResponse:
+        """
+        @summary 启动作业实例。
+        
+        @param request: StartJobWithParamsRequest
+        @return: StartJobWithParamsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.StartJobWithParamsHeaders()
         return self.start_job_with_params_with_options(namespace, request, headers, runtime)
 
     async def start_job_with_params_async(
         self,
         namespace: str,
         request: ververica_20220718_models.StartJobWithParamsRequest,
     ) -> ververica_20220718_models.StartJobWithParamsResponse:
+        """
+        @summary 启动作业实例。
+        
+        @param request: StartJobWithParamsRequest
+        @return: StartJobWithParamsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.StartJobWithParamsHeaders()
         return await self.start_job_with_params_with_options_async(namespace, request, headers, runtime)
 
     def stop_job_with_options(
         self,
         namespace: str,
         job_id: str,
         request: ververica_20220718_models.StopJobRequest,
         headers: ververica_20220718_models.StopJobHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.StopJobResponse:
+        """
+        @summary 调用StopJob停止实例。
+        
+        @param request: StopJobRequest
+        @param headers: StopJobHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopJobResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -2267,14 +3055,22 @@
         self,
         namespace: str,
         job_id: str,
         request: ververica_20220718_models.StopJobRequest,
         headers: ververica_20220718_models.StopJobHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.StopJobResponse:
+        """
+        @summary 调用StopJob停止实例。
+        
+        @param request: StopJobRequest
+        @param headers: StopJobHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopJobResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -2299,36 +3095,56 @@
 
     def stop_job(
         self,
         namespace: str,
         job_id: str,
         request: ververica_20220718_models.StopJobRequest,
     ) -> ververica_20220718_models.StopJobResponse:
+        """
+        @summary 调用StopJob停止实例。
+        
+        @param request: StopJobRequest
+        @return: StopJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.StopJobHeaders()
         return self.stop_job_with_options(namespace, job_id, request, headers, runtime)
 
     async def stop_job_async(
         self,
         namespace: str,
         job_id: str,
         request: ververica_20220718_models.StopJobRequest,
     ) -> ververica_20220718_models.StopJobResponse:
+        """
+        @summary 调用StopJob停止实例。
+        
+        @param request: StopJobRequest
+        @return: StopJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.StopJobHeaders()
         return await self.stop_job_with_options_async(namespace, job_id, request, headers, runtime)
 
     def update_deployment_with_options(
         self,
         namespace: str,
         deployment_id: str,
         request: ververica_20220718_models.UpdateDeploymentRequest,
         headers: ververica_20220718_models.UpdateDeploymentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.UpdateDeploymentResponse:
+        """
+        @summary update a deployment using patch
+        
+        @param request: UpdateDeploymentRequest
+        @param headers: UpdateDeploymentHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateDeploymentResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -2355,14 +3171,22 @@
         self,
         namespace: str,
         deployment_id: str,
         request: ververica_20220718_models.UpdateDeploymentRequest,
         headers: ververica_20220718_models.UpdateDeploymentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.UpdateDeploymentResponse:
+        """
+        @summary update a deployment using patch
+        
+        @param request: UpdateDeploymentRequest
+        @param headers: UpdateDeploymentHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateDeploymentResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -2387,35 +3211,55 @@
 
     def update_deployment(
         self,
         namespace: str,
         deployment_id: str,
         request: ververica_20220718_models.UpdateDeploymentRequest,
     ) -> ververica_20220718_models.UpdateDeploymentResponse:
+        """
+        @summary update a deployment using patch
+        
+        @param request: UpdateDeploymentRequest
+        @return: UpdateDeploymentResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.UpdateDeploymentHeaders()
         return self.update_deployment_with_options(namespace, deployment_id, request, headers, runtime)
 
     async def update_deployment_async(
         self,
         namespace: str,
         deployment_id: str,
         request: ververica_20220718_models.UpdateDeploymentRequest,
     ) -> ververica_20220718_models.UpdateDeploymentResponse:
+        """
+        @summary update a deployment using patch
+        
+        @param request: UpdateDeploymentRequest
+        @return: UpdateDeploymentResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.UpdateDeploymentHeaders()
         return await self.update_deployment_with_options_async(namespace, deployment_id, request, headers, runtime)
 
     def update_member_with_options(
         self,
         namespace: str,
         request: ververica_20220718_models.UpdateMemberRequest,
         headers: ververica_20220718_models.UpdateMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.UpdateMemberResponse:
+        """
+        @summary 调用UpdateMember更新成员。
+        
+        @param request: UpdateMemberRequest
+        @param headers: UpdateMemberHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateMemberResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -2441,14 +3285,22 @@
     async def update_member_with_options_async(
         self,
         namespace: str,
         request: ververica_20220718_models.UpdateMemberRequest,
         headers: ververica_20220718_models.UpdateMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ververica_20220718_models.UpdateMemberResponse:
+        """
+        @summary 调用UpdateMember更新成员。
+        
+        @param request: UpdateMemberRequest
+        @param headers: UpdateMemberHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateMemberResponse
+        """
         UtilClient.validate_model(request)
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.workspace):
             real_headers['workspace'] = UtilClient.to_jsonstring(headers.workspace)
         req = open_api_models.OpenApiRequest(
@@ -2472,19 +3324,31 @@
         )
 
     def update_member(
         self,
         namespace: str,
         request: ververica_20220718_models.UpdateMemberRequest,
     ) -> ververica_20220718_models.UpdateMemberResponse:
+        """
+        @summary 调用UpdateMember更新成员。
+        
+        @param request: UpdateMemberRequest
+        @return: UpdateMemberResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.UpdateMemberHeaders()
         return self.update_member_with_options(namespace, request, headers, runtime)
 
     async def update_member_async(
         self,
         namespace: str,
         request: ververica_20220718_models.UpdateMemberRequest,
     ) -> ververica_20220718_models.UpdateMemberResponse:
+        """
+        @summary 调用UpdateMember更新成员。
+        
+        @param request: UpdateMemberRequest
+        @return: UpdateMemberResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = ververica_20220718_models.UpdateMemberHeaders()
         return await self.update_member_with_options_async(namespace, request, headers, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718/models.py` & `alibabacloud_ververica20220718-1.3.0/alibabacloud_ververica20220718/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -552,14 +552,47 @@
         if m.get('running') is not None:
             self.running = m.get('running')
         if m.get('starting') is not None:
             self.starting = m.get('starting')
         return self
 
 
+class LocalVariable(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        value: str = None,
+    ):
+        self.name = name
+        self.value = value
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
+        if self.name is not None:
+            result['name'] = self.name
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
 class Log4jLogger(TeaModel):
     def __init__(
         self,
         logger_level: str = None,
         logger_name: str = None,
     ):
         self.logger_level = logger_level
@@ -679,59 +712,71 @@
 
 
 class Deployment(TeaModel):
     def __init__(
         self,
         artifact: Artifact = None,
         batch_resource_setting: BatchResourceSetting = None,
+        created_at: str = None,
         creator: str = None,
         creator_name: str = None,
         deployment_has_changed: bool = None,
         deployment_id: str = None,
         deployment_target: BriefDeploymentTarget = None,
         description: str = None,
         engine_version: str = None,
         execution_mode: str = None,
         flink_conf: Dict[str, Any] = None,
         job_summary: JobSummary = None,
+        local_variables: List[LocalVariable] = None,
         logging: Logging = None,
+        modified_at: str = None,
         modifier: str = None,
         modifier_name: str = None,
         name: str = None,
         namespace: str = None,
         streaming_resource_setting: StreamingResourceSetting = None,
+        workspace: str = None,
     ):
         self.artifact = artifact
         self.batch_resource_setting = batch_resource_setting
+        self.created_at = created_at
         self.creator = creator
         self.creator_name = creator_name
         self.deployment_has_changed = deployment_has_changed
         self.deployment_id = deployment_id
         self.deployment_target = deployment_target
         self.description = description
         self.engine_version = engine_version
         self.execution_mode = execution_mode
         self.flink_conf = flink_conf
         self.job_summary = job_summary
+        self.local_variables = local_variables
         self.logging = logging
+        self.modified_at = modified_at
         self.modifier = modifier
         self.modifier_name = modifier_name
         self.name = name
         self.namespace = namespace
         self.streaming_resource_setting = streaming_resource_setting
+        self.workspace = workspace
 
     def validate(self):
         if self.artifact:
             self.artifact.validate()
         if self.batch_resource_setting:
             self.batch_resource_setting.validate()
         if self.deployment_target:
             self.deployment_target.validate()
         if self.job_summary:
             self.job_summary.validate()
+        if self.local_variables:
+            for k in self.local_variables:
+                if k:
+                    k.validate()
         if self.logging:
             self.logging.validate()
         if self.streaming_resource_setting:
             self.streaming_resource_setting.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -739,14 +784,16 @@
             return _map
 
         result = dict()
         if self.artifact is not None:
             result['artifact'] = self.artifact.to_map()
         if self.batch_resource_setting is not None:
             result['batchResourceSetting'] = self.batch_resource_setting.to_map()
+        if self.created_at is not None:
+            result['createdAt'] = self.created_at
         if self.creator is not None:
             result['creator'] = self.creator
         if self.creator_name is not None:
             result['creatorName'] = self.creator_name
         if self.deployment_has_changed is not None:
             result['deploymentHasChanged'] = self.deployment_has_changed
         if self.deployment_id is not None:
@@ -759,36 +806,46 @@
             result['engineVersion'] = self.engine_version
         if self.execution_mode is not None:
             result['executionMode'] = self.execution_mode
         if self.flink_conf is not None:
             result['flinkConf'] = self.flink_conf
         if self.job_summary is not None:
             result['jobSummary'] = self.job_summary.to_map()
+        result['localVariables'] = []
+        if self.local_variables is not None:
+            for k in self.local_variables:
+                result['localVariables'].append(k.to_map() if k else None)
         if self.logging is not None:
             result['logging'] = self.logging.to_map()
+        if self.modified_at is not None:
+            result['modifiedAt'] = self.modified_at
         if self.modifier is not None:
             result['modifier'] = self.modifier
         if self.modifier_name is not None:
             result['modifierName'] = self.modifier_name
         if self.name is not None:
             result['name'] = self.name
         if self.namespace is not None:
             result['namespace'] = self.namespace
         if self.streaming_resource_setting is not None:
             result['streamingResourceSetting'] = self.streaming_resource_setting.to_map()
+        if self.workspace is not None:
+            result['workspace'] = self.workspace
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('artifact') is not None:
             temp_model = Artifact()
             self.artifact = temp_model.from_map(m['artifact'])
         if m.get('batchResourceSetting') is not None:
             temp_model = BatchResourceSetting()
             self.batch_resource_setting = temp_model.from_map(m['batchResourceSetting'])
+        if m.get('createdAt') is not None:
+            self.created_at = m.get('createdAt')
         if m.get('creator') is not None:
             self.creator = m.get('creator')
         if m.get('creatorName') is not None:
             self.creator_name = m.get('creatorName')
         if m.get('deploymentHasChanged') is not None:
             self.deployment_has_changed = m.get('deploymentHasChanged')
         if m.get('deploymentId') is not None:
@@ -803,28 +860,37 @@
         if m.get('executionMode') is not None:
             self.execution_mode = m.get('executionMode')
         if m.get('flinkConf') is not None:
             self.flink_conf = m.get('flinkConf')
         if m.get('jobSummary') is not None:
             temp_model = JobSummary()
             self.job_summary = temp_model.from_map(m['jobSummary'])
+        self.local_variables = []
+        if m.get('localVariables') is not None:
+            for k in m.get('localVariables'):
+                temp_model = LocalVariable()
+                self.local_variables.append(temp_model.from_map(k))
         if m.get('logging') is not None:
             temp_model = Logging()
             self.logging = temp_model.from_map(m['logging'])
+        if m.get('modifiedAt') is not None:
+            self.modified_at = m.get('modifiedAt')
         if m.get('modifier') is not None:
             self.modifier = m.get('modifier')
         if m.get('modifierName') is not None:
             self.modifier_name = m.get('modifierName')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('namespace') is not None:
             self.namespace = m.get('namespace')
         if m.get('streamingResourceSetting') is not None:
             temp_model = StreamingResourceSetting()
             self.streaming_resource_setting = temp_model.from_map(m['streamingResourceSetting'])
+        if m.get('workspace') is not None:
+            self.workspace = m.get('workspace')
         return self
 
 
 class DeploymentRestoreStrategy(TeaModel):
     def __init__(
         self,
         allow_non_restored_state: bool = None,
@@ -898,14 +964,53 @@
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('namespace') is not None:
             self.namespace = m.get('namespace')
         return self
 
 
+class EditableNamespace(TeaModel):
+    def __init__(
+        self,
+        namespace: str = None,
+        role: str = None,
+        workspace_id: str = None,
+    ):
+        self.namespace = namespace
+        self.role = role
+        self.workspace_id = workspace_id
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
+        if self.namespace is not None:
+            result['Namespace'] = self.namespace
+        if self.role is not None:
+            result['Role'] = self.role
+        if self.workspace_id is not None:
+            result['WorkspaceId'] = self.workspace_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        if m.get('Role') is not None:
+            self.role = m.get('Role')
+        if m.get('WorkspaceId') is not None:
+            self.workspace_id = m.get('WorkspaceId')
+        return self
+
+
 class EngineVersionSupportedFeatures(TeaModel):
     def __init__(
         self,
         support_native_savepoint: bool = None,
         use_for_sql_deployments: bool = None,
     ):
         self.support_native_savepoint = support_native_savepoint
@@ -938,16 +1043,18 @@
 class EngineVersionMetadata(TeaModel):
     def __init__(
         self,
         engine_version: str = None,
         features: EngineVersionSupportedFeatures = None,
         status: str = None,
     ):
+        # This parameter is required.
         self.engine_version = engine_version
         self.features = features
+        # This parameter is required.
         self.status = status
 
     def validate(self):
         if self.features:
             self.features.validate()
 
     def to_map(self):
@@ -1013,14 +1120,71 @@
         if m.get('engineVersionMetadata') is not None:
             for k in m.get('engineVersionMetadata'):
                 temp_model = EngineVersionMetadata()
                 self.engine_version_metadata.append(temp_model.from_map(k))
         return self
 
 
+class ErrorDetails(TeaModel):
+    def __init__(
+        self,
+        column_number: str = None,
+        end_column_number: str = None,
+        end_line_number: str = None,
+        invalidflink_conf: List[str] = None,
+        line_number: str = None,
+        message: str = None,
+    ):
+        self.column_number = column_number
+        self.end_column_number = end_column_number
+        self.end_line_number = end_line_number
+        self.invalidflink_conf = invalidflink_conf
+        self.line_number = line_number
+        self.message = message
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
+        if self.column_number is not None:
+            result['columnNumber'] = self.column_number
+        if self.end_column_number is not None:
+            result['endColumnNumber'] = self.end_column_number
+        if self.end_line_number is not None:
+            result['endLineNumber'] = self.end_line_number
+        if self.invalidflink_conf is not None:
+            result['invalidflinkConf'] = self.invalidflink_conf
+        if self.line_number is not None:
+            result['lineNumber'] = self.line_number
+        if self.message is not None:
+            result['message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('columnNumber') is not None:
+            self.column_number = m.get('columnNumber')
+        if m.get('endColumnNumber') is not None:
+            self.end_column_number = m.get('endColumnNumber')
+        if m.get('endLineNumber') is not None:
+            self.end_line_number = m.get('endLineNumber')
+        if m.get('invalidflinkConf') is not None:
+            self.invalidflink_conf = m.get('invalidflinkConf')
+        if m.get('lineNumber') is not None:
+            self.line_number = m.get('lineNumber')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        return self
+
+
 class JobMetric(TeaModel):
     def __init__(
         self,
         total_cpu: float = None,
         total_memory_byte: int = None,
     ):
         self.total_cpu = total_cpu
@@ -1167,63 +1331,75 @@
 
 
 class Job(TeaModel):
     def __init__(
         self,
         artifact: Artifact = None,
         batch_resource_setting: BatchResourceSetting = None,
+        created_at: str = None,
         creator: str = None,
         creator_name: str = None,
         deployment_id: str = None,
         deployment_name: str = None,
         end_time: int = None,
         engine_version: str = None,
         execution_mode: str = None,
         flink_conf: Dict[str, Any] = None,
         job_id: str = None,
+        local_variables: List[LocalVariable] = None,
         logging: Logging = None,
         metric: JobMetric = None,
+        modified_at: str = None,
         modifier: str = None,
         modifier_name: str = None,
         namespace: str = None,
         restore_strategy: DeploymentRestoreStrategy = None,
         session_cluster_name: str = None,
         start_time: int = None,
         status: JobStatus = None,
         streaming_resource_setting: StreamingResourceSetting = None,
         user_flink_conf: Dict[str, Any] = None,
+        workspace: str = None,
     ):
         self.artifact = artifact
         self.batch_resource_setting = batch_resource_setting
+        self.created_at = created_at
         self.creator = creator
         self.creator_name = creator_name
         self.deployment_id = deployment_id
         self.deployment_name = deployment_name
         self.end_time = end_time
         self.engine_version = engine_version
         self.execution_mode = execution_mode
         self.flink_conf = flink_conf
         self.job_id = job_id
+        self.local_variables = local_variables
         self.logging = logging
         self.metric = metric
+        self.modified_at = modified_at
         self.modifier = modifier
         self.modifier_name = modifier_name
         self.namespace = namespace
         self.restore_strategy = restore_strategy
         self.session_cluster_name = session_cluster_name
         self.start_time = start_time
         self.status = status
         self.streaming_resource_setting = streaming_resource_setting
         self.user_flink_conf = user_flink_conf
+        self.workspace = workspace
 
     def validate(self):
         if self.artifact:
             self.artifact.validate()
         if self.batch_resource_setting:
             self.batch_resource_setting.validate()
+        if self.local_variables:
+            for k in self.local_variables:
+                if k:
+                    k.validate()
         if self.logging:
             self.logging.validate()
         if self.metric:
             self.metric.validate()
         if self.restore_strategy:
             self.restore_strategy.validate()
         if self.status:
@@ -1237,14 +1413,16 @@
             return _map
 
         result = dict()
         if self.artifact is not None:
             result['artifact'] = self.artifact.to_map()
         if self.batch_resource_setting is not None:
             result['batchResourceSetting'] = self.batch_resource_setting.to_map()
+        if self.created_at is not None:
+            result['createdAt'] = self.created_at
         if self.creator is not None:
             result['creator'] = self.creator
         if self.creator_name is not None:
             result['creatorName'] = self.creator_name
         if self.deployment_id is not None:
             result['deploymentId'] = self.deployment_id
         if self.deployment_name is not None:
@@ -1255,18 +1433,24 @@
             result['engineVersion'] = self.engine_version
         if self.execution_mode is not None:
             result['executionMode'] = self.execution_mode
         if self.flink_conf is not None:
             result['flinkConf'] = self.flink_conf
         if self.job_id is not None:
             result['jobId'] = self.job_id
+        result['localVariables'] = []
+        if self.local_variables is not None:
+            for k in self.local_variables:
+                result['localVariables'].append(k.to_map() if k else None)
         if self.logging is not None:
             result['logging'] = self.logging.to_map()
         if self.metric is not None:
             result['metric'] = self.metric.to_map()
+        if self.modified_at is not None:
+            result['modifiedAt'] = self.modified_at
         if self.modifier is not None:
             result['modifier'] = self.modifier
         if self.modifier_name is not None:
             result['modifierName'] = self.modifier_name
         if self.namespace is not None:
             result['namespace'] = self.namespace
         if self.restore_strategy is not None:
@@ -1277,24 +1461,28 @@
             result['startTime'] = self.start_time
         if self.status is not None:
             result['status'] = self.status.to_map()
         if self.streaming_resource_setting is not None:
             result['streamingResourceSetting'] = self.streaming_resource_setting.to_map()
         if self.user_flink_conf is not None:
             result['userFlinkConf'] = self.user_flink_conf
+        if self.workspace is not None:
+            result['workspace'] = self.workspace
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('artifact') is not None:
             temp_model = Artifact()
             self.artifact = temp_model.from_map(m['artifact'])
         if m.get('batchResourceSetting') is not None:
             temp_model = BatchResourceSetting()
             self.batch_resource_setting = temp_model.from_map(m['batchResourceSetting'])
+        if m.get('createdAt') is not None:
+            self.created_at = m.get('createdAt')
         if m.get('creator') is not None:
             self.creator = m.get('creator')
         if m.get('creatorName') is not None:
             self.creator_name = m.get('creatorName')
         if m.get('deploymentId') is not None:
             self.deployment_id = m.get('deploymentId')
         if m.get('deploymentName') is not None:
@@ -1305,20 +1493,27 @@
             self.engine_version = m.get('engineVersion')
         if m.get('executionMode') is not None:
             self.execution_mode = m.get('executionMode')
         if m.get('flinkConf') is not None:
             self.flink_conf = m.get('flinkConf')
         if m.get('jobId') is not None:
             self.job_id = m.get('jobId')
+        self.local_variables = []
+        if m.get('localVariables') is not None:
+            for k in m.get('localVariables'):
+                temp_model = LocalVariable()
+                self.local_variables.append(temp_model.from_map(k))
         if m.get('logging') is not None:
             temp_model = Logging()
             self.logging = temp_model.from_map(m['logging'])
         if m.get('metric') is not None:
             temp_model = JobMetric()
             self.metric = temp_model.from_map(m['metric'])
+        if m.get('modifiedAt') is not None:
+            self.modified_at = m.get('modifiedAt')
         if m.get('modifier') is not None:
             self.modifier = m.get('modifier')
         if m.get('modifierName') is not None:
             self.modifier_name = m.get('modifierName')
         if m.get('namespace') is not None:
             self.namespace = m.get('namespace')
         if m.get('restoreStrategy') is not None:
@@ -1332,64 +1527,82 @@
             temp_model = JobStatus()
             self.status = temp_model.from_map(m['status'])
         if m.get('streamingResourceSetting') is not None:
             temp_model = StreamingResourceSetting()
             self.streaming_resource_setting = temp_model.from_map(m['streamingResourceSetting'])
         if m.get('userFlinkConf') is not None:
             self.user_flink_conf = m.get('userFlinkConf')
+        if m.get('workspace') is not None:
+            self.workspace = m.get('workspace')
         return self
 
 
 class JobStartParameters(TeaModel):
     def __init__(
         self,
         deployment_id: str = None,
+        local_variables: List[LocalVariable] = None,
         resource_queue_name: str = None,
         restore_strategy: DeploymentRestoreStrategy = None,
     ):
         self.deployment_id = deployment_id
+        self.local_variables = local_variables
         self.resource_queue_name = resource_queue_name
         self.restore_strategy = restore_strategy
 
     def validate(self):
+        if self.local_variables:
+            for k in self.local_variables:
+                if k:
+                    k.validate()
         if self.restore_strategy:
             self.restore_strategy.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.deployment_id is not None:
             result['deploymentId'] = self.deployment_id
+        result['localVariables'] = []
+        if self.local_variables is not None:
+            for k in self.local_variables:
+                result['localVariables'].append(k.to_map() if k else None)
         if self.resource_queue_name is not None:
             result['resourceQueueName'] = self.resource_queue_name
         if self.restore_strategy is not None:
             result['restoreStrategy'] = self.restore_strategy.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('deploymentId') is not None:
             self.deployment_id = m.get('deploymentId')
+        self.local_variables = []
+        if m.get('localVariables') is not None:
+            for k in m.get('localVariables'):
+                temp_model = LocalVariable()
+                self.local_variables.append(temp_model.from_map(k))
         if m.get('resourceQueueName') is not None:
             self.resource_queue_name = m.get('resourceQueueName')
         if m.get('restoreStrategy') is not None:
             temp_model = DeploymentRestoreStrategy()
             self.restore_strategy = temp_model.from_map(m['restoreStrategy'])
         return self
 
 
 class Member(TeaModel):
     def __init__(
         self,
         member: str = None,
         role: str = None,
     ):
+        # This parameter is required.
         self.member = member
         self.role = role
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1578,14 +1791,126 @@
             temp_model = SavepointStatus()
             self.status = temp_model.from_map(m['status'])
         if m.get('stopWithDrainEnabled') is not None:
             self.stop_with_drain_enabled = m.get('stopWithDrainEnabled')
         return self
 
 
+class SqlStatementValidationResult(TeaModel):
+    def __init__(
+        self,
+        error_details: ErrorDetails = None,
+        message: str = None,
+        success: bool = None,
+        validation_result: str = None,
+    ):
+        self.error_details = error_details
+        self.message = message
+        self.success = success
+        self.validation_result = validation_result
+
+    def validate(self):
+        if self.error_details:
+            self.error_details.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_details is not None:
+            result['errorDetails'] = self.error_details.to_map()
+        if self.message is not None:
+            result['message'] = self.message
+        if self.success is not None:
+            result['success'] = self.success
+        if self.validation_result is not None:
+            result['validationResult'] = self.validation_result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('errorDetails') is not None:
+            temp_model = ErrorDetails()
+            self.error_details = temp_model.from_map(m['errorDetails'])
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('validationResult') is not None:
+            self.validation_result = m.get('validationResult')
+        return self
+
+
+class SqlStatementWithContext(TeaModel):
+    def __init__(
+        self,
+        additional_dependencies: List[str] = None,
+        batch_mode: bool = None,
+        catalog: str = None,
+        database: str = None,
+        flink_configuration: Dict[str, Any] = None,
+        statement: str = None,
+        version_name: str = None,
+    ):
+        self.additional_dependencies = additional_dependencies
+        # This parameter is required.
+        self.batch_mode = batch_mode
+        self.catalog = catalog
+        self.database = database
+        self.flink_configuration = flink_configuration
+        # This parameter is required.
+        self.statement = statement
+        self.version_name = version_name
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
+        if self.additional_dependencies is not None:
+            result['additionalDependencies'] = self.additional_dependencies
+        if self.batch_mode is not None:
+            result['batchMode'] = self.batch_mode
+        if self.catalog is not None:
+            result['catalog'] = self.catalog
+        if self.database is not None:
+            result['database'] = self.database
+        if self.flink_configuration is not None:
+            result['flinkConfiguration'] = self.flink_configuration
+        if self.statement is not None:
+            result['statement'] = self.statement
+        if self.version_name is not None:
+            result['versionName'] = self.version_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('additionalDependencies') is not None:
+            self.additional_dependencies = m.get('additionalDependencies')
+        if m.get('batchMode') is not None:
+            self.batch_mode = m.get('batchMode')
+        if m.get('catalog') is not None:
+            self.catalog = m.get('catalog')
+        if m.get('database') is not None:
+            self.database = m.get('database')
+        if m.get('flinkConfiguration') is not None:
+            self.flink_configuration = m.get('flinkConfiguration')
+        if m.get('statement') is not None:
+            self.statement = m.get('statement')
+        if m.get('versionName') is not None:
+            self.version_name = m.get('versionName')
+        return self
+
+
 class StartJobRequestBody(TeaModel):
     def __init__(
         self,
         deployment_id: str = None,
         resource_setting_spec: BriefResourceSetting = None,
         restore_strategy: DeploymentRestoreStrategy = None,
     ):
@@ -1627,14 +1952,15 @@
 
 
 class StopJobRequestBody(TeaModel):
     def __init__(
         self,
         stop_strategy: str = None,
     ):
+        # This parameter is required.
         self.stop_strategy = stop_strategy
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1658,16 +1984,19 @@
         self,
         description: str = None,
         kind: str = None,
         name: str = None,
         value: str = None,
     ):
         self.description = description
+        # This parameter is required.
         self.kind = kind
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1701,14 +2030,15 @@
 class CreateDeploymentHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1732,14 +2062,15 @@
 
 
 class CreateDeploymentRequest(TeaModel):
     def __init__(
         self,
         body: Deployment = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -1827,17 +2158,14 @@
         body: CreateDeploymentResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1866,14 +2194,15 @@
 class CreateMemberHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1992,17 +2321,14 @@
         body: CreateMemberResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2031,14 +2357,15 @@
 class CreateSavepointHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2064,14 +2391,15 @@
 class CreateSavepointRequest(TeaModel):
     def __init__(
         self,
         deployment_id: str = None,
         description: str = None,
         native_format: bool = None,
     ):
+        # This parameter is required.
         self.deployment_id = deployment_id
         self.description = description
         self.native_format = native_format
 
     def validate(self):
         pass
 
@@ -2167,17 +2495,14 @@
         body: CreateSavepointResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2206,14 +2531,15 @@
 class CreateVariableHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2237,14 +2563,15 @@
 
 
 class CreateVariableRequest(TeaModel):
     def __init__(
         self,
         body: Variable = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -2332,17 +2659,14 @@
         body: CreateVariableResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2371,14 +2695,15 @@
 class DeleteDeploymentHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2460,17 +2785,14 @@
         body: DeleteDeploymentResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2499,14 +2821,15 @@
 class DeleteJobHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2588,17 +2911,14 @@
         body: DeleteJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2627,14 +2947,15 @@
 class DeleteMemberHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2716,17 +3037,14 @@
         body: DeleteMemberResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2755,14 +3073,15 @@
 class DeleteSavepointHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2844,17 +3163,14 @@
         body: DeleteSavepointResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2883,14 +3199,15 @@
 class DeleteVariableHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2972,17 +3289,14 @@
         body: DeleteVariableResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3011,14 +3325,15 @@
 class FlinkApiProxyHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3045,17 +3360,21 @@
     def __init__(
         self,
         flink_api_path: str = None,
         namespace: str = None,
         resource_id: str = None,
         resource_type: str = None,
     ):
+        # This parameter is required.
         self.flink_api_path = flink_api_path
+        # This parameter is required.
         self.namespace = namespace
+        # This parameter is required.
         self.resource_id = resource_id
+        # This parameter is required.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3151,17 +3470,14 @@
         body: FlinkApiProxyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3190,14 +3506,15 @@
 class GenerateResourcePlanWithFlinkConfAsyncHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3341,17 +3658,14 @@
         body: GenerateResourcePlanWithFlinkConfAsyncResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3380,14 +3694,15 @@
 class GetDeploymentHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3477,17 +3792,14 @@
         body: GetDeploymentResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3516,14 +3828,15 @@
 class GetGenerateResourcePlanResultHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3613,17 +3926,14 @@
         body: GetGenerateResourcePlanResultResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3652,14 +3962,15 @@
 class GetJobHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3749,17 +4060,14 @@
         body: GetJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3788,14 +4096,15 @@
 class GetMemberHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3885,17 +4194,14 @@
         body: GetMemberResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3924,14 +4230,15 @@
 class GetSavepointHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4021,17 +4328,14 @@
         body: GetSavepointResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4060,14 +4364,15 @@
 class ListDeploymentTargetsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4214,17 +4519,14 @@
         body: ListDeploymentTargetsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4253,14 +4555,15 @@
 class ListDeploymentsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4282,53 +4585,83 @@
             self.workspace = m.get('workspace')
         return self
 
 
 class ListDeploymentsRequest(TeaModel):
     def __init__(
         self,
+        creator: str = None,
         execution_mode: str = None,
+        label_key: str = None,
+        label_value_array: str = None,
+        modifier: str = None,
         name: str = None,
         page_index: int = None,
         page_size: int = None,
+        status: str = None,
     ):
+        self.creator = creator
         self.execution_mode = execution_mode
+        self.label_key = label_key
+        self.label_value_array = label_value_array
+        self.modifier = modifier
         self.name = name
         self.page_index = page_index
         self.page_size = page_size
+        self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.creator is not None:
+            result['creator'] = self.creator
         if self.execution_mode is not None:
             result['executionMode'] = self.execution_mode
+        if self.label_key is not None:
+            result['labelKey'] = self.label_key
+        if self.label_value_array is not None:
+            result['labelValueArray'] = self.label_value_array
+        if self.modifier is not None:
+            result['modifier'] = self.modifier
         if self.name is not None:
             result['name'] = self.name
         if self.page_index is not None:
             result['pageIndex'] = self.page_index
         if self.page_size is not None:
             result['pageSize'] = self.page_size
+        if self.status is not None:
+            result['status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('creator') is not None:
+            self.creator = m.get('creator')
         if m.get('executionMode') is not None:
             self.execution_mode = m.get('executionMode')
+        if m.get('labelKey') is not None:
+            self.label_key = m.get('labelKey')
+        if m.get('labelValueArray') is not None:
+            self.label_value_array = m.get('labelValueArray')
+        if m.get('modifier') is not None:
+            self.modifier = m.get('modifier')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('pageIndex') is not None:
             self.page_index = m.get('pageIndex')
         if m.get('pageSize') is not None:
             self.page_size = m.get('pageSize')
+        if m.get('status') is not None:
+            self.status = m.get('status')
         return self
 
 
 class ListDeploymentsResponseBody(TeaModel):
     def __init__(
         self,
         data: List[Deployment] = None,
@@ -4419,17 +4752,14 @@
         body: ListDeploymentsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4451,21 +4781,227 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListDeploymentsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListEditableNamespaceRequest(TeaModel):
+    def __init__(
+        self,
+        namespace: str = None,
+        page_index: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        workspace_id: str = None,
+    ):
+        self.namespace = namespace
+        self.page_index = page_index
+        self.page_size = page_size
+        # This parameter is required.
+        self.region_id = region_id
+        self.workspace_id = workspace_id
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
+        if self.namespace is not None:
+            result['namespace'] = self.namespace
+        if self.page_index is not None:
+            result['pageIndex'] = self.page_index
+        if self.page_size is not None:
+            result['pageSize'] = self.page_size
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.workspace_id is not None:
+            result['workspaceId'] = self.workspace_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('namespace') is not None:
+            self.namespace = m.get('namespace')
+        if m.get('pageIndex') is not None:
+            self.page_index = m.get('pageIndex')
+        if m.get('pageSize') is not None:
+            self.page_size = m.get('pageSize')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('workspaceId') is not None:
+            self.workspace_id = m.get('workspaceId')
+        return self
+
+
+class ListEditableNamespaceResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        editable_namespaces: List[EditableNamespace] = None,
+        page_index: str = None,
+        page_size: str = None,
+        total: str = None,
+    ):
+        self.editable_namespaces = editable_namespaces
+        self.page_index = page_index
+        self.page_size = page_size
+        self.total = total
+
+    def validate(self):
+        if self.editable_namespaces:
+            for k in self.editable_namespaces:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['editableNamespaces'] = []
+        if self.editable_namespaces is not None:
+            for k in self.editable_namespaces:
+                result['editableNamespaces'].append(k.to_map() if k else None)
+        if self.page_index is not None:
+            result['pageIndex'] = self.page_index
+        if self.page_size is not None:
+            result['pageSize'] = self.page_size
+        if self.total is not None:
+            result['total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.editable_namespaces = []
+        if m.get('editableNamespaces') is not None:
+            for k in m.get('editableNamespaces'):
+                temp_model = EditableNamespace()
+                self.editable_namespaces.append(temp_model.from_map(k))
+        if m.get('pageIndex') is not None:
+            self.page_index = m.get('pageIndex')
+        if m.get('pageSize') is not None:
+            self.page_size = m.get('pageSize')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        return self
+
+
+class ListEditableNamespaceResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: ListEditableNamespaceResponseBodyData = None,
+        http_code: int = None,
+        message: str = None,
+        reason: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.data = data
+        self.http_code = http_code
+        self.message = message
+        self.reason = reason
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        if self.http_code is not None:
+            result['httpCode'] = self.http_code
+        if self.message is not None:
+            result['message'] = self.message
+        if self.reason is not None:
+            result['reason'] = self.reason
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('data') is not None:
+            temp_model = ListEditableNamespaceResponseBodyData()
+            self.data = temp_model.from_map(m['data'])
+        if m.get('httpCode') is not None:
+            self.http_code = m.get('httpCode')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        if m.get('reason') is not None:
+            self.reason = m.get('reason')
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class ListEditableNamespaceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListEditableNamespaceResponseBody = None,
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
+            temp_model = ListEditableNamespaceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListEngineVersionMetadataHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4555,17 +5091,14 @@
         body: ListEngineVersionMetadataResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4594,14 +5127,15 @@
 class ListJobsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4626,18 +5160,21 @@
 
 class ListJobsRequest(TeaModel):
     def __init__(
         self,
         deployment_id: str = None,
         page_index: int = None,
         page_size: int = None,
+        sort_name: str = None,
     ):
+        # This parameter is required.
         self.deployment_id = deployment_id
         self.page_index = page_index
         self.page_size = page_size
+        self.sort_name = sort_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -4646,24 +5183,28 @@
         result = dict()
         if self.deployment_id is not None:
             result['deploymentId'] = self.deployment_id
         if self.page_index is not None:
             result['pageIndex'] = self.page_index
         if self.page_size is not None:
             result['pageSize'] = self.page_size
+        if self.sort_name is not None:
+            result['sortName'] = self.sort_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('deploymentId') is not None:
             self.deployment_id = m.get('deploymentId')
         if m.get('pageIndex') is not None:
             self.page_index = m.get('pageIndex')
         if m.get('pageSize') is not None:
             self.page_size = m.get('pageSize')
+        if m.get('sortName') is not None:
+            self.sort_name = m.get('sortName')
         return self
 
 
 class ListJobsResponseBody(TeaModel):
     def __init__(
         self,
         data: List[Job] = None,
@@ -4754,17 +5295,14 @@
         body: ListJobsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4793,14 +5331,15 @@
 class ListMembersHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4947,17 +5486,14 @@
         body: ListMembersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4986,14 +5522,15 @@
 class ListSavepointsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5152,17 +5689,14 @@
         body: ListSavepointsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5191,14 +5725,15 @@
 class ListVariablesHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5345,17 +5880,14 @@
         body: ListVariablesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5384,14 +5916,15 @@
 class StartJobHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5415,14 +5948,15 @@
 
 
 class StartJobRequest(TeaModel):
     def __init__(
         self,
         body: StartJobRequestBody = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -5510,17 +6044,14 @@
         body: StartJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5549,14 +6080,15 @@
 class StartJobWithParamsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5675,17 +6207,14 @@
         body: StartJobWithParamsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5714,14 +6243,15 @@
 class StopJobHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5745,14 +6275,15 @@
 
 
 class StopJobRequest(TeaModel):
     def __init__(
         self,
         body: StopJobRequestBody = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -5840,17 +6371,14 @@
         body: StopJobResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5879,14 +6407,15 @@
 class UpdateDeploymentHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5910,14 +6439,15 @@
 
 
 class UpdateDeploymentRequest(TeaModel):
     def __init__(
         self,
         body: Deployment = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -6005,17 +6535,14 @@
         body: UpdateDeploymentResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6044,14 +6571,15 @@
 class UpdateMemberHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         workspace: str = None,
     ):
         self.common_headers = common_headers
+        # This parameter is required.
         self.workspace = workspace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6170,17 +6698,14 @@
         body: UpdateMemberResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_ververica20220718-1.2.1/alibabacloud_ververica20220718.egg-info/PKG-INFO` & `alibabacloud_ververica20220718-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-ververica20220718
-Version: 1.2.1
+Name: alibabacloud_ververica20220718
+Version: 1.3.0
 Summary: Alibaba Cloud ververica (20220718) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ververica-20220718/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_ververica20220718-1.2.1/setup.py` & `alibabacloud_ververica20220718-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ververica20220718.
 
-Created on 13/11/2023
+Created on 24/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ververica20220718"
 NAME = "alibabacloud_ververica20220718" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ververica (20220718) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```


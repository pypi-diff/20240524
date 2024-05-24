# Comparing `tmp/qcloud-python-sts-3.1.5.tar.gz` & `tmp/qcloud-python-sts-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qcloud-python-sts-3.1.5.tar", last modified: Wed Jun 14 02:38:33 2023, max compression
+gzip compressed data, was "dist/qcloud-python-sts-3.1.6.tar", last modified: Fri May 24 05:17:35 2024, max compression
```

## Comparing `qcloud-python-sts-3.1.5.tar` & `qcloud-python-sts-3.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3856 2023-06-13 09:39:11.000000 qcloud-python-sts-3.1.5/README.md
--rw-r--r--   0 root         (0) root         (0)     4151 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-13 09:39:11.000000 qcloud-python-sts-3.1.5/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/sts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 09:39:11.000000 qcloud-python-sts-3.1.5/sts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12155 2023-06-13 09:39:11.000000 qcloud-python-sts-3.1.5/sts/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/qcloud_python_sts.egg-info/
--rw-r--r--   0 root         (0) root         (0)      261 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/qcloud_python_sts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     4151 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/qcloud_python_sts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/qcloud_python_sts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/qcloud_python_sts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-14 02:38:33.000000 qcloud-python-sts-3.1.5/qcloud_python_sts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      566 2023-06-14 02:36:27.000000 qcloud-python-sts-3.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-13 09:39:11.000000 qcloud-python-sts-3.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4922 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3856 2023-06-13 09:39:11.000000 qcloud-python-sts-3.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/qcloud_python_sts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4922 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/qcloud_python_sts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/qcloud_python_sts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/qcloud_python_sts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/qcloud_python_sts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/qcloud_python_sts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2024-05-24 05:15:02.000000 qcloud-python-sts-3.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 05:17:35.000000 qcloud-python-sts-3.1.6/sts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 09:39:11.000000 qcloud-python-sts-3.1.6/sts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14099 2024-05-24 05:15:02.000000 qcloud-python-sts-3.1.6/sts/sts.py
```

### Comparing `qcloud-python-sts-3.1.5/README.md` & `qcloud-python-sts-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `qcloud-python-sts-3.1.5/PKG-INFO` & `qcloud-python-sts-3.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,106 @@
 Metadata-Version: 2.1
 Name: qcloud-python-sts
-Version: 3.1.5
+Version: 3.1.6
 Summary: this is sts for python on v3
 Home-page: https://github.com/tencentyun/qcloud-cos-sts-sdk
 Author: qcloudterminal
 Author-email: qcloudterminal@gmail.com
 License: MIT
+Description: ## 获取 SDK
+        
+        ```
+        pip install -U qcloud-python-sts
+        ```
+        
+        ## 调用示例
+        
+        请查看 [demo](https://github.com/tencentyun/qcloud-cos-sts-sdk/tree/master/python/demo) 里的示例。
+        
+        ## 接口说明
+        
+        ### get_credential
+        
+        获取临时密钥接口
+        
+        ### 参数说明
+        
+        |字段|类型|描述|
+        | ---- | ---- | ---- |
+        |secret_id|String| 云 API 密钥 Id|
+        |secret_key|String| 云 API 密钥 key|
+        |duration_seconds|long| 要申请的临时密钥最长有效时间，单位秒，默认 1800，最大可设置 7200 |
+        |bucket|String| 存储桶名称：bucketName-appid, 如 test-125000000|
+        |region|String| 存储桶所属地域，如 ap-guangzhou|
+        |allow_prefix|list|资源的前缀，可以根据自己网站的用户登录态判断允许上传的具体路径，例子： a.jpg 或者 a/* 或者 * (使用通配符*存在重大安全风险, 请谨慎评估使用)|
+        |allow_actions|list| 授予 COS API 权限集合, 如简单上传操作：name/cos:PutObject|
+        |policy|dict| 策略：由 allow_actions、bucket、allow_prefix字段组成的描述授权的具体信息|
+        
+        ### 返回值说明
+        
+        |字段|类型|描述|
+        | ---- | ---- | ---- |
+        |credentials | dict | 临时密钥信息 |
+        |tmpSecretId | String | 临时密钥 Id，可用于计算签名 |
+        |tmpSecretKey | String | 临时密钥 Key，可用于计算签名 |
+        |sessionToken | String | 请求时需要用的 token 字符串，最终请求 COS API 时，需要放在 Header 的 x-cos-security-token 字段 |
+        |startTime | String | 密钥的起始时间，是 UNIX 时间戳 |
+        |expiredTime | String | 密钥的失效时间，是 UNIX 时间戳 |
+        
+        ### 返回结果
+        
+        成功的话，可以拿到包含密钥的 JSON 文本：
+        
+        ```json
+        {
+            "credentials": {
+                "tmpSecretId": "AKIDEPMQB_Q9Jt2fJxXyIekOzKZzx-sdGQgBga4TzsUdTWL9xlvsjInOHhCYFqfoKOY4",
+                "tmpSecretKey": "W/3Lbl1YEW02mCoawIesl5kNehSskrSbp1cT1tgW70g=",
+                "sessionToken": "c6xnSYAxyFbX8Y50627y9AA79u6Qfucw6924760b61588b79fea4c277b01ba157UVdr_10Y30bdpYtO8CXedYZe3KKZ_DyzaPiSFfNAcbr2MTfAgwJe-dhYhfyLMkeCqWyTNF-rOdOb0rp4Gto7p4yQAKuIPhQhuDd77gcAyGakC2WXHVd6ZuVaYIXBizZxqIHAf4lPiLHa6SZejSQfa_p5Ip2U1cAdkEionKbrX97xTKTcA_5Pu525CFSzHZIQibc2uNMZ-IRdQp12MaXZB6bxM6nB4xXH45mDIlbIGjaAsrtRJJ3csmf82uBKaJrYQoguAjBepMH91WcH87LlW9Ya3emNfVX7NMRRf64riYd_vomGF0TLgan9smEKAOdtaL94IkLvVJdhLqpvjBjp_4JCdqwlFAixaTzGJHdJzpGWOh0mQ6jDegAWgRYTrJvc5caYTz7Vphl8XoX5wHKKESUn_vqyTAid32t0vNYE034FIelxYT6VXuetYD_mvPfbHVDIXaFt7e_O8hRLkFwrdAIVaUml1mRPvccv2qOWSXs"
+            },
+            "expiration": "2019-08-07T08:54:35Z",
+            "startTime": 1565166275,
+            "expiredTime": 1565168075
+        }
+        ```
+        
+        ### get_policy
+        
+        获取策略(policy)接口。本接口适用于接收 Web、iOS、Android 客户端 SDK 提供的 Scope 参数。推荐您把 Scope 参数放在请求的 Body 里面，通过 POST 方式传到后台。
+        
+        ### 参数说明
+        
+        |字段|类型|描述|
+        | ---- | ---- | ---- |
+        |bucket|String| 存储桶名称：bucketName-appid, 如 test-125000000|
+        |region|String| 存储桶所属地域，如 ap-guangzhou|
+        |resource_prefix|String|资源的前缀，可以根据自己网站的用户登录态判断允许上传的具体路径，例子： a.jpg 或者 a/* 或者 * (使用通配符*存在重大安全风险, 请谨慎评估使用) |
+        |action|String| 授予 COS API 权限，, 如简单上传操作：name/cos:PutObject|
+        |scope|Scope| 构造policy的信息：由 action、bucket、region、sourcePrefix组成|
+        
+        ### 返回值说明
+        |字段|类型|描述|
+        | ---- | ---- | ---- |
+        |policy | dict | 申请临时密钥所需的权限策略 |
+        
+        
+        ### 返回结果
+        ```json
+        {
+        "version":"2.0",
+        "statement":[
+        	{
+        		"action":["name/cos:PutObject"],
+        		"effect":"allow",
+        		"resource":["qcs::cos:ap-guangzhou:uid/1250000000:example-1250000000/1.txt"]
+        	},
+        	{
+        		"action":["name/cos:GetObject" ],
+        		"effect":"allow",
+        		"resource":["qcs::cos:ap-guangzhou:uid/1250000000:example-1250000000/dir/exampleobject" ]
+        	}
+        ]
+        }
+        ```
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-
-## 获取 SDK
-
-```
-pip install -U qcloud-python-sts
-```
-
-## 调用示例
-
-请查看 [demo](https://github.com/tencentyun/qcloud-cos-sts-sdk/tree/master/python/demo) 里的示例。
-
-## 接口说明
-
-### get_credential
-
-获取临时密钥接口
-
-### 参数说明
-
-|字段|类型|描述|
-| ---- | ---- | ---- |
-|secret_id|String| 云 API 密钥 Id|
-|secret_key|String| 云 API 密钥 key|
-|duration_seconds|long| 要申请的临时密钥最长有效时间，单位秒，默认 1800，最大可设置 7200 |
-|bucket|String| 存储桶名称：bucketName-appid, 如 test-125000000|
-|region|String| 存储桶所属地域，如 ap-guangzhou|
-|allow_prefix|list|资源的前缀，可以根据自己网站的用户登录态判断允许上传的具体路径，例子： a.jpg 或者 a/* 或者 * (使用通配符*存在重大安全风险, 请谨慎评估使用)|
-|allow_actions|list| 授予 COS API 权限集合, 如简单上传操作：name/cos:PutObject|
-|policy|dict| 策略：由 allow_actions、bucket、allow_prefix字段组成的描述授权的具体信息|
-
-### 返回值说明
-
-|字段|类型|描述|
-| ---- | ---- | ---- |
-|credentials | dict | 临时密钥信息 |
-|tmpSecretId | String | 临时密钥 Id，可用于计算签名 |
-|tmpSecretKey | String | 临时密钥 Key，可用于计算签名 |
-|sessionToken | String | 请求时需要用的 token 字符串，最终请求 COS API 时，需要放在 Header 的 x-cos-security-token 字段 |
-|startTime | String | 密钥的起始时间，是 UNIX 时间戳 |
-|expiredTime | String | 密钥的失效时间，是 UNIX 时间戳 |
-
-### 返回结果
-
-成功的话，可以拿到包含密钥的 JSON 文本：
-
-```json
-{
-    "credentials": {
-        "tmpSecretId": "AKIDEPMQB_Q9Jt2fJxXyIekOzKZzx-sdGQgBga4TzsUdTWL9xlvsjInOHhCYFqfoKOY4",
-        "tmpSecretKey": "W/3Lbl1YEW02mCoawIesl5kNehSskrSbp1cT1tgW70g=",
-        "sessionToken": "c6xnSYAxyFbX8Y50627y9AA79u6Qfucw6924760b61588b79fea4c277b01ba157UVdr_10Y30bdpYtO8CXedYZe3KKZ_DyzaPiSFfNAcbr2MTfAgwJe-dhYhfyLMkeCqWyTNF-rOdOb0rp4Gto7p4yQAKuIPhQhuDd77gcAyGakC2WXHVd6ZuVaYIXBizZxqIHAf4lPiLHa6SZejSQfa_p5Ip2U1cAdkEionKbrX97xTKTcA_5Pu525CFSzHZIQibc2uNMZ-IRdQp12MaXZB6bxM6nB4xXH45mDIlbIGjaAsrtRJJ3csmf82uBKaJrYQoguAjBepMH91WcH87LlW9Ya3emNfVX7NMRRf64riYd_vomGF0TLgan9smEKAOdtaL94IkLvVJdhLqpvjBjp_4JCdqwlFAixaTzGJHdJzpGWOh0mQ6jDegAWgRYTrJvc5caYTz7Vphl8XoX5wHKKESUn_vqyTAid32t0vNYE034FIelxYT6VXuetYD_mvPfbHVDIXaFt7e_O8hRLkFwrdAIVaUml1mRPvccv2qOWSXs"
-    },
-    "expiration": "2019-08-07T08:54:35Z",
-    "startTime": 1565166275,
-    "expiredTime": 1565168075
-}
-```
-
-### get_policy
-
-获取策略(policy)接口。本接口适用于接收 Web、iOS、Android 客户端 SDK 提供的 Scope 参数。推荐您把 Scope 参数放在请求的 Body 里面，通过 POST 方式传到后台。
-
-### 参数说明
-
-|字段|类型|描述|
-| ---- | ---- | ---- |
-|bucket|String| 存储桶名称：bucketName-appid, 如 test-125000000|
-|region|String| 存储桶所属地域，如 ap-guangzhou|
-|resource_prefix|String|资源的前缀，可以根据自己网站的用户登录态判断允许上传的具体路径，例子： a.jpg 或者 a/* 或者 * (使用通配符*存在重大安全风险, 请谨慎评估使用) |
-|action|String| 授予 COS API 权限，, 如简单上传操作：name/cos:PutObject|
-|scope|Scope| 构造policy的信息：由 action、bucket、region、sourcePrefix组成|
-
-### 返回值说明
-|字段|类型|描述|
-| ---- | ---- | ---- |
-|policy | dict | 申请临时密钥所需的权限策略 |
-
-
-### 返回结果
-```json
-{
-"version":"2.0",
-"statement":[
-	{
-		"action":["name/cos:PutObject"],
-		"effect":"allow",
-		"resource":["qcs::cos:ap-guangzhou:uid/1250000000:example-1250000000/1.txt"]
-	},
-	{
-		"action":["name/cos:GetObject" ],
-		"effect":"allow",
-		"resource":["qcs::cos:ap-guangzhou:uid/1250000000:example-1250000000/dir/exampleobject" ]
-	}
-]
-}
-```
-
-
```

### Comparing `qcloud-python-sts-3.1.5/sts/sts.py` & `qcloud-python-sts-3.1.6/sts/sts.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     resource = None
     allow_actions = None
     condition = None
     policy = None
     network_proxy = None
     url = sts_url
     domain = sts_domain
+    service_type = 'cos'
 
     def __init__(self, config={}):
         self.parse_parameters(config)
 
     def parse_parameters(self, config):
         if not isinstance(config, dict):
             raise ValueError("Error: config is not dict")
@@ -87,17 +88,38 @@
                 raise ValueError('Error: bucket is invalid: ' + self.bucket)
             appid = str(self.bucket[(split_index + 1):]).strip()
 
             self.resource = list()
             for prefix in resource_prefix:
                 if not str(prefix).startswith('/'):
                     prefix = '/' + prefix
-                self.resource.append("qcs::cos:{region}:uid/{appid}:{bucket}{prefix}".format(region=self.region,
+                if self.service_type == 'cos':
+                    self.resource.append("qcs::{service_type}:{region}:uid/{appid}:{bucket}{prefix}".format(service_type=self.service_type, region=self.region,
                                                                                     appid=appid, bucket=self.bucket,
                                                                                     prefix=prefix))
+                elif self.service_type == 'ci':
+                    self.resource.append("qcs::{service_type}:{region}:uid/{appid}:bucket/{bucket}{prefix}".format(service_type=self.service_type, region=self.region,
+                                                                                                              appid=appid, bucket=self.bucket,
+                                                                                                              prefix=prefix))
+
+    def add_resource(self, resource):
+        """
+        追加需要的资源，仅当 self.policy 字段未设置时有效
+        :param resource: 需要追加的资源，支持str与list两种类型
+        """
+        if self.policy is not None:
+            return
+        if self.resource is None:
+            self.resource = list()
+        if isinstance(resource, str):
+            self.resource.append(resource)
+        elif isinstance(resource, list):
+            self.resource.extend(resource)
+        else:
+            raise ValueError('Error: param type is invalid, type:' + str(type(resource)))
 
     @staticmethod
     def get_policy(scopes=[]):
         if not isinstance(scopes, list):
             return None
         policy = dict()
         policy['version'] = '2.0'
@@ -251,14 +273,19 @@
                 bc_json['sessionToken'] = v
             else:
                 bc_json[k[0].lower() + k[1:]] = v
         
         return bc_json
 
 
+class CISts(Sts):
+    service_type = 'ci'
+    pass
+
+
 class Tools(object):
 
     @staticmethod
     def _flat_key_values(a):
         return a[0] + '=' + str(a[1])
 
     @staticmethod
@@ -274,14 +301,15 @@
 class Scope(object):
     action = None
     bucket = None
     region = None
     resource_prefix = None
     condition = None
     effect = 'allow'
+    service_type = 'cos'
 
     def __init__(self, action=None, bucket=None, region=None, resource_prefix=None):
         self.action = action
         self.bucket = bucket
         self.region = region
         self.resource_prefix = resource_prefix
 
@@ -323,17 +351,22 @@
         
         resource = list()
         if isinstance(self.resource_prefix, str):
             self.resource_prefix = [self.resource_prefix]
         for i in range(len(self.resource_prefix)):
             if not str(self.resource_prefix[i]).startswith('/'):
                 self.resource_prefix[i] = '/' + self.resource_prefix[i]
-            resource.append("qcs::cos:{region}:uid/{appid}:{bucket}{prefix}".format(region=self.region,
-                                                                                appid=appid, bucket=self.bucket,
-                                                                                prefix=self.resource_prefix[i]))
+                if self.service_type == 'cos':
+                    resource.append("qcs::{service_type}:{region}:uid/{appid}:{bucket}{prefix}".format(service_type=self.service_type, region=self.region,
+                                                                                        appid=appid, bucket=self.bucket,
+                                                                                        prefix=self.resource_prefix[i]))
+                elif self.service_type == 'ci':
+                    resource.append("qcs::{service_type}:{region}:uid/{appid}:bucket/{bucket}{prefix}".format(service_type=self.service_type, region=self.region,
+                                                                                                       appid=appid, bucket=self.bucket,
+                                                                                                       prefix=self.resource_prefix[i]))
         return resource
 
     def get_effect(self):
         return self.effect
     
     def get_condition(self):
         return self.condition
@@ -344,7 +377,12 @@
         result['bucket'] = self.bucket
         result['region'] = self.region
         result['prefix'] = self.resource_prefix
         result['effect'] = self.effect
         result['condition'] = self.condition
         return result
 
+
+class CIScope(Scope):
+    service_type = 'ci'
+    pass
+
```

### Comparing `qcloud-python-sts-3.1.5/qcloud_python_sts.egg-info/PKG-INFO` & `qcloud-python-sts-3.1.6/qcloud_python_sts.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,106 @@
 Metadata-Version: 2.1
 Name: qcloud-python-sts
-Version: 3.1.5
+Version: 3.1.6
 Summary: this is sts for python on v3
 Home-page: https://github.com/tencentyun/qcloud-cos-sts-sdk
 Author: qcloudterminal
 Author-email: qcloudterminal@gmail.com
 License: MIT
+Description: ## 获取 SDK
+        
+        ```
+        pip install -U qcloud-python-sts
+        ```
+        
+        ## 调用示例
+        
+        请查看 [demo](https://github.com/tencentyun/qcloud-cos-sts-sdk/tree/master/python/demo) 里的示例。
+        
+        ## 接口说明
+        
+        ### get_credential
+        
+        获取临时密钥接口
+        
+        ### 参数说明
+        
+        |字段|类型|描述|
+        | ---- | ---- | ---- |
+        |secret_id|String| 云 API 密钥 Id|
+        |secret_key|String| 云 API 密钥 key|
+        |duration_seconds|long| 要申请的临时密钥最长有效时间，单位秒，默认 1800，最大可设置 7200 |
+        |bucket|String| 存储桶名称：bucketName-appid, 如 test-125000000|
+        |region|String| 存储桶所属地域，如 ap-guangzhou|
+        |allow_prefix|list|资源的前缀，可以根据自己网站的用户登录态判断允许上传的具体路径，例子： a.jpg 或者 a/* 或者 * (使用通配符*存在重大安全风险, 请谨慎评估使用)|
+        |allow_actions|list| 授予 COS API 权限集合, 如简单上传操作：name/cos:PutObject|
+        |policy|dict| 策略：由 allow_actions、bucket、allow_prefix字段组成的描述授权的具体信息|
+        
+        ### 返回值说明
+        
+        |字段|类型|描述|
+        | ---- | ---- | ---- |
+        |credentials | dict | 临时密钥信息 |
+        |tmpSecretId | String | 临时密钥 Id，可用于计算签名 |
+        |tmpSecretKey | String | 临时密钥 Key，可用于计算签名 |
+        |sessionToken | String | 请求时需要用的 token 字符串，最终请求 COS API 时，需要放在 Header 的 x-cos-security-token 字段 |
+        |startTime | String | 密钥的起始时间，是 UNIX 时间戳 |
+        |expiredTime | String | 密钥的失效时间，是 UNIX 时间戳 |
+        
+        ### 返回结果
+        
+        成功的话，可以拿到包含密钥的 JSON 文本：
+        
+        ```json
+        {
+            "credentials": {
+                "tmpSecretId": "AKIDEPMQB_Q9Jt2fJxXyIekOzKZzx-sdGQgBga4TzsUdTWL9xlvsjInOHhCYFqfoKOY4",
+                "tmpSecretKey": "W/3Lbl1YEW02mCoawIesl5kNehSskrSbp1cT1tgW70g=",
+                "sessionToken": "c6xnSYAxyFbX8Y50627y9AA79u6Qfucw6924760b61588b79fea4c277b01ba157UVdr_10Y30bdpYtO8CXedYZe3KKZ_DyzaPiSFfNAcbr2MTfAgwJe-dhYhfyLMkeCqWyTNF-rOdOb0rp4Gto7p4yQAKuIPhQhuDd77gcAyGakC2WXHVd6ZuVaYIXBizZxqIHAf4lPiLHa6SZejSQfa_p5Ip2U1cAdkEionKbrX97xTKTcA_5Pu525CFSzHZIQibc2uNMZ-IRdQp12MaXZB6bxM6nB4xXH45mDIlbIGjaAsrtRJJ3csmf82uBKaJrYQoguAjBepMH91WcH87LlW9Ya3emNfVX7NMRRf64riYd_vomGF0TLgan9smEKAOdtaL94IkLvVJdhLqpvjBjp_4JCdqwlFAixaTzGJHdJzpGWOh0mQ6jDegAWgRYTrJvc5caYTz7Vphl8XoX5wHKKESUn_vqyTAid32t0vNYE034FIelxYT6VXuetYD_mvPfbHVDIXaFt7e_O8hRLkFwrdAIVaUml1mRPvccv2qOWSXs"
+            },
+            "expiration": "2019-08-07T08:54:35Z",
+            "startTime": 1565166275,
+            "expiredTime": 1565168075
+        }
+        ```
+        
+        ### get_policy
+        
+        获取策略(policy)接口。本接口适用于接收 Web、iOS、Android 客户端 SDK 提供的 Scope 参数。推荐您把 Scope 参数放在请求的 Body 里面，通过 POST 方式传到后台。
+        
+        ### 参数说明
+        
+        |字段|类型|描述|
+        | ---- | ---- | ---- |
+        |bucket|String| 存储桶名称：bucketName-appid, 如 test-125000000|
+        |region|String| 存储桶所属地域，如 ap-guangzhou|
+        |resource_prefix|String|资源的前缀，可以根据自己网站的用户登录态判断允许上传的具体路径，例子： a.jpg 或者 a/* 或者 * (使用通配符*存在重大安全风险, 请谨慎评估使用) |
+        |action|String| 授予 COS API 权限，, 如简单上传操作：name/cos:PutObject|
+        |scope|Scope| 构造policy的信息：由 action、bucket、region、sourcePrefix组成|
+        
+        ### 返回值说明
+        |字段|类型|描述|
+        | ---- | ---- | ---- |
+        |policy | dict | 申请临时密钥所需的权限策略 |
+        
+        
+        ### 返回结果
+        ```json
+        {
+        "version":"2.0",
+        "statement":[
+        	{
+        		"action":["name/cos:PutObject"],
+        		"effect":"allow",
+        		"resource":["qcs::cos:ap-guangzhou:uid/1250000000:example-1250000000/1.txt"]
+        	},
+        	{
+        		"action":["name/cos:GetObject" ],
+        		"effect":"allow",
+        		"resource":["qcs::cos:ap-guangzhou:uid/1250000000:example-1250000000/dir/exampleobject" ]
+        	}
+        ]
+        }
+        ```
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-
-## 获取 SDK
-
-```
-pip install -U qcloud-python-sts
-```
-
-## 调用示例
-
-请查看 [demo](https://github.com/tencentyun/qcloud-cos-sts-sdk/tree/master/python/demo) 里的示例。
-
-## 接口说明
-
-### get_credential
-
-获取临时密钥接口
-
-### 参数说明
-
-|字段|类型|描述|
-| ---- | ---- | ---- |
-|secret_id|String| 云 API 密钥 Id|
-|secret_key|String| 云 API 密钥 key|
-|duration_seconds|long| 要申请的临时密钥最长有效时间，单位秒，默认 1800，最大可设置 7200 |
-|bucket|String| 存储桶名称：bucketName-appid, 如 test-125000000|
-|region|String| 存储桶所属地域，如 ap-guangzhou|
-|allow_prefix|list|资源的前缀，可以根据自己网站的用户登录态判断允许上传的具体路径，例子： a.jpg 或者 a/* 或者 * (使用通配符*存在重大安全风险, 请谨慎评估使用)|
-|allow_actions|list| 授予 COS API 权限集合, 如简单上传操作：name/cos:PutObject|
-|policy|dict| 策略：由 allow_actions、bucket、allow_prefix字段组成的描述授权的具体信息|
-
-### 返回值说明
-
-|字段|类型|描述|
-| ---- | ---- | ---- |
-|credentials | dict | 临时密钥信息 |
-|tmpSecretId | String | 临时密钥 Id，可用于计算签名 |
-|tmpSecretKey | String | 临时密钥 Key，可用于计算签名 |
-|sessionToken | String | 请求时需要用的 token 字符串，最终请求 COS API 时，需要放在 Header 的 x-cos-security-token 字段 |
-|startTime | String | 密钥的起始时间，是 UNIX 时间戳 |
-|expiredTime | String | 密钥的失效时间，是 UNIX 时间戳 |
-
-### 返回结果
-
-成功的话，可以拿到包含密钥的 JSON 文本：
-
-```json
-{
-    "credentials": {
-        "tmpSecretId": "AKIDEPMQB_Q9Jt2fJxXyIekOzKZzx-sdGQgBga4TzsUdTWL9xlvsjInOHhCYFqfoKOY4",
-        "tmpSecretKey": "W/3Lbl1YEW02mCoawIesl5kNehSskrSbp1cT1tgW70g=",
-        "sessionToken": "c6xnSYAxyFbX8Y50627y9AA79u6Qfucw6924760b61588b79fea4c277b01ba157UVdr_10Y30bdpYtO8CXedYZe3KKZ_DyzaPiSFfNAcbr2MTfAgwJe-dhYhfyLMkeCqWyTNF-rOdOb0rp4Gto7p4yQAKuIPhQhuDd77gcAyGakC2WXHVd6ZuVaYIXBizZxqIHAf4lPiLHa6SZejSQfa_p5Ip2U1cAdkEionKbrX97xTKTcA_5Pu525CFSzHZIQibc2uNMZ-IRdQp12MaXZB6bxM6nB4xXH45mDIlbIGjaAsrtRJJ3csmf82uBKaJrYQoguAjBepMH91WcH87LlW9Ya3emNfVX7NMRRf64riYd_vomGF0TLgan9smEKAOdtaL94IkLvVJdhLqpvjBjp_4JCdqwlFAixaTzGJHdJzpGWOh0mQ6jDegAWgRYTrJvc5caYTz7Vphl8XoX5wHKKESUn_vqyTAid32t0vNYE034FIelxYT6VXuetYD_mvPfbHVDIXaFt7e_O8hRLkFwrdAIVaUml1mRPvccv2qOWSXs"
-    },
-    "expiration": "2019-08-07T08:54:35Z",
-    "startTime": 1565166275,
-    "expiredTime": 1565168075
-}
-```
-
-### get_policy
-
-获取策略(policy)接口。本接口适用于接收 Web、iOS、Android 客户端 SDK 提供的 Scope 参数。推荐您把 Scope 参数放在请求的 Body 里面，通过 POST 方式传到后台。
-
-### 参数说明
-
-|字段|类型|描述|
-| ---- | ---- | ---- |
-|bucket|String| 存储桶名称：bucketName-appid, 如 test-125000000|
-|region|String| 存储桶所属地域，如 ap-guangzhou|
-|resource_prefix|String|资源的前缀，可以根据自己网站的用户登录态判断允许上传的具体路径，例子： a.jpg 或者 a/* 或者 * (使用通配符*存在重大安全风险, 请谨慎评估使用) |
-|action|String| 授予 COS API 权限，, 如简单上传操作：name/cos:PutObject|
-|scope|Scope| 构造policy的信息：由 action、bucket、region、sourcePrefix组成|
-
-### 返回值说明
-|字段|类型|描述|
-| ---- | ---- | ---- |
-|policy | dict | 申请临时密钥所需的权限策略 |
-
-
-### 返回结果
-```json
-{
-"version":"2.0",
-"statement":[
-	{
-		"action":["name/cos:PutObject"],
-		"effect":"allow",
-		"resource":["qcs::cos:ap-guangzhou:uid/1250000000:example-1250000000/1.txt"]
-	},
-	{
-		"action":["name/cos:GetObject" ],
-		"effect":"allow",
-		"resource":["qcs::cos:ap-guangzhou:uid/1250000000:example-1250000000/dir/exampleobject" ]
-	}
-]
-}
-```
-
-
```

### Comparing `qcloud-python-sts-3.1.5/setup.py` & `qcloud-python-sts-3.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import io
 
 with io.open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='qcloud-python-sts',
-    version='3.1.5',
+    version='3.1.6',
     description='this is sts for python on v3',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/tencentyun/qcloud-cos-sts-sdk',
     author='qcloudterminal',
     author_email='qcloudterminal@gmail.com',
     license='MIT',
```


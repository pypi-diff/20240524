# Comparing `tmp/pyva_framework-3.3.3.tar.gz` & `tmp/pyva_framework-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyva_framework-3.3.3.tar", last modified: Tue May 21 07:18:55 2024, max compression
+gzip compressed data, was "pyva_framework-3.3.4.tar", last modified: Fri May 24 08:50:13 2024, max compression
```

## Comparing `pyva_framework-3.3.3.tar` & `pyva_framework-3.3.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.998657 pyva_framework-3.3.3/
--rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/LICENSE
--rw-r--r--   0 szq        (501) staff       (20)     2464 2024-05-21 07:18:55.998376 pyva_framework-3.3.3/PKG-INFO
--rw-r--r--   0 szq        (501) staff       (20)     1349 2024-05-21 06:47:59.000000 pyva_framework-3.3.3/README.md
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.989681 pyva_framework-3.3.3/pyva/
--rw-r--r--   0 szq        (501) staff       (20)     1455 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/Application.py
--rw-r--r--   0 szq        (501) staff       (20)      708 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/Global.py
--rw-r--r--   0 szq        (501) staff       (20)     1010 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/GlobalInit.py
--rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.989934 pyva_framework-3.3.3/pyva/cli/
--rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/cli/__init__.py
--rw-r--r--   0 szq        (501) staff       (20)     1464 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/cli/main.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.990054 pyva_framework-3.3.3/pyva/client/
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.991561 pyva_framework-3.3.3/pyva/client/dingtalk/
--rw-r--r--   0 szq        (501) staff       (20)     2563 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkContactClient.py
--rw-r--r--   0 szq        (501) staff       (20)     3239 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkOauth2Client.py
--rw-r--r--   0 szq        (501) staff       (20)     6758 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkRobotClient.py
--rw-r--r--   0 szq        (501) staff       (20)     5526 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkYidaClient.py
--rw-r--r--   0 szq        (501) staff       (20)       31 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/dingtalk/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.992264 pyva_framework-3.3.3/pyva/common/
--rw-r--r--   0 szq        (501) staff       (20)      999 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/common/FastapiEvents.py
--rw-r--r--   0 szq        (501) staff       (20)     1911 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/common/FastapiException.py
--rw-r--r--   0 szq        (501) staff       (20)     1229 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/common/LoggerHandler.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/common/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.993634 pyva_framework-3.3.3/pyva/config/
--rw-r--r--   0 szq        (501) staff       (20)     1069 2024-05-21 06:55:20.000000 pyva_framework-3.3.3/pyva/config/AppConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      893 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/DbConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      525 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/config/DingtalkConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      128 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/DingtalkRobotConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      729 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/FastapiConfig.py
--rw-r--r--   0 szq        (501) staff       (20)     3524 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/config/LoggingConfig.py
--rw-r--r--   0 szq        (501) staff       (20)       88 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/MongoConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      894 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/NacosConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      392 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/config/RedisConfig.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/config/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.994125 pyva_framework-3.3.3/pyva/dao/
--rw-r--r--   0 szq        (501) staff       (20)     1401 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/dao/BaseDao.py
--rw-r--r--   0 szq        (501) staff       (20)     5952 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/dao/ListDao.py
--rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/dao/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.994524 pyva_framework-3.3.3/pyva/dto/
--rw-r--r--   0 szq        (501) staff       (20)     1360 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/dto/BaseDto.py
--rw-r--r--   0 szq        (501) staff       (20)     1395 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/dto/ListDto.py
--rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/dto/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.995029 pyva_framework-3.3.3/pyva/entity/
--rw-r--r--   0 szq        (501) staff       (20)     1190 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/entity/BaseEntity.py
--rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/entity/GeneralHumpEntity.py
--rw-r--r--   0 szq        (501) staff       (20)      441 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/entity/HumpEntity.py
--rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/entity/__init__.py
--rw-r--r--   0 szq        (501) staff       (20)     1047 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/startupApp.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.997274 pyva_framework-3.3.3/pyva/util/
--rw-r--r--   0 szq        (501) staff       (20)     5269 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/ConfigUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     9245 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/DbUtil.py
--rw-r--r--   0 szq        (501) staff       (20)      581 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/DictUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2780 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/EntityUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1081 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/FileUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1807 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/IpUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2006 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/JsonUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2034 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/LockerUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1985 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/MongoUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     6692 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/NacosUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1608 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/PathUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     4136 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/util/QrcodeUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2180 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/util/RedisUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     6613 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/TimeUtil.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/util/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.998026 pyva_framework-3.3.3/pyva_framework.egg-info/
--rw-r--r--   0 szq        (501) staff       (20)     2464 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/PKG-INFO
--rw-r--r--   0 szq        (501) staff       (20)     1578 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/SOURCES.txt
--rw-r--r--   0 szq        (501) staff       (20)        1 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/dependency_links.txt
--rw-r--r--   0 szq        (501) staff       (20)       43 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/entry_points.txt
--rw-r--r--   0 szq        (501) staff       (20)      307 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/requires.txt
--rw-r--r--   0 szq        (501) staff       (20)        5 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/top_level.txt
--rw-r--r--   0 szq        (501) staff       (20)       38 2024-05-21 07:18:55.998706 pyva_framework-3.3.3/setup.cfg
--rw-r--r--   0 szq        (501) staff       (20)     1092 2024-05-21 07:02:29.000000 pyva_framework-3.3.3/setup.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.714496 pyva_framework-3.3.4/
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/LICENSE
+-rw-r--r--   0 szq        (501) staff       (20)     2464 2024-05-24 08:50:13.714257 pyva_framework-3.3.4/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1349 2024-05-21 06:47:59.000000 pyva_framework-3.3.4/README.md
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.704948 pyva_framework-3.3.4/pyva/
+-rw-r--r--   0 szq        (501) staff       (20)     1455 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/Application.py
+-rw-r--r--   0 szq        (501) staff       (20)      708 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/Global.py
+-rw-r--r--   0 szq        (501) staff       (20)     1010 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/GlobalInit.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.705217 pyva_framework-3.3.4/pyva/cli/
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/cli/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1464 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/cli/main.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.705343 pyva_framework-3.3.4/pyva/client/
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.706842 pyva_framework-3.3.4/pyva/client/dingtalk/
+-rw-r--r--   0 szq        (501) staff       (20)     2563 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkContactClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     3239 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkOauth2Client.py
+-rw-r--r--   0 szq        (501) staff       (20)     6758 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkRobotClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     5526 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkYidaClient.py
+-rw-r--r--   0 szq        (501) staff       (20)       31 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/dingtalk/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.707349 pyva_framework-3.3.4/pyva/common/
+-rw-r--r--   0 szq        (501) staff       (20)      999 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/common/FastapiEvents.py
+-rw-r--r--   0 szq        (501) staff       (20)     1911 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/common/FastapiException.py
+-rw-r--r--   0 szq        (501) staff       (20)     1229 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/common/LoggerHandler.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/common/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.708696 pyva_framework-3.3.4/pyva/config/
+-rw-r--r--   0 szq        (501) staff       (20)     1069 2024-05-21 06:55:20.000000 pyva_framework-3.3.4/pyva/config/AppConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      893 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/DbConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      525 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/config/DingtalkConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      128 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/DingtalkRobotConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      729 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/FastapiConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)     3524 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/config/LoggingConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       88 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/MongoConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      894 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/NacosConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      392 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/config/RedisConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/config/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.709244 pyva_framework-3.3.4/pyva/dao/
+-rw-r--r--   0 szq        (501) staff       (20)     1401 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/dao/BaseDao.py
+-rw-r--r--   0 szq        (501) staff       (20)     5952 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/dao/ListDao.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/dao/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.709671 pyva_framework-3.3.4/pyva/dto/
+-rw-r--r--   0 szq        (501) staff       (20)     1360 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/dto/BaseDto.py
+-rw-r--r--   0 szq        (501) staff       (20)     1395 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/dto/ListDto.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/dto/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.710225 pyva_framework-3.3.4/pyva/entity/
+-rw-r--r--   0 szq        (501) staff       (20)     1190 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/entity/BaseEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/entity/GeneralHumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)      441 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/entity/HumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/entity/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1047 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/startupApp.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.712984 pyva_framework-3.3.4/pyva/util/
+-rw-r--r--   0 szq        (501) staff       (20)     5269 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/ConfigUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     9245 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/DbUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)      581 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/DictUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2780 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/EntityUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1081 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/FileUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1807 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/IpUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2006 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/JsonUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2034 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/LockerUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1985 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/MongoUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6692 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/NacosUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1608 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/PathUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     4136 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/util/QrcodeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2180 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/util/RedisUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6613 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/TimeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/util/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.713972 pyva_framework-3.3.4/pyva_framework.egg-info/
+-rw-r--r--   0 szq        (501) staff       (20)     2464 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1578 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 szq        (501) staff       (20)        1 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 szq        (501) staff       (20)       43 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/entry_points.txt
+-rw-r--r--   0 szq        (501) staff       (20)      307 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/requires.txt
+-rw-r--r--   0 szq        (501) staff       (20)        5 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/top_level.txt
+-rw-r--r--   0 szq        (501) staff       (20)       38 2024-05-24 08:50:13.714533 pyva_framework-3.3.4/setup.cfg
+-rw-r--r--   0 szq        (501) staff       (20)     1092 2024-05-24 08:44:20.000000 pyva_framework-3.3.4/setup.py
```

### Comparing `pyva_framework-3.3.3/LICENSE` & `pyva_framework-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/PKG-INFO` & `pyva_framework-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyva-framework
-Version: 3.3.3
+Version: 3.3.4
 Summary: PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 Home-page: https://github.com/zhenqiang-sun/pyva
 Author: Zhenqiang Sun
 Author-email: zhenqiang.sun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: PyMySQL==1.1.0
 Requires-Dist: sqlacodegen==2.3.0
```

### Comparing `pyva_framework-3.3.3/README.md` & `pyva_framework-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/Application.py` & `pyva_framework-3.3.4/pyva/Application.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/Global.py` & `pyva_framework-3.3.4/pyva/Global.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/GlobalInit.py` & `pyva_framework-3.3.4/pyva/GlobalInit.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/cli/main.py` & `pyva_framework-3.3.4/pyva/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkContactClient.py` & `pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkContactClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkOauth2Client.py` & `pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkOauth2Client.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkRobotClient.py` & `pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkRobotClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkYidaClient.py` & `pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkYidaClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/common/FastapiEvents.py` & `pyva_framework-3.3.4/pyva/common/FastapiEvents.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/common/FastapiException.py` & `pyva_framework-3.3.4/pyva/common/FastapiException.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/common/LoggerHandler.py` & `pyva_framework-3.3.4/pyva/common/LoggerHandler.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/config/AppConfig.py` & `pyva_framework-3.3.4/pyva/config/AppConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/config/DbConfig.py` & `pyva_framework-3.3.4/pyva/config/DbConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/config/DingtalkConfig.py` & `pyva_framework-3.3.4/pyva/config/DingtalkConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/config/FastapiConfig.py` & `pyva_framework-3.3.4/pyva/config/FastapiConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/config/LoggingConfig.py` & `pyva_framework-3.3.4/pyva/config/LoggingConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/config/NacosConfig.py` & `pyva_framework-3.3.4/pyva/config/NacosConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/dao/BaseDao.py` & `pyva_framework-3.3.4/pyva/dao/BaseDao.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/dao/ListDao.py` & `pyva_framework-3.3.4/pyva/dao/ListDao.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/dto/BaseDto.py` & `pyva_framework-3.3.4/pyva/dto/BaseDto.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/dto/ListDto.py` & `pyva_framework-3.3.4/pyva/dto/ListDto.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/entity/BaseEntity.py` & `pyva_framework-3.3.4/pyva/entity/BaseEntity.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/entity/GeneralHumpEntity.py` & `pyva_framework-3.3.4/pyva/entity/GeneralHumpEntity.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/startupApp.py` & `pyva_framework-3.3.4/pyva/startupApp.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/ConfigUtil.py` & `pyva_framework-3.3.4/pyva/util/ConfigUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/DbUtil.py` & `pyva_framework-3.3.4/pyva/util/DbUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/DictUtil.py` & `pyva_framework-3.3.4/pyva/util/DictUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/EntityUtil.py` & `pyva_framework-3.3.4/pyva/util/EntityUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/FileUtil.py` & `pyva_framework-3.3.4/pyva/util/FileUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/IpUtil.py` & `pyva_framework-3.3.4/pyva/util/IpUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/JsonUtil.py` & `pyva_framework-3.3.4/pyva/util/JsonUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/LockerUtil.py` & `pyva_framework-3.3.4/pyva/util/LockerUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/MongoUtil.py` & `pyva_framework-3.3.4/pyva/util/MongoUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/NacosUtil.py` & `pyva_framework-3.3.4/pyva/util/NacosUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/PathUtil.py` & `pyva_framework-3.3.4/pyva/util/PathUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/QrcodeUtil.py` & `pyva_framework-3.3.4/pyva/util/QrcodeUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/RedisUtil.py` & `pyva_framework-3.3.4/pyva/util/RedisUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva/util/TimeUtil.py` & `pyva_framework-3.3.4/pyva/util/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/pyva_framework.egg-info/PKG-INFO` & `pyva_framework-3.3.4/pyva_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyva-framework
-Version: 3.3.3
+Version: 3.3.4
 Summary: PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 Home-page: https://github.com/zhenqiang-sun/pyva
 Author: Zhenqiang Sun
 Author-email: zhenqiang.sun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: PyMySQL==1.1.0
 Requires-Dist: sqlacodegen==2.3.0
```

### Comparing `pyva_framework-3.3.3/pyva_framework.egg-info/SOURCES.txt` & `pyva_framework-3.3.4/pyva_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.3/setup.py` & `pyva_framework-3.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
     requirements = re.sub(r'(?m)#.*$', '', requirements)
 
 setuptools.setup(
     name="pyva-framework",
-    version="3.3.3",
+    version="3.3.4",
     author="Zhenqiang Sun",
     author_email="zhenqiang.sun@gmail.com",
     description="PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhenqiang-sun/pyva",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.11",
+    python_requires=">=3.10",
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'pyva=pyva.cli.main:app',
         ],
     },
 )
```


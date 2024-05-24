# Comparing `tmp/hui-tools-0.4.1.tar.gz` & `tmp/hui-tools-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hui-tools-0.4.1.tar", last modified: Fri Apr 26 13:58:46 2024, max compression
+gzip compressed data, was "hui-tools-0.4.2.tar", last modified: Fri May 24 10:12:33 2024, max compression
```

## Comparing `hui-tools-0.4.1.tar` & `hui-tools-0.4.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.227215 hui-tools-0.4.1/
--rw-r--r--   0 liuminhui   (501) staff       (20)    11357 2023-07-29 10:14:17.000000 hui-tools-0.4.1/LICENSE
--rw-r--r--   0 liuminhui   (501) staff       (20)       53 2024-04-26 13:50:18.000000 hui-tools-0.4.1/MANIFEST.in
--rw-r--r--   0 liuminhui   (501) staff       (20)    17724 2024-04-26 13:58:46.226945 hui-tools-0.4.1/PKG-INFO
--rw-r--r--   0 liuminhui   (501) staff       (20)    15809 2024-04-15 11:39:36.000000 hui-tools-0.4.1/README.md
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.205510 hui-tools-0.4.1/hui_tools.egg-info/
--rw-r--r--   0 liuminhui   (501) staff       (20)    17724 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/PKG-INFO
--rw-r--r--   0 liuminhui   (501) staff       (20)     3866 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/SOURCES.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/dependency_links.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)       75 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/entry_points.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)      562 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/requires.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)       15 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/top_level.txt
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.205647 hui-tools-0.4.1/py_tools/
--rw-r--r--   0 liuminhui   (501) staff       (20)        1 2023-09-04 08:25:07.000000 hui-tools-0.4.1/py_tools/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.206787 hui-tools-0.4.1/py_tools/chatbot/
--rw-r--r--   0 liuminhui   (501) staff       (20)      128 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/chatbot/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)    11243 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/chatbot/app_server.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     5238 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/chatbot/chatbot.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2385 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/chatbot/factory.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.207074 hui-tools-0.4.1/py_tools/connections/
--rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.207559 hui-tools-0.4.1/py_tools/connections/db/
--rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/db/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.209129 hui-tools-0.4.1/py_tools/connections/db/mysql/
--rw-r--r--   0 liuminhui   (501) staff       (20)      215 2024-03-28 15:06:17.000000 hui-tools-0.4.1/py_tools/connections/db/mysql/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)    20121 2024-04-17 03:58:06.000000 hui-tools-0.4.1/py_tools/connections/db/mysql/client.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1722 2024-04-17 03:58:06.000000 hui-tools-0.4.1/py_tools/connections/db/mysql/orm_model.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2581 2024-04-24 02:13:05.000000 hui-tools-0.4.1/py_tools/connections/db/redis_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.209638 hui-tools-0.4.1/py_tools/connections/http/
--rw-r--r--   0 liuminhui   (501) staff       (20)      158 2023-08-10 03:40:34.000000 hui-tools-0.4.1/py_tools/connections/http/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     8809 2023-09-28 06:51:00.000000 hui-tools-0.4.1/py_tools/connections/http/client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.210200 hui-tools-0.4.1/py_tools/connections/mq/
--rw-r--r--   0 liuminhui   (501) staff       (20)      185 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/mq/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      184 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/mq/kafka_client.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      187 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/mq/rabbitmq_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.210581 hui-tools-0.4.1/py_tools/connections/oss/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2024-03-28 01:23:21.000000 hui-tools-0.4.1/py_tools/connections/oss/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1955 2024-03-28 01:23:21.000000 hui-tools-0.4.1/py_tools/connections/oss/minio_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.210812 hui-tools-0.4.1/py_tools/constants/
--rw-r--r--   0 liuminhui   (501) staff       (20)      171 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/constants/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.211376 hui-tools-0.4.1/py_tools/data_models/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/data_models/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      270 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/data_models/time.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2674 2024-04-24 04:49:33.000000 hui-tools-0.4.1/py_tools/data_models/unit.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.212145 hui-tools-0.4.1/py_tools/decorators/
--rw-r--r--   0 liuminhui   (501) staff       (20)      213 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/decorators/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     6380 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/decorators/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     4831 2024-04-24 02:14:22.000000 hui-tools-0.4.1/py_tools/decorators/cache.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.214294 hui-tools-0.4.1/py_tools/enums/
--rw-r--r--   0 liuminhui   (501) staff       (20)      334 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/enums/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2304 2024-04-24 03:43:33.000000 hui-tools-0.4.1/py_tools/enums/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1234 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/enums/error.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/enums/feishu.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      452 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/enums/http.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      486 2024-04-24 03:43:33.000000 hui-tools-0.4.1/py_tools/enums/pub_biz.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-09-09 06:12:03.000000 hui-tools-0.4.1/py_tools/enums/time.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.214662 hui-tools-0.4.1/py_tools/exceptions/
--rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/exceptions/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1141 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/exceptions/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.214877 hui-tools-0.4.1/py_tools/logging/
--rw-r--r--   0 liuminhui   (501) staff       (20)       26 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/logging/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.215268 hui-tools-0.4.1/py_tools/meta_cls/
--rw-r--r--   0 liuminhui   (501) staff       (20)       35 2023-09-04 07:12:03.000000 hui-tools-0.4.1/py_tools/meta_cls/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      963 2023-09-09 06:35:40.000000 hui-tools-0.4.1/py_tools/meta_cls/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.217872 hui-tools-0.4.1/py_tools/utils/
--rw-r--r--   0 liuminhui   (501) staff       (20)      166 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/utils/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1067 2024-04-24 11:01:10.000000 hui-tools-0.4.1/py_tools/utils/aio.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/utils/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     5992 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/utils/excel.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      951 2024-04-24 03:52:42.000000 hui-tools-0.4.1/py_tools/utils/func.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/utils/mask.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.218572 hui-tools-0.4.1/py_tools/utils/project_templates/
--rw-r--r--   0 liuminhui   (501) staff       (20)       35 2024-04-26 11:46:23.000000 hui-tools-0.4.1/py_tools/utils/project_templates/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2770 2024-04-26 12:24:15.000000 hui-tools-0.4.1/py_tools/utils/project_templates/make_pro.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.202352 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.218866 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.218978 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/constants/
--rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/constants/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.219282 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/
--rw-r--r--   0 liuminhui   (501) staff       (20)      745 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.202697 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.219684 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/manage/
--rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/manage/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      150 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/manage/user.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.220327 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/table/
--rw-r--r--   0 liuminhui   (501) staff       (20)       28 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/table/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      446 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/table/user.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.220996 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/redis/
--rw-r--r--   0 liuminhui   (501) staff       (20)       66 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/redis/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)       81 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/redis/cache_info.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      132 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/redis/client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.221186 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/
--rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.221454 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/api_models/
--rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/api_models/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.221677 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/logic_models/
--rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/logic_models/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.222082 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/enums/
--rw-r--r--   0 liuminhui   (501) staff       (20)       33 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/enums/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      369 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/enums/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.222288 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/handlers/
--rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/handlers/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.222498 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/middlewares/
--rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/middlewares/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.222761 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/routes/
--rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/routes/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 11:46:23.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/server.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.223091 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/services/
--rw-r--r--   0 liuminhui   (501) staff       (20)        0 2023-09-05 15:16:08.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/services/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)       77 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/services/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.224165 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/
--rw-r--r--   0 liuminhui   (501) staff       (20)      399 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)       75 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/base_setting.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      235 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/db_setting.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1702 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/log_setting.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.225269 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/
--rw-r--r--   0 liuminhui   (501) staff       (20)       34 2023-10-30 08:27:36.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      239 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/context_util.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      721 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/log_util.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1153 2023-10-30 08:27:36.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/trace_util.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      919 2024-04-26 11:46:23.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/web.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      179 2023-09-09 16:16:35.000000 hui-tools-0.4.1/py_tools/utils/serializer.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     6538 2024-04-24 02:48:33.000000 hui-tools-0.4.1/py_tools/utils/time.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     4592 2024-04-24 03:58:59.000000 hui-tools-0.4.1/py_tools/utils/tree.py
--rw-r--r--   0 liuminhui   (501) staff       (20)       38 2024-04-26 13:58:46.227285 hui-tools-0.4.1/setup.cfg
--rw-r--r--   0 liuminhui   (501) staff       (20)     2498 2024-04-26 13:58:01.000000 hui-tools-0.4.1/setup.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.225476 hui-tools-0.4.1/tests/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.1/tests/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.707175 hui-tools-0.4.2/
+-rw-r--r--   0 liuminhui   (501) staff       (20)    11357 2023-07-29 10:14:17.000000 hui-tools-0.4.2/LICENSE
+-rw-r--r--   0 liuminhui   (501) staff       (20)       53 2024-04-26 13:50:18.000000 hui-tools-0.4.2/MANIFEST.in
+-rw-r--r--   0 liuminhui   (501) staff       (20)     9871 2024-05-24 10:12:33.706878 hui-tools-0.4.2/PKG-INFO
+-rw-r--r--   0 liuminhui   (501) staff       (20)     7924 2024-05-24 10:12:30.000000 hui-tools-0.4.2/README.md
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.686040 hui-tools-0.4.2/hui_tools.egg-info/
+-rw-r--r--   0 liuminhui   (501) staff       (20)     9871 2024-05-24 10:12:33.000000 hui-tools-0.4.2/hui_tools.egg-info/PKG-INFO
+-rw-r--r--   0 liuminhui   (501) staff       (20)     3866 2024-05-24 10:12:33.000000 hui-tools-0.4.2/hui_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-05-24 10:12:33.000000 hui-tools-0.4.2/hui_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)       75 2024-05-24 10:12:33.000000 hui-tools-0.4.2/hui_tools.egg-info/entry_points.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)      598 2024-05-24 10:12:33.000000 hui-tools-0.4.2/hui_tools.egg-info/requires.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)       15 2024-05-24 10:12:33.000000 hui-tools-0.4.2/hui_tools.egg-info/top_level.txt
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.686184 hui-tools-0.4.2/py_tools/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2023-09-04 08:25:07.000000 hui-tools-0.4.2/py_tools/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.687558 hui-tools-0.4.2/py_tools/chatbot/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      128 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/chatbot/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)    11243 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/chatbot/app_server.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     5238 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/chatbot/chatbot.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2385 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/chatbot/factory.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.687733 hui-tools-0.4.2/py_tools/connections/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/connections/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.688060 hui-tools-0.4.2/py_tools/connections/db/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/connections/db/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.689165 hui-tools-0.4.2/py_tools/connections/db/mysql/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      215 2024-03-28 15:06:17.000000 hui-tools-0.4.2/py_tools/connections/db/mysql/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)    20121 2024-04-17 03:58:06.000000 hui-tools-0.4.2/py_tools/connections/db/mysql/client.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1722 2024-04-17 03:58:06.000000 hui-tools-0.4.2/py_tools/connections/db/mysql/orm_model.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2581 2024-04-24 02:13:05.000000 hui-tools-0.4.2/py_tools/connections/db/redis_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.689664 hui-tools-0.4.2/py_tools/connections/http/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      158 2023-08-10 03:40:34.000000 hui-tools-0.4.2/py_tools/connections/http/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)    10334 2024-05-24 09:56:44.000000 hui-tools-0.4.2/py_tools/connections/http/client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.690159 hui-tools-0.4.2/py_tools/connections/mq/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      185 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/connections/mq/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      184 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/connections/mq/kafka_client.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      187 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/connections/mq/rabbitmq_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.690590 hui-tools-0.4.2/py_tools/connections/oss/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2024-03-28 01:23:21.000000 hui-tools-0.4.2/py_tools/connections/oss/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1955 2024-03-28 01:23:21.000000 hui-tools-0.4.2/py_tools/connections/oss/minio_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.690848 hui-tools-0.4.2/py_tools/constants/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      171 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/constants/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.691398 hui-tools-0.4.2/py_tools/data_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/data_models/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      270 2023-09-09 16:15:14.000000 hui-tools-0.4.2/py_tools/data_models/time.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2674 2024-04-24 04:49:33.000000 hui-tools-0.4.2/py_tools/data_models/unit.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.692125 hui-tools-0.4.2/py_tools/decorators/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      213 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/decorators/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     6380 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/decorators/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     5051 2024-04-28 07:00:05.000000 hui-tools-0.4.2/py_tools/decorators/cache.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.693944 hui-tools-0.4.2/py_tools/enums/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      325 2024-05-24 09:46:39.000000 hui-tools-0.4.2/py_tools/enums/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2304 2024-04-24 03:43:33.000000 hui-tools-0.4.2/py_tools/enums/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1234 2023-09-09 16:15:14.000000 hui-tools-0.4.2/py_tools/enums/error.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/enums/feishu.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      342 2024-05-24 09:46:39.000000 hui-tools-0.4.2/py_tools/enums/http.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      486 2024-04-24 03:43:33.000000 hui-tools-0.4.2/py_tools/enums/pub_biz.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-09-09 06:12:03.000000 hui-tools-0.4.2/py_tools/enums/time.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.694342 hui-tools-0.4.2/py_tools/exceptions/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/exceptions/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1141 2023-09-09 16:15:14.000000 hui-tools-0.4.2/py_tools/exceptions/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.694569 hui-tools-0.4.2/py_tools/logging/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       26 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/logging/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.694961 hui-tools-0.4.2/py_tools/meta_cls/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       35 2023-09-04 07:12:03.000000 hui-tools-0.4.2/py_tools/meta_cls/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      963 2023-09-09 06:35:40.000000 hui-tools-0.4.2/py_tools/meta_cls/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.697390 hui-tools-0.4.2/py_tools/utils/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      166 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/utils/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1067 2024-04-24 11:01:10.000000 hui-tools-0.4.2/py_tools/utils/aio.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/utils/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     5992 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/utils/excel.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      951 2024-04-24 03:52:42.000000 hui-tools-0.4.2/py_tools/utils/func.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.2/py_tools/utils/mask.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.697931 hui-tools-0.4.2/py_tools/utils/project_templates/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       35 2024-04-26 11:46:23.000000 hui-tools-0.4.2/py_tools/utils/project_templates/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2771 2024-04-26 14:17:58.000000 hui-tools-0.4.2/py_tools/utils/project_templates/make_pro.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.682775 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.698235 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.698336 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/constants/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 14:20:56.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/constants/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.698443 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      745 2024-04-26 14:17:58.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.683118 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/orm/
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.699144 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/orm/manage/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-04-26 11:15:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/orm/manage/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      151 2024-04-26 14:17:58.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/orm/manage/user.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.699806 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/orm/table/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       28 2024-04-26 11:15:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/orm/table/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      447 2024-04-26 14:17:58.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/orm/table/user.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.700569 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/redis/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       66 2024-04-26 11:15:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/redis/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       80 2024-04-26 14:17:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/redis/cache_info.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      132 2024-04-26 11:15:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/redis/client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.700823 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/data_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 14:20:56.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/data_models/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.700945 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/data_models/api_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 14:20:56.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/data_models/api_models/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.701048 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/data_models/logic_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 14:20:56.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/data_models/logic_models/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.701470 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/enums/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       33 2024-04-26 11:15:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/enums/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      369 2024-04-26 11:27:24.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/enums/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.702079 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/handlers/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 14:20:56.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/handlers/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.702210 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/middlewares/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 14:20:56.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/middlewares/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.702319 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/routes/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 14:20:56.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/routes/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 11:46:23.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/server.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.702544 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/services/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2023-09-05 15:16:08.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/services/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       75 2024-04-26 14:17:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/services/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.703657 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/settings/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      292 2024-04-26 14:22:16.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/settings/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       74 2024-04-26 14:17:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/settings/base_setting.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      234 2024-04-26 14:17:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/settings/db_setting.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1702 2024-04-26 11:27:24.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/settings/log_setting.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.705157 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/utils/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       34 2023-10-30 08:27:36.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/utils/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      239 2024-04-26 11:15:57.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/utils/context_util.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      721 2024-04-26 14:17:58.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/utils/log_util.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1153 2023-10-30 08:27:36.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/utils/trace_util.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      919 2024-04-26 11:46:23.000000 hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/utils/web.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      179 2023-09-09 16:16:35.000000 hui-tools-0.4.2/py_tools/utils/serializer.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     6538 2024-04-24 02:48:33.000000 hui-tools-0.4.2/py_tools/utils/time.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     4592 2024-04-24 03:58:59.000000 hui-tools-0.4.2/py_tools/utils/tree.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       38 2024-05-24 10:12:33.707232 hui-tools-0.4.2/setup.cfg
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2526 2024-05-24 10:12:30.000000 hui-tools-0.4.2/setup.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-05-24 10:12:33.705443 hui-tools-0.4.2/tests/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.2/tests/__init__.py
```

### Comparing `hui-tools-0.4.1/LICENSE` & `hui-tools-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/hui_tools.egg-info/SOURCES.txt` & `hui-tools-0.4.2/hui_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/chatbot/app_server.py` & `hui-tools-0.4.2/py_tools/chatbot/app_server.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/chatbot/chatbot.py` & `hui-tools-0.4.2/py_tools/chatbot/chatbot.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/chatbot/factory.py` & `hui-tools-0.4.2/py_tools/chatbot/factory.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/connections/db/mysql/client.py` & `hui-tools-0.4.2/py_tools/connections/db/mysql/client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/connections/db/mysql/orm_model.py` & `hui-tools-0.4.2/py_tools/connections/db/mysql/orm_model.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/connections/db/redis_client.py` & `hui-tools-0.4.2/py_tools/connections/db/redis_client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/connections/http/client.py` & `hui-tools-0.4.2/py_tools/connections/http/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,162 +1,200 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 # @Author: Hui
 # @Desc: { http客户端 }
 # @Date: 2023/08/10 09:33
-import httpx
+import aiohttp
 from datetime import timedelta
 
 import requests
+from aiohttp import ClientResponse
 
-from py_tools.enums import HttpMethod, RespFmt
+from py_tools.enums import HttpMethod
+
+
+class AsyncRequest:
+    def __init__(self, client, method: HttpMethod, url, **kwargs):
+        self.client = client
+        self.method = method
+        self.url = url
+        self.params = kwargs.pop("params", None)
+        self.data = kwargs.pop("data", None)
+        self.timeout = kwargs.pop("timeout", None)
+        self.headers = kwargs.pop("headers", None)
+        self.kwargs = kwargs
+
+    async def execute(self) -> ClientResponse:
+        return await self.client._request(
+            self.method,
+            self.url,
+            params=self.params,
+            data=self.data,
+            timeout=self.timeout,
+            headers=self.headers,
+            **self.kwargs
+        )
+
+    async def json(self):
+        async with await self.execute() as response:
+            return await response.json()
+
+    async def text(self):
+        async with await self.execute() as response:
+            return await response.text()
+
+    async def bytes(self):
+        async with await self.execute() as response:
+            return await response.read()
+
+    async def stream(self, chunk_size=1024):
+        async with await self.execute() as response:
+            async for chunk in response.content.iter_chunked(chunk_size):
+                yield chunk
 
 
 class AsyncHttpClient:
-    """异步HTTP客户端
+    """异步HTTP客户端(支持链式调用)
 
-    通过httpx封装，实现了常见的HTTP方法,支持设置超时时间、请求参数等，简化了异步调用的层级缩进。
+    基于aiohttp封装，实现了常见的HTTP方法,支持设置超时时间、请求参数等，简化了异步调用的层级缩进。
+
+    Examples:
+        >>> url = "https://juejin.cn/"
+        >>> resp = await AsyncHttpClient().get(url).execute()
+        >>> text_data = await AsyncHttpClient().get(url, params={"test": "hui"}).text()
+        >>> json_data = await AsyncHttpClient().post(url, data={"test": "hui"}).json()
+        >>> byte_data = await AsyncHttpClient().get(url).bytes()
+        >>>
+        >>> async for chunk in AsyncHttpClient().get(url).stream(chunk_size=512):
+        >>>     # 流式调用
+        >>>     print(chunk)
 
     Attributes:
         default_timeout: 默认请求超时时间,单位秒
         default_headers: 默认请求头字典
-        default_resp_fmt: 默认响应格式json
-        client: httpx 异步客户端
-        response: 每次实例请求的响应
+        new_session: 是否使用的新的客户端，默认共享一个 ClientSession
     """
+    # aiohttp 异步客户端
+    client_session: aiohttp.ClientSession = None
+    client_session_set = set()
 
-    def __init__(self, timeout=timedelta(seconds=10), headers: dict = None, resp_fmt: RespFmt = RespFmt.JSON):
+    def __init__(self, timeout=timedelta(seconds=10), headers: dict = None, new_session=False, **kwargs):
         """构造异步HTTP客户端"""
-        self.default_timeout = timeout
+        self.default_timeout = aiohttp.ClientTimeout(timeout.total_seconds())
         self.default_headers = headers or {}
-        self.default_resp_fmt = resp_fmt
-        self.client = httpx.AsyncClient()
-        self.response: httpx.Response = None
+        self.new_session = new_session
+        self.kwargs = kwargs
+
+    async def _get_client_session(self):
+        if self.new_session:
+            client_session = aiohttp.ClientSession(
+                headers=self.default_headers, timeout=self.default_timeout, **self.kwargs
+            )
+            self.client_session_set.add(client_session)
+            return client_session
+
+        if self.client_session is not None:
+            return self.client_session
+
+        AsyncHttpClient.client_session = aiohttp.ClientSession(
+            headers=self.default_headers, timeout=self.default_timeout, **self.kwargs
+        )
+        self.client_session_set.add(AsyncHttpClient.client_session)
+        return self.client_session
+
+    @classmethod
+    async def close(cls):
+        for client_session in cls.client_session_set:
+            await client_session.close()
 
     async def _request(
             self,
-            method: HttpMethod, url: str,
-            params: dict = None, data: dict = None,
-            timeout: timedelta = None, **kwargs
+            method: HttpMethod,
+            url: str,
+            params: dict = None,
+            data: dict = None,
+            timeout: timedelta = None,
+            headers: dict = None,
+            **kwargs
     ):
         """内部请求实现方法
 
         创建客户端会话,构造并发送HTTP请求,返回响应对象
 
         Args:
             method: HttpMethod 请求方法, 'GET', 'POST' 等
             url: 请求URL
             params: 请求查询字符串参数字典
             data: 请求体数据字典
             timeout: 超时时间,单位秒
+            headers: 请求头
             kwargs: 其他关键字参数
 
         Returns:
             httpx.Response: HTTP响应对象
         """
         timeout = timeout or self.default_timeout
-        headers = self.default_headers or {}
-        self.response = await self.client.request(
-            method=method.value,
-            url=url,
-            params=params,
-            data=data,
-            headers=headers,
-            timeout=timeout.total_seconds(),
-            **kwargs
-        )
-        return self.response
+        if isinstance(timeout, timedelta):
+            timeout = aiohttp.ClientTimeout(timeout.total_seconds())
 
-    def _parse_response(self, resp_fmt: RespFmt = None):
-        """解析响应
-
-        Args:
-            resp_fmt: 响应格式
-
-        Returns:
-            resp Union[dict, bytes, str]
-        """
-        resp_fmt = resp_fmt or self.default_resp_fmt
-        resp_content_mapping = {
-            RespFmt.JSON: self.json,
-            RespFmt.BYTES: self.bytes,
-            RespFmt.TEXT: self.text,
-        }
-        resp_func = resp_content_mapping.get(resp_fmt)
-        return resp_func()
-
-    def json(self):
-        return self.response.json()
-
-    def bytes(self):
-        return self.response.content
-
-    def text(self):
-        return self.response.text
+        headers = headers or {}
+        headers = self.default_headers.update(**headers)
+        client_session = await self._get_client_session()
+        return await client_session.request(
+            method.value, url, params=params, data=data, timeout=timeout, headers=headers, **kwargs
+        )
 
-    async def get(self, url: str, params: dict = None, timeout: timedelta = None, resp_fmt: RespFmt = None, **kwargs):
+    def get(self, url: str, params: dict = None, timeout: timedelta = None, **kwargs) -> AsyncRequest:
         """GET请求
 
         Args:
             url: 请求URL
             params: 请求查询字符串参数字典
             timeout: 请求超时时间,单位秒
-            resp_fmt: 响应格式，默认None 使用实例对象的 default_resp_fmt
 
-        Returns:
-            resp => dict or bytes
+        Returns: AsyncRequest
         """
 
-        await self._request(HttpMethod.GET, url, params=params, timeout=timeout, **kwargs)
-        return self._parse_response(resp_fmt)
+        return AsyncRequest(self, HttpMethod.GET, url, params=params, timeout=timeout, **kwargs)
 
-    async def post(self, url: str, data: dict = None, timeout: timedelta = None, resp_fmt: RespFmt = None, **kwargs):
+    async def post(self, url: str, data: dict = None, timeout: timedelta = None, **kwargs) -> AsyncRequest:
         """POST请求
 
         Args:
             url: 请求URL
             data: 请求体数据字典
             timeout: 请求超时时间,单位秒
-            resp_fmt: 响应格式，默认None 使用实例对象的 default_resp_fmt
 
-        Returns:
-            resp => dict or bytes
+        Returns: AsyncRequest
         """
-        await self._request(HttpMethod.POST, url, data=data, timeout=timeout, **kwargs)
-        return self._parse_response(resp_fmt)
+        return AsyncRequest(self, HttpMethod.GET, url, data=data, timeout=timeout, **kwargs)
 
-    async def put(self, url: str, data: dict = None, timeout: timedelta = None, resp_fmt: RespFmt = None, **kwargs):
+    async def put(self, url: str, data: dict = None, timeout: timedelta = None, **kwargs):
         """PUT请求
 
         Args:
             url: 请求URL
             data: 请求体数据字典
             timeout: 请求超时时间,单位秒
-            resp_fmt: 响应格式，默认None 使用实例对象的 default_resp_fmt
 
-        Returns:
-            resp => dict
+        Returns: AsyncRequest
         """
-        await self._request(HttpMethod.PUT, url, data=data, timeout=timeout, **kwargs)
-        return self._parse_response(resp_fmt)
+        return AsyncRequest(self, HttpMethod.GET, url, data=data, timeout=timeout, **kwargs)
 
-    async def delete(self, url: str, data: dict = None, timeout: timedelta = None, resp_fmt: RespFmt = None, **kwargs):
+    async def delete(self, url: str, data: dict = None, timeout: timedelta = None, **kwargs):
         """DELETE请求
 
         Args:
             url: 请求URL
             data: 请求体数据字典
             timeout: 请求超时时间,单位秒
-            resp_fmt: 响应格式，默认None 使用实例对象的 default_resp_fmt
 
-        Returns:
-            resp => dict
+        Returns: AsyncRequest
         """
-        await self._request(HttpMethod.DELETE, url, data=data, timeout=timeout, **kwargs)
-        return self._parse_response(resp_fmt)
+        return AsyncRequest(self, HttpMethod.GET, url, data=data, timeout=timeout, **kwargs)
 
 
 class HttpClient:
     """同步HTTP客户端
 
     通过request封装，实现了常见的HTTP方法,支持设置超时时间、请求参数等，链式调用
```

### Comparing `hui-tools-0.4.1/py_tools/connections/oss/minio_client.py` & `hui-tools-0.4.2/py_tools/connections/oss/minio_client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/data_models/unit.py` & `hui-tools-0.4.2/py_tools/data_models/unit.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/decorators/base.py` & `hui-tools-0.4.2/py_tools/decorators/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/decorators/cache.py` & `hui-tools-0.4.2/py_tools/decorators/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import functools
 import hashlib
 import json
 from datetime import timedelta
 from typing import Union
 
 import cacheout
+import memcache
 from pydantic import BaseModel, Field
 from redis import Redis
 from redis import asyncio as aioredis
 
 from py_tools import constants
 
 
@@ -74,14 +75,23 @@
     def set(self, key, value, ttl):
         self.cache_client.set(key=key, value=value, ttl=ttl)
 
 
 MEMORY_PROXY = MemoryCacheProxy(cache_client=cacheout.Cache(maxsize=1024))
 
 
+class MemcacheCacheProxy(BaseCacheProxy):
+
+    def __init__(self, cache_client: memcache.Client):
+        super().__init__(cache_client)
+
+    def set(self, key, value, ttl):
+        self.cache_client.set(key, value, time=ttl)
+
+
 def cache_json(
     cache_proxy: BaseCacheProxy = MEMORY_PROXY,
     key_prefix: str = constants.CACHE_KEY_PREFIX,
     ttl: Union[int, timedelta] = 60,
 ):
     """
     缓存装饰器（仅支持缓存能够json序列化的数据）
@@ -96,15 +106,15 @@
     if isinstance(ttl, timedelta):
         ttl = int(ttl.total_seconds())
 
     def _cache(func):
         def _gen_key(*args, **kwargs):
             """生成缓存的key"""
 
-            # 没有传递key信息，根据函数信息与参数生成
+            # 根据函数信息与参数生成
             # key => 函数所在模块:函数名:函数位置参数:函数关键字参数 进行hash
             param_args_str = ",".join([str(arg) for arg in args])
             param_kwargs_str = ",".join(sorted([f"{k}:{v}" for k, v in kwargs.items()]))
             hash_str = f"{func.__module__}:{func.__name__}:{param_args_str}:{param_kwargs_str}"
             hash_ret = hashlib.sha256(hash_str.encode()).hexdigest()
 
             # 根据哈希结果生成key 默认前缀:函数所在模块:函数名:hash
```

### Comparing `hui-tools-0.4.1/py_tools/enums/base.py` & `hui-tools-0.4.2/py_tools/enums/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/enums/error.py` & `hui-tools-0.4.2/py_tools/enums/error.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/enums/feishu.py` & `hui-tools-0.4.2/py_tools/enums/feishu.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/enums/time.py` & `hui-tools-0.4.2/py_tools/enums/time.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/exceptions/base.py` & `hui-tools-0.4.2/py_tools/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/meta_cls/base.py` & `hui-tools-0.4.2/py_tools/meta_cls/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/utils/aio.py` & `hui-tools-0.4.2/py_tools/utils/aio.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/utils/excel.py` & `hui-tools-0.4.2/py_tools/utils/excel.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/utils/func.py` & `hui-tools-0.4.2/py_tools/utils/func.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/utils/project_templates/make_pro.py` & `hui-tools-0.4.2/py_tools/utils/project_templates/make_pro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 # @Author: Hui
 # @File: project_template.py
 # @Desc: { 项目模板工具模块 }
 # @Date: 2024/04/26 17:46
-import os
 import argparse
+import os
 import shutil
+
 from loguru import logger
 
 template_dir = os.path.dirname(__file__)
 py_template_dir = os.path.join(template_dir, "python_project")
 
 
 def gen_py_project(project_name):
@@ -56,25 +57,25 @@
 
 def make_project_java(args):
     print(f"Generating Java project [{args.project_name}] structure...")
     # Add code to generate Java project structure
 
 
 def make_project():
-    parser = argparse.ArgumentParser(description='Generate project structure.')
-    subparsers = parser.add_subparsers(dest='subcommand')
+    parser = argparse.ArgumentParser(description="Generate project structure.")
+    subparsers = parser.add_subparsers(dest="subcommand")
 
-    project_parser = subparsers.add_parser('make_project')
-    project_parser.add_argument('project_name', help='Name of the project')
-    project_parser.add_argument('--python', action='store_true', help='Generate Python project structure')
-    project_parser.add_argument('--java', action='store_true', help='Generate Java project structure')
+    project_parser = subparsers.add_parser("make_project")
+    project_parser.add_argument("project_name", help="Name of the project")
+    project_parser.add_argument("--python", action="store_true", help="Generate Python project structure")
+    project_parser.add_argument("--java", action="store_true", help="Generate Java project structure")
 
     args = parser.parse_args()
 
-    if args.subcommand == 'make_project':
+    if args.subcommand == "make_project":
         if args.python:
             make_project_python(args)
         elif args.java:
             make_project_java(args)
         else:
             make_project_python(args)
     else:
```

### Comparing `hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/__init__.py` & `hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/dao/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from py_tools.connections.db.mysql import DBManager, SQLAlchemyManager
-
 from src import settings
 from src.dao.redis import RedisManager
 
+from py_tools.connections.db.mysql import DBManager, SQLAlchemyManager
+
 
 async def init_orm():
     """初始化mysql的ORM"""
     db_client = SQLAlchemyManager(
         host=settings.mysql_host,
         port=settings.mysql_port,
         user=settings.mysql_user,
```

### Comparing `hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/log_setting.py` & `hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/settings/log_setting.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/log_util.py` & `hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/utils/log_util.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from py_tools.logging import logger
-
 from src.utils import context_util
 
+from py_tools.logging import logger
+
 
 def _logger_filter(record):
     """日志过滤器补充request_id或trace_id"""
     req_id = context_util.REQUEST_ID.get()
     trace_id = context_util.TRACE_ID.get()
 
     trace_msg = f"{req_id} | {trace_id}"
```

### Comparing `hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/trace_util.py` & `hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/utils/trace_util.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/web.py` & `hui-tools-0.4.2/py_tools/utils/project_templates/python_project/src/utils/web.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/utils/time.py` & `hui-tools-0.4.2/py_tools/utils/time.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/py_tools/utils/tree.py` & `hui-tools-0.4.2/py_tools/utils/tree.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.1/setup.py` & `hui-tools-0.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 # @Author: Hui
-# @Desc: { 时间工具类模块 }
+# @Desc: { pypi打包模块 }
 # @Date: 2023/9/04 19:59
 import operator
 from functools import reduce
 
 from setuptools import find_packages, setup
 
 
 class PKGManager:
     name = "hui-tools"
-    version = "0.4.1"
+    version = "0.4.2"
     author = "hui"
     author_email = "huidbk@163.com"
 
     @classmethod
     def get_pkg_desc(cls):
         """获取包描述"""
         with open("README.md", "r") as f:
             long_description = f.read()
         return long_description
 
     @classmethod
     def get_install_requires(cls):
         """获取必须安装依赖"""
-        requires = ["loguru>=0.7.0,<0.8", "pydantic>=2.1.1,<3", "asgiref==3.8.1"]
+        requires = [
+            "loguru>=0.7.0,<0.8",
+            "pydantic>=2.1.1,<3",
+            "asgiref==3.8.1",
+            "python-dateutil==2.8.2",
+            "requests==2.31.0",
+            "aiohttp==3.9.5",
+            "cacheout==0.14.1",
+        ]
         return requires
 
     @classmethod
     def get_extras_require(cls):
         """
         可选的依赖
         """
         extras_require = {
             "db-orm": ["sqlalchemy[asyncio]==2.0.20", "aiomysql==0.2.0"],
             "db-redis": ["redis>=4.5.4"],
+            "cache-proxy": ["redis>=4.5.4", "python-memcached==1.62", "cacheout==0.14.1"],
             "minio": ["minio==7.1.17"],
-            "chatbot": ["requests==2.31.0", "cacheout==0.14.1"],
-            "http-client": ["httpx==0.24.1", "requests==2.31.0"],
-            "time-tools": ["python-dateutil==2.8.2"],
             "excel-tools": ["pandas==1.3.5", "openpyxl==3.0.10"],
         }
 
         extras_require["all"] = list(set(reduce(operator.add, [cls.get_install_requires(), *extras_require.values()])))
         return extras_require
 
 
@@ -62,19 +68,15 @@
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
         extras_require=PKGManager.get_extras_require(),
         python_requires=">=3.7",
-        entry_points={
-            'console_scripts': [
-                'py_tools = py_tools.utils.project_templates:make_project'
-            ]
-        },
+        entry_points={"console_scripts": ["py_tools = py_tools.utils.project_templates:make_project"]},
         include_package_data=True,
     )
 
 
 if __name__ == "__main__":
     # python3 setup.py sdist bdist_wheel
     # twine upload --repository testpypi dist/*
```


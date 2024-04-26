# Comparing `tmp/hui-tools-0.4.0.tar.gz` & `tmp/hui-tools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hui-tools-0.4.0.tar", last modified: Wed Apr 24 10:47:19 2024, max compression
+gzip compressed data, was "hui-tools-0.4.1.tar", last modified: Fri Apr 26 13:58:46 2024, max compression
```

## Comparing `hui-tools-0.4.0.tar` & `hui-tools-0.4.1.tar`

### file list

```diff
@@ -1,76 +1,128 @@
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.314090 hui-tools-0.4.0/
--rw-r--r--   0 liuminhui   (501) staff       (20)    11357 2023-07-29 10:14:17.000000 hui-tools-0.4.0/LICENSE
--rw-r--r--   0 liuminhui   (501) staff       (20)    17724 2024-04-24 10:47:19.313742 hui-tools-0.4.0/PKG-INFO
--rw-r--r--   0 liuminhui   (501) staff       (20)    15809 2024-04-15 11:39:36.000000 hui-tools-0.4.0/README.md
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.301820 hui-tools-0.4.0/hui_tools.egg-info/
--rw-r--r--   0 liuminhui   (501) staff       (20)    17724 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/PKG-INFO
--rw-r--r--   0 liuminhui   (501) staff       (20)     1594 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/SOURCES.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/dependency_links.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)      562 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/requires.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)       15 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/top_level.txt
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.302026 hui-tools-0.4.0/py_tools/
--rw-r--r--   0 liuminhui   (501) staff       (20)        1 2023-09-04 08:25:07.000000 hui-tools-0.4.0/py_tools/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.303373 hui-tools-0.4.0/py_tools/chatbot/
--rw-r--r--   0 liuminhui   (501) staff       (20)      128 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/chatbot/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)    11243 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/chatbot/app_server.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     5238 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/chatbot/chatbot.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2385 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/chatbot/factory.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.303550 hui-tools-0.4.0/py_tools/connections/
--rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.303909 hui-tools-0.4.0/py_tools/connections/db/
--rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/db/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.304868 hui-tools-0.4.0/py_tools/connections/db/mysql/
--rw-r--r--   0 liuminhui   (501) staff       (20)      215 2024-03-28 15:06:17.000000 hui-tools-0.4.0/py_tools/connections/db/mysql/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)    20121 2024-04-17 03:58:06.000000 hui-tools-0.4.0/py_tools/connections/db/mysql/client.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1722 2024-04-17 03:58:06.000000 hui-tools-0.4.0/py_tools/connections/db/mysql/orm_model.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2581 2024-04-24 02:13:05.000000 hui-tools-0.4.0/py_tools/connections/db/redis_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.305331 hui-tools-0.4.0/py_tools/connections/http/
--rw-r--r--   0 liuminhui   (501) staff       (20)      158 2023-08-10 03:40:34.000000 hui-tools-0.4.0/py_tools/connections/http/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     8809 2023-09-28 06:51:00.000000 hui-tools-0.4.0/py_tools/connections/http/client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.306038 hui-tools-0.4.0/py_tools/connections/mq/
--rw-r--r--   0 liuminhui   (501) staff       (20)      185 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/mq/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      184 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/mq/kafka_client.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      187 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/mq/rabbitmq_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.306458 hui-tools-0.4.0/py_tools/connections/oss/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2024-03-28 01:23:21.000000 hui-tools-0.4.0/py_tools/connections/oss/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1955 2024-03-28 01:23:21.000000 hui-tools-0.4.0/py_tools/connections/oss/minio_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.306690 hui-tools-0.4.0/py_tools/constants/
--rw-r--r--   0 liuminhui   (501) staff       (20)      171 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/constants/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.307244 hui-tools-0.4.0/py_tools/data_models/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/data_models/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      270 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/data_models/time.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2674 2024-04-24 04:49:33.000000 hui-tools-0.4.0/py_tools/data_models/unit.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.307763 hui-tools-0.4.0/py_tools/decorators/
--rw-r--r--   0 liuminhui   (501) staff       (20)      213 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/decorators/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     6380 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/decorators/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     4831 2024-04-24 02:14:22.000000 hui-tools-0.4.0/py_tools/decorators/cache.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.309430 hui-tools-0.4.0/py_tools/enums/
--rw-r--r--   0 liuminhui   (501) staff       (20)      334 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/enums/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2304 2024-04-24 03:43:33.000000 hui-tools-0.4.0/py_tools/enums/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1234 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/enums/error.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/enums/feishu.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      452 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/enums/http.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      486 2024-04-24 03:43:33.000000 hui-tools-0.4.0/py_tools/enums/pub_biz.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-09-09 06:12:03.000000 hui-tools-0.4.0/py_tools/enums/time.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.309841 hui-tools-0.4.0/py_tools/exceptions/
--rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/exceptions/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1141 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/exceptions/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.310107 hui-tools-0.4.0/py_tools/logging/
--rw-r--r--   0 liuminhui   (501) staff       (20)       26 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/logging/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.310519 hui-tools-0.4.0/py_tools/meta_cls/
--rw-r--r--   0 liuminhui   (501) staff       (20)       35 2023-09-04 07:12:03.000000 hui-tools-0.4.0/py_tools/meta_cls/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      963 2023-09-09 06:35:40.000000 hui-tools-0.4.0/py_tools/meta_cls/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.312122 hui-tools-0.4.0/py_tools/utils/
--rw-r--r--   0 liuminhui   (501) staff       (20)      166 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/utils/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1067 2024-04-24 10:35:38.000000 hui-tools-0.4.0/py_tools/utils/aio.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/utils/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     5992 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/utils/excel.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      951 2024-04-24 03:52:42.000000 hui-tools-0.4.0/py_tools/utils/func.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/utils/mask.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      179 2023-09-09 16:16:35.000000 hui-tools-0.4.0/py_tools/utils/serializer.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     6538 2024-04-24 02:48:33.000000 hui-tools-0.4.0/py_tools/utils/time.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     4592 2024-04-24 03:58:59.000000 hui-tools-0.4.0/py_tools/utils/tree.py
--rw-r--r--   0 liuminhui   (501) staff       (20)       38 2024-04-24 10:47:19.314146 hui-tools-0.4.0/setup.cfg
--rw-r--r--   0 liuminhui   (501) staff       (20)     2307 2024-04-24 10:45:44.000000 hui-tools-0.4.0/setup.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.312263 hui-tools-0.4.0/tests/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.0/tests/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.227215 hui-tools-0.4.1/
+-rw-r--r--   0 liuminhui   (501) staff       (20)    11357 2023-07-29 10:14:17.000000 hui-tools-0.4.1/LICENSE
+-rw-r--r--   0 liuminhui   (501) staff       (20)       53 2024-04-26 13:50:18.000000 hui-tools-0.4.1/MANIFEST.in
+-rw-r--r--   0 liuminhui   (501) staff       (20)    17724 2024-04-26 13:58:46.226945 hui-tools-0.4.1/PKG-INFO
+-rw-r--r--   0 liuminhui   (501) staff       (20)    15809 2024-04-15 11:39:36.000000 hui-tools-0.4.1/README.md
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.205510 hui-tools-0.4.1/hui_tools.egg-info/
+-rw-r--r--   0 liuminhui   (501) staff       (20)    17724 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/PKG-INFO
+-rw-r--r--   0 liuminhui   (501) staff       (20)     3866 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)       75 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/entry_points.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)      562 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/requires.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)       15 2024-04-26 13:58:46.000000 hui-tools-0.4.1/hui_tools.egg-info/top_level.txt
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.205647 hui-tools-0.4.1/py_tools/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2023-09-04 08:25:07.000000 hui-tools-0.4.1/py_tools/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.206787 hui-tools-0.4.1/py_tools/chatbot/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      128 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/chatbot/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)    11243 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/chatbot/app_server.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     5238 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/chatbot/chatbot.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2385 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/chatbot/factory.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.207074 hui-tools-0.4.1/py_tools/connections/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.207559 hui-tools-0.4.1/py_tools/connections/db/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/db/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.209129 hui-tools-0.4.1/py_tools/connections/db/mysql/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      215 2024-03-28 15:06:17.000000 hui-tools-0.4.1/py_tools/connections/db/mysql/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)    20121 2024-04-17 03:58:06.000000 hui-tools-0.4.1/py_tools/connections/db/mysql/client.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1722 2024-04-17 03:58:06.000000 hui-tools-0.4.1/py_tools/connections/db/mysql/orm_model.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2581 2024-04-24 02:13:05.000000 hui-tools-0.4.1/py_tools/connections/db/redis_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.209638 hui-tools-0.4.1/py_tools/connections/http/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      158 2023-08-10 03:40:34.000000 hui-tools-0.4.1/py_tools/connections/http/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     8809 2023-09-28 06:51:00.000000 hui-tools-0.4.1/py_tools/connections/http/client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.210200 hui-tools-0.4.1/py_tools/connections/mq/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      185 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/mq/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      184 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/mq/kafka_client.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      187 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/connections/mq/rabbitmq_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.210581 hui-tools-0.4.1/py_tools/connections/oss/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2024-03-28 01:23:21.000000 hui-tools-0.4.1/py_tools/connections/oss/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1955 2024-03-28 01:23:21.000000 hui-tools-0.4.1/py_tools/connections/oss/minio_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.210812 hui-tools-0.4.1/py_tools/constants/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      171 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/constants/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.211376 hui-tools-0.4.1/py_tools/data_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/data_models/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      270 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/data_models/time.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2674 2024-04-24 04:49:33.000000 hui-tools-0.4.1/py_tools/data_models/unit.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.212145 hui-tools-0.4.1/py_tools/decorators/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      213 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/decorators/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     6380 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/decorators/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     4831 2024-04-24 02:14:22.000000 hui-tools-0.4.1/py_tools/decorators/cache.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.214294 hui-tools-0.4.1/py_tools/enums/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      334 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/enums/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2304 2024-04-24 03:43:33.000000 hui-tools-0.4.1/py_tools/enums/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1234 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/enums/error.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/enums/feishu.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      452 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/enums/http.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      486 2024-04-24 03:43:33.000000 hui-tools-0.4.1/py_tools/enums/pub_biz.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-09-09 06:12:03.000000 hui-tools-0.4.1/py_tools/enums/time.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.214662 hui-tools-0.4.1/py_tools/exceptions/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/exceptions/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1141 2023-09-09 16:15:14.000000 hui-tools-0.4.1/py_tools/exceptions/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.214877 hui-tools-0.4.1/py_tools/logging/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       26 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/logging/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.215268 hui-tools-0.4.1/py_tools/meta_cls/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       35 2023-09-04 07:12:03.000000 hui-tools-0.4.1/py_tools/meta_cls/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      963 2023-09-09 06:35:40.000000 hui-tools-0.4.1/py_tools/meta_cls/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.217872 hui-tools-0.4.1/py_tools/utils/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      166 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/utils/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1067 2024-04-24 11:01:10.000000 hui-tools-0.4.1/py_tools/utils/aio.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/utils/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     5992 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/utils/excel.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      951 2024-04-24 03:52:42.000000 hui-tools-0.4.1/py_tools/utils/func.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.1/py_tools/utils/mask.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.218572 hui-tools-0.4.1/py_tools/utils/project_templates/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       35 2024-04-26 11:46:23.000000 hui-tools-0.4.1/py_tools/utils/project_templates/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2770 2024-04-26 12:24:15.000000 hui-tools-0.4.1/py_tools/utils/project_templates/make_pro.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.202352 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.218866 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.218978 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/constants/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/constants/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.219282 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      745 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.202697 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.219684 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/manage/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/manage/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      150 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/manage/user.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.220327 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/table/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       28 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/table/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      446 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/orm/table/user.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.220996 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/redis/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       66 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/redis/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       81 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/redis/cache_info.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      132 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/dao/redis/client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.221186 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.221454 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/api_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/api_models/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.221677 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/logic_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/data_models/logic_models/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.222082 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/enums/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       33 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/enums/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      369 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/enums/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.222288 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/handlers/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/handlers/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.222498 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/middlewares/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/middlewares/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.222761 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/routes/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      194 2024-04-26 13:52:42.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/routes/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2024-04-26 11:46:23.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/server.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.223091 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/services/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        0 2023-09-05 15:16:08.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/services/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       77 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/services/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.224165 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      399 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       75 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/base_setting.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      235 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/db_setting.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1702 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/settings/log_setting.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.225269 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       34 2023-10-30 08:27:36.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      239 2024-04-26 11:15:57.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/context_util.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      721 2024-04-26 11:27:24.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/log_util.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1153 2023-10-30 08:27:36.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/trace_util.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      919 2024-04-26 11:46:23.000000 hui-tools-0.4.1/py_tools/utils/project_templates/python_project/src/utils/web.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      179 2023-09-09 16:16:35.000000 hui-tools-0.4.1/py_tools/utils/serializer.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     6538 2024-04-24 02:48:33.000000 hui-tools-0.4.1/py_tools/utils/time.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     4592 2024-04-24 03:58:59.000000 hui-tools-0.4.1/py_tools/utils/tree.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       38 2024-04-26 13:58:46.227285 hui-tools-0.4.1/setup.cfg
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2498 2024-04-26 13:58:01.000000 hui-tools-0.4.1/setup.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-26 13:58:46.225476 hui-tools-0.4.1/tests/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.1/tests/__init__.py
```

### Comparing `hui-tools-0.4.0/LICENSE` & `hui-tools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/PKG-INFO` & `hui-tools-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hui-tools
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/HuiDBK/py-tools
 Author: hui
 Author-email: huidbk@163.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -29,27 +29,27 @@
 Requires-Dist: requests==2.31.0; extra == "http-client"
 Provides-Extra: time-tools
 Requires-Dist: python-dateutil==2.8.2; extra == "time-tools"
 Provides-Extra: excel-tools
 Requires-Dist: pandas==1.3.5; extra == "excel-tools"
 Requires-Dist: openpyxl==3.0.10; extra == "excel-tools"
 Provides-Extra: all
-Requires-Dist: cacheout==0.14.1; extra == "all"
-Requires-Dist: asgiref==3.8.1; extra == "all"
-Requires-Dist: minio==7.1.17; extra == "all"
-Requires-Dist: python-dateutil==2.8.2; extra == "all"
-Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
 Requires-Dist: openpyxl==3.0.10; extra == "all"
-Requires-Dist: redis>=4.5.4; extra == "all"
+Requires-Dist: requests==2.31.0; extra == "all"
 Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "all"
-Requires-Dist: httpx==0.24.1; extra == "all"
-Requires-Dist: pandas==1.3.5; extra == "all"
 Requires-Dist: aiomysql==0.2.0; extra == "all"
+Requires-Dist: pandas==1.3.5; extra == "all"
+Requires-Dist: minio==7.1.17; extra == "all"
+Requires-Dist: cacheout==0.14.1; extra == "all"
+Requires-Dist: httpx==0.24.1; extra == "all"
 Requires-Dist: pydantic<3,>=2.1.1; extra == "all"
-Requires-Dist: requests==2.31.0; extra == "all"
+Requires-Dist: python-dateutil==2.8.2; extra == "all"
+Requires-Dist: asgiref==3.8.1; extra == "all"
+Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
+Requires-Dist: redis>=4.5.4; extra == "all"
 
 # Py-Tools
 
 > Py-Tools 是一个实用的 Python 工具集和可复用组件库，旨在简化常见任务，提高 Python 项目的开发效率。
 > 
 > 设计细节请移步到掘金查看：https://juejin.cn/column/7131286129713610766
```

### Comparing `hui-tools-0.4.0/README.md` & `hui-tools-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/hui_tools.egg-info/PKG-INFO` & `hui-tools-0.4.1/hui_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hui-tools
-Version: 0.4.0
+Version: 0.4.1
 Home-page: https://github.com/HuiDBK/py-tools
 Author: hui
 Author-email: huidbk@163.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -29,27 +29,27 @@
 Requires-Dist: requests==2.31.0; extra == "http-client"
 Provides-Extra: time-tools
 Requires-Dist: python-dateutil==2.8.2; extra == "time-tools"
 Provides-Extra: excel-tools
 Requires-Dist: pandas==1.3.5; extra == "excel-tools"
 Requires-Dist: openpyxl==3.0.10; extra == "excel-tools"
 Provides-Extra: all
-Requires-Dist: cacheout==0.14.1; extra == "all"
-Requires-Dist: asgiref==3.8.1; extra == "all"
-Requires-Dist: minio==7.1.17; extra == "all"
-Requires-Dist: python-dateutil==2.8.2; extra == "all"
-Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
 Requires-Dist: openpyxl==3.0.10; extra == "all"
-Requires-Dist: redis>=4.5.4; extra == "all"
+Requires-Dist: requests==2.31.0; extra == "all"
 Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "all"
-Requires-Dist: httpx==0.24.1; extra == "all"
-Requires-Dist: pandas==1.3.5; extra == "all"
 Requires-Dist: aiomysql==0.2.0; extra == "all"
+Requires-Dist: pandas==1.3.5; extra == "all"
+Requires-Dist: minio==7.1.17; extra == "all"
+Requires-Dist: cacheout==0.14.1; extra == "all"
+Requires-Dist: httpx==0.24.1; extra == "all"
 Requires-Dist: pydantic<3,>=2.1.1; extra == "all"
-Requires-Dist: requests==2.31.0; extra == "all"
+Requires-Dist: python-dateutil==2.8.2; extra == "all"
+Requires-Dist: asgiref==3.8.1; extra == "all"
+Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
+Requires-Dist: redis>=4.5.4; extra == "all"
 
 # Py-Tools
 
 > Py-Tools 是一个实用的 Python 工具集和可复用组件库，旨在简化常见任务，提高 Python 项目的开发效率。
 > 
 > 设计细节请移步到掘金查看：https://juejin.cn/column/7131286129713610766
```

### Comparing `hui-tools-0.4.0/hui_tools.egg-info/requires.txt` & `hui-tools-0.4.1/hui_tools.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 loguru<0.8,>=0.7.0
 pydantic<3,>=2.1.1
 asgiref==3.8.1
 
 [all]
-cacheout==0.14.1
-asgiref==3.8.1
-minio==7.1.17
-python-dateutil==2.8.2
-loguru<0.8,>=0.7.0
 openpyxl==3.0.10
-redis>=4.5.4
+requests==2.31.0
 sqlalchemy[asyncio]==2.0.20
-httpx==0.24.1
-pandas==1.3.5
 aiomysql==0.2.0
+pandas==1.3.5
+minio==7.1.17
+cacheout==0.14.1
+httpx==0.24.1
 pydantic<3,>=2.1.1
-requests==2.31.0
+python-dateutil==2.8.2
+asgiref==3.8.1
+loguru<0.8,>=0.7.0
+redis>=4.5.4
 
 [chatbot]
 requests==2.31.0
 cacheout==0.14.1
 
 [db-orm]
 sqlalchemy[asyncio]==2.0.20
```

### Comparing `hui-tools-0.4.0/py_tools/chatbot/app_server.py` & `hui-tools-0.4.1/py_tools/chatbot/app_server.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/chatbot/chatbot.py` & `hui-tools-0.4.1/py_tools/chatbot/chatbot.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/chatbot/factory.py` & `hui-tools-0.4.1/py_tools/chatbot/factory.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/connections/db/mysql/client.py` & `hui-tools-0.4.1/py_tools/connections/db/mysql/client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/connections/db/mysql/orm_model.py` & `hui-tools-0.4.1/py_tools/connections/db/mysql/orm_model.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/connections/db/redis_client.py` & `hui-tools-0.4.1/py_tools/connections/db/redis_client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/connections/http/client.py` & `hui-tools-0.4.1/py_tools/connections/http/client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/connections/oss/minio_client.py` & `hui-tools-0.4.1/py_tools/connections/oss/minio_client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/data_models/unit.py` & `hui-tools-0.4.1/py_tools/data_models/unit.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/decorators/base.py` & `hui-tools-0.4.1/py_tools/decorators/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/decorators/cache.py` & `hui-tools-0.4.1/py_tools/decorators/cache.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/enums/base.py` & `hui-tools-0.4.1/py_tools/enums/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/enums/error.py` & `hui-tools-0.4.1/py_tools/enums/error.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/enums/feishu.py` & `hui-tools-0.4.1/py_tools/enums/feishu.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/enums/time.py` & `hui-tools-0.4.1/py_tools/enums/time.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/exceptions/base.py` & `hui-tools-0.4.1/py_tools/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/meta_cls/base.py` & `hui-tools-0.4.1/py_tools/meta_cls/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/utils/aio.py` & `hui-tools-0.4.1/py_tools/utils/aio.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/utils/excel.py` & `hui-tools-0.4.1/py_tools/utils/excel.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/utils/func.py` & `hui-tools-0.4.1/py_tools/utils/func.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/utils/time.py` & `hui-tools-0.4.1/py_tools/utils/time.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/py_tools/utils/tree.py` & `hui-tools-0.4.1/py_tools/utils/tree.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.4.0/setup.py` & `hui-tools-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from functools import reduce
 
 from setuptools import find_packages, setup
 
 
 class PKGManager:
     name = "hui-tools"
-    version = "0.4.0"
+    version = "0.4.1"
     author = "hui"
     author_email = "huidbk@163.com"
 
     @classmethod
     def get_pkg_desc(cls):
         """获取包描述"""
         with open("README.md", "r") as f:
@@ -62,14 +62,20 @@
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
         extras_require=PKGManager.get_extras_require(),
         python_requires=">=3.7",
+        entry_points={
+            'console_scripts': [
+                'py_tools = py_tools.utils.project_templates:make_project'
+            ]
+        },
+        include_package_data=True,
     )
 
 
 if __name__ == "__main__":
     # python3 setup.py sdist bdist_wheel
     # twine upload --repository testpypi dist/*
     # twine upload dist/*
```


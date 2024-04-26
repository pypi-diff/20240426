# Comparing `tmp/air_drf_relation-0.6.0.tar.gz` & `tmp/air_drf_relation-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air_drf_relation-0.6.0.tar", last modified: Thu Jun 22 20:55:57 2023, max compression
+gzip compressed data, was "air_drf_relation-0.6.1.tar", last modified: Fri Apr 26 07:37:12 2024, max compression
```

## Comparing `air_drf_relation-0.6.0.tar` & `air_drf_relation-0.6.1.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.194984 air_drf_relation-0.6.0/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1074 2021-06-27 18:03:44.000000 air_drf_relation-0.6.0/LICENSE
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       87 2021-06-27 19:16:11.000000 air_drf_relation-0.6.0/MANIFEST.in
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-06-22 20:55:57.195193 air_drf_relation-0.6.0/PKG-INFO
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     6483 2022-05-26 10:52:59.000000 air_drf_relation-0.6.0/README.md
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.182767 air_drf_relation-0.6.0/air_drf_relation/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      346 2022-05-26 10:45:07.000000 air_drf_relation-0.6.0/air_drf_relation/__init__.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.186832 air_drf_relation-0.6.0/air_drf_relation/__pycache__/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      492 2022-05-26 10:48:51.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1452 2022-05-04 08:27:13.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/context_builder.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-04 08:28:39.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/decorators.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     3466 2022-03-03 07:13:47.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2441 2022-05-26 11:22:49.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/fields.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1236 2022-05-04 08:27:13.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/filters.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1703 2023-06-22 20:52:06.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/model_fields.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     5012 2023-02-11 11:33:06.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     3021 2023-02-08 21:41:02.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)    11142 2023-06-22 20:21:50.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/serializers.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      332 2022-05-26 10:48:51.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1293 2023-06-22 20:13:08.000000 air_drf_relation-0.6.0/air_drf_relation/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      832 2022-05-04 08:26:21.000000 air_drf_relation-0.6.0/air_drf_relation/context_builder.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      696 2022-05-04 07:31:58.000000 air_drf_relation-0.6.0/air_drf_relation/decorators.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     4316 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/air_drf_relation/extra_kwargs.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1855 2022-05-26 11:22:46.000000 air_drf_relation-0.6.0/air_drf_relation/fields.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      690 2022-05-04 07:35:13.000000 air_drf_relation-0.6.0/air_drf_relation/filters.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1168 2023-06-22 20:52:03.000000 air_drf_relation-0.6.0/air_drf_relation/model_fields.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     5763 2023-02-11 11:19:46.000000 air_drf_relation-0.6.0/air_drf_relation/preload_objects_manager.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     3103 2023-02-08 21:41:00.000000 air_drf_relation-0.6.0/air_drf_relation/queryset_optimization.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)    11015 2023-06-22 20:21:49.000000 air_drf_relation-0.6.0/air_drf_relation/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      240 2022-05-26 10:47:07.000000 air_drf_relation-0.6.0/air_drf_relation/settings.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      873 2023-04-25 22:09:43.000000 air_drf_relation-0.6.0/air_drf_relation/utils.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.183951 air_drf_relation-0.6.0/air_drf_relation.egg-info/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2023-06-22 20:55:57.000000 air_drf_relation-0.6.0/air_drf_relation.egg-info/PKG-INFO
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2343 2023-06-22 20:55:57.000000 air_drf_relation-0.6.0/air_drf_relation.egg-info/SOURCES.txt
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-06-22 20:55:57.000000 air_drf_relation-0.6.0/air_drf_relation.egg-info/dependency_links.txt
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-02-08 22:24:16.000000 air_drf_relation-0.6.0/air_drf_relation.egg-info/not-zip-safe
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      109 2023-06-22 20:55:57.000000 air_drf_relation-0.6.0/air_drf_relation.egg-info/requires.txt
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       50 2023-06-22 20:55:57.000000 air_drf_relation-0.6.0/air_drf_relation.egg-info/top_level.txt
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.188099 air_drf_relation-0.6.0/device/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      144 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.188530 air_drf_relation-0.6.0/device/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      698 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      371 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/migrations/0002_alter_device_code.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      251 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      888 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     2505 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/device/views.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.190142 air_drf_relation-0.6.0/film/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.6.0/film/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2023-02-08 21:16:41.000000 air_drf_relation-0.6.0/film/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2023-02-08 21:16:41.000000 air_drf_relation-0.6.0/film/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.190584 air_drf_relation-0.6.0/film/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1093 2023-02-08 22:30:35.000000 air_drf_relation-0.6.0/film/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.6.0/film/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      586 2023-06-22 20:50:27.000000 air_drf_relation-0.6.0/film/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      877 2023-06-22 20:50:37.000000 air_drf_relation-0.6.0/film/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1813 2023-06-22 20:33:44.000000 air_drf_relation-0.6.0/film/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2023-02-08 23:17:50.000000 air_drf_relation-0.6.0/film/urls.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      217 2023-02-08 23:17:39.000000 air_drf_relation-0.6.0/film/views.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       73 2023-06-22 20:55:57.195660 air_drf_relation-0.6.0/setup.cfg
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      980 2023-06-22 20:55:02.000000 air_drf_relation-0.6.0/setup.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.191881 air_drf_relation-0.6.0/table/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.6.0/table/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.6.0/table/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      142 2022-05-13 12:51:44.000000 air_drf_relation-0.6.0/table/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.192903 air_drf_relation-0.6.0/table/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-13 12:54:15.000000 air_drf_relation-0.6.0/table/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      417 2022-05-13 12:58:02.000000 air_drf_relation-0.6.0/table/migrations/0002_table_name.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1820 2022-05-13 15:42:11.000000 air_drf_relation-0.6.0/table/migrations/0003_auto_20220513_1542.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      545 2022-05-13 15:43:10.000000 air_drf_relation-0.6.0/table/migrations/0004_material_company.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.6.0/table/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      916 2022-05-13 15:43:05.000000 air_drf_relation-0.6.0/table/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1342 2023-02-11 11:37:09.000000 air_drf_relation-0.6.0/table/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     5277 2023-04-18 14:13:22.000000 air_drf_relation-0.6.0/table/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.6.0/table/views.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.194040 air_drf_relation-0.6.0/task/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/admin.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/apps.py
-drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2023-06-22 20:55:57.194878 air_drf_relation-0.6.0/task/migrations/
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      558 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/migrations/0001_initial.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      387 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/migrations/0002_alter_task_image.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      598 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/migrations/0003_tag.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      512 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/migrations/0004_tag_task.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/migrations/__init__.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      391 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/models.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      462 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/serializers.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)     1346 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/tests.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/urls.py
--rw-r--r--   0 kirillcelisev   (501) staff       (20)      935 2022-03-03 07:12:43.000000 air_drf_relation-0.6.0/task/views.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.273541 air_drf_relation-0.6.1/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1074 2021-06-27 18:03:44.000000 air_drf_relation-0.6.1/LICENSE
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       87 2021-06-27 19:16:11.000000 air_drf_relation-0.6.1/MANIFEST.in
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2024-04-26 07:37:12.273693 air_drf_relation-0.6.1/PKG-INFO
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     6483 2022-05-26 10:52:59.000000 air_drf_relation-0.6.1/README.md
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.260131 air_drf_relation-0.6.1/air_drf_relation/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      346 2022-05-26 10:45:07.000000 air_drf_relation-0.6.1/air_drf_relation/__init__.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.264159 air_drf_relation-0.6.1/air_drf_relation/__pycache__/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      492 2022-05-26 10:48:51.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1452 2022-05-04 08:27:13.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/context_builder.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-04 08:28:39.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/decorators.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     3466 2022-03-03 07:13:47.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     2441 2022-05-26 11:22:49.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/fields.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1236 2022-05-04 08:27:13.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/filters.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1703 2023-06-22 20:52:06.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/model_fields.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     5012 2023-02-11 11:33:06.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     3021 2023-02-08 21:41:02.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)    11142 2023-06-22 20:21:50.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/serializers.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      332 2022-05-26 10:48:51.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1293 2023-06-22 20:13:08.000000 air_drf_relation-0.6.1/air_drf_relation/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      832 2022-05-04 08:26:21.000000 air_drf_relation-0.6.1/air_drf_relation/context_builder.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      742 2024-04-26 07:36:08.000000 air_drf_relation-0.6.1/air_drf_relation/decorators.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      709 2024-04-26 07:36:08.000000 air_drf_relation-0.6.1/air_drf_relation/encoders.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     4316 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/air_drf_relation/extra_kwargs.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1855 2022-05-26 11:22:46.000000 air_drf_relation-0.6.1/air_drf_relation/fields.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      690 2022-05-04 07:35:13.000000 air_drf_relation-0.6.1/air_drf_relation/filters.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1168 2023-06-22 20:52:03.000000 air_drf_relation-0.6.1/air_drf_relation/model_fields.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     5763 2023-02-11 11:19:46.000000 air_drf_relation-0.6.1/air_drf_relation/preload_objects_manager.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     3103 2023-02-08 21:41:00.000000 air_drf_relation-0.6.1/air_drf_relation/queryset_optimization.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)    11015 2023-06-22 20:21:49.000000 air_drf_relation-0.6.1/air_drf_relation/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      240 2022-05-26 10:47:07.000000 air_drf_relation-0.6.1/air_drf_relation/settings.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      873 2023-04-25 22:09:43.000000 air_drf_relation-0.6.1/air_drf_relation/utils.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.261100 air_drf_relation-0.6.1/air_drf_relation.egg-info/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     8696 2024-04-26 07:37:12.000000 air_drf_relation-0.6.1/air_drf_relation.egg-info/PKG-INFO
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     2372 2024-04-26 07:37:12.000000 air_drf_relation-0.6.1/air_drf_relation.egg-info/SOURCES.txt
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2024-04-26 07:37:12.000000 air_drf_relation-0.6.1/air_drf_relation.egg-info/dependency_links.txt
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        1 2023-02-08 22:24:16.000000 air_drf_relation-0.6.1/air_drf_relation.egg-info/not-zip-safe
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      109 2024-04-26 07:37:12.000000 air_drf_relation-0.6.1/air_drf_relation.egg-info/requires.txt
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       50 2024-04-26 07:37:12.000000 air_drf_relation-0.6.1/air_drf_relation.egg-info/top_level.txt
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.265536 air_drf_relation-0.6.1/device/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      144 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.266030 air_drf_relation-0.6.1/device/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      698 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      371 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/migrations/0002_alter_device_code.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      251 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      888 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     2505 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/device/views.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.267721 air_drf_relation-0.6.1/film/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.6.1/film/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2023-02-08 21:16:41.000000 air_drf_relation-0.6.1/film/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2023-02-08 21:16:41.000000 air_drf_relation-0.6.1/film/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.268220 air_drf_relation-0.6.1/film/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1093 2023-02-08 22:30:35.000000 air_drf_relation-0.6.1/film/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2023-02-08 21:16:41.000000 air_drf_relation-0.6.1/film/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      586 2023-06-22 20:50:27.000000 air_drf_relation-0.6.1/film/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      877 2023-06-22 20:50:37.000000 air_drf_relation-0.6.1/film/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1813 2023-06-22 20:33:44.000000 air_drf_relation-0.6.1/film/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2023-02-08 23:17:50.000000 air_drf_relation-0.6.1/film/urls.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      217 2023-02-08 23:17:39.000000 air_drf_relation-0.6.1/film/views.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       73 2024-04-26 07:37:12.274065 air_drf_relation-0.6.1/setup.cfg
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      980 2024-04-26 07:36:37.000000 air_drf_relation-0.6.1/setup.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.269768 air_drf_relation-0.6.1/table/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.6.1/table/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-05-13 12:51:44.000000 air_drf_relation-0.6.1/table/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      142 2022-05-13 12:51:44.000000 air_drf_relation-0.6.1/table/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.271191 air_drf_relation-0.6.1/table/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      885 2022-05-13 12:54:15.000000 air_drf_relation-0.6.1/table/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      417 2022-05-13 12:58:02.000000 air_drf_relation-0.6.1/table/migrations/0002_table_name.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1820 2022-05-13 15:42:11.000000 air_drf_relation-0.6.1/table/migrations/0003_auto_20220513_1542.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      545 2022-05-13 15:43:10.000000 air_drf_relation-0.6.1/table/migrations/0004_material_company.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-05-13 12:51:44.000000 air_drf_relation-0.6.1/table/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      916 2024-04-26 07:35:55.000000 air_drf_relation-0.6.1/table/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1342 2024-04-26 07:35:55.000000 air_drf_relation-0.6.1/table/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     5277 2024-04-26 07:35:55.000000 air_drf_relation-0.6.1/table/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2024-04-26 07:35:55.000000 air_drf_relation-0.6.1/table/views.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.272518 air_drf_relation-0.6.1/task/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)       63 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/admin.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      140 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/apps.py
+drwxr-xr-x   0 kirillcelisev   (501) staff       (20)        0 2024-04-26 07:37:12.273450 air_drf_relation-0.6.1/task/migrations/
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      558 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/migrations/0001_initial.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      387 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/migrations/0002_alter_task_image.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      598 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/migrations/0003_tag.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      512 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/migrations/0004_tag_task.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)        0 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/migrations/__init__.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      391 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/models.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      462 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/serializers.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)     1346 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/tests.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      163 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/urls.py
+-rw-r--r--   0 kirillcelisev   (501) staff       (20)      935 2022-03-03 07:12:43.000000 air_drf_relation-0.6.1/task/views.py
```

### Comparing `air_drf_relation-0.6.0/LICENSE` & `air_drf_relation-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/PKG-INFO` & `air_drf_relation-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air_drf_relation
-Version: 0.6.0
+Version: 0.6.1
 Summary: Improved interaction with DRF relations.
 Home-page: https://github.com/bubaley/air-drf-relation
 Author: bubaley
 Author-email: bubaley.fu@gmail.com
 License: MIT
 Description: **AIR-DRF-RELATION**
```

### Comparing `air_drf_relation-0.6.0/README.md` & `air_drf_relation-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/context_builder.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/context_builder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/decorators.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/decorators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/extra_kwargs.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/fields.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/fields.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/filters.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/filters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/model_fields.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/model_fields.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/preload_objects_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/queryset_optimization.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/serializers.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/serializers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/__pycache__/utils.cpython-39.pyc` & `air_drf_relation-0.6.1/air_drf_relation/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/context_builder.py` & `air_drf_relation-0.6.1/air_drf_relation/context_builder.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/decorators.py` & `air_drf_relation-0.6.1/air_drf_relation/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from functools import wraps
+
 from django import db
 from datetime import datetime
 
 
 def queries_count(func):
+    @wraps(func)
     def inner(*args, **kwargs):
         init_count = len(db.connection.queries)
         start_time = datetime.utcnow()
         res = func(*args, **kwargs)
         end_time = datetime.utcnow()
         end_count = len(db.connection.queries)
         values = [
```

### Comparing `air_drf_relation-0.6.0/air_drf_relation/extra_kwargs.py` & `air_drf_relation-0.6.1/air_drf_relation/extra_kwargs.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/fields.py` & `air_drf_relation-0.6.1/air_drf_relation/fields.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/filters.py` & `air_drf_relation-0.6.1/air_drf_relation/filters.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/model_fields.py` & `air_drf_relation-0.6.1/air_drf_relation/model_fields.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/preload_objects_manager.py` & `air_drf_relation-0.6.1/air_drf_relation/preload_objects_manager.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/queryset_optimization.py` & `air_drf_relation-0.6.1/air_drf_relation/queryset_optimization.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/serializers.py` & `air_drf_relation-0.6.1/air_drf_relation/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation/utils.py` & `air_drf_relation-0.6.1/air_drf_relation/utils.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/air_drf_relation.egg-info/PKG-INFO` & `air_drf_relation-0.6.1/air_drf_relation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air-drf-relation
-Version: 0.6.0
+Version: 0.6.1
 Summary: Improved interaction with DRF relations.
 Home-page: https://github.com/bubaley/air-drf-relation
 Author: bubaley
 Author-email: bubaley.fu@gmail.com
 License: MIT
 Description: **AIR-DRF-RELATION**
```

### Comparing `air_drf_relation-0.6.0/air_drf_relation.egg-info/SOURCES.txt` & `air_drf_relation-0.6.1/air_drf_relation.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 air_drf_relation/__init__.py
 air_drf_relation/context_builder.py
 air_drf_relation/decorators.py
+air_drf_relation/encoders.py
 air_drf_relation/extra_kwargs.py
 air_drf_relation/fields.py
 air_drf_relation/filters.py
 air_drf_relation/model_fields.py
 air_drf_relation/preload_objects_manager.py
 air_drf_relation/queryset_optimization.py
 air_drf_relation/serializers.py
```

### Comparing `air_drf_relation-0.6.0/device/migrations/0001_initial.py` & `air_drf_relation-0.6.1/device/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/device/serializers.py` & `air_drf_relation-0.6.1/device/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/device/tests.py` & `air_drf_relation-0.6.1/device/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/film/migrations/0001_initial.py` & `air_drf_relation-0.6.1/film/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/film/models.py` & `air_drf_relation-0.6.1/film/models.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/film/serializers.py` & `air_drf_relation-0.6.1/film/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/film/tests.py` & `air_drf_relation-0.6.1/film/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/setup.py` & `air_drf_relation-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='air_drf_relation',
-      version='0.6.0',
+      version='0.6.1',
       description='Improved interaction with DRF relations.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       keywords='django rest relation nested pk primary object',
       url='https://github.com/bubaley/air-drf-relation',
       author='bubaley',
       author_email='bubaley.fu@gmail.com',
```

### Comparing `air_drf_relation-0.6.0/table/migrations/0001_initial.py` & `air_drf_relation-0.6.1/table/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/table/migrations/0003_auto_20220513_1542.py` & `air_drf_relation-0.6.1/table/migrations/0003_auto_20220513_1542.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/table/migrations/0004_material_company.py` & `air_drf_relation-0.6.1/table/migrations/0004_material_company.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/table/models.py` & `air_drf_relation-0.6.1/table/models.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/table/serializers.py` & `air_drf_relation-0.6.1/table/serializers.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/table/tests.py` & `air_drf_relation-0.6.1/table/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/task/migrations/0001_initial.py` & `air_drf_relation-0.6.1/task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/task/migrations/0003_tag.py` & `air_drf_relation-0.6.1/task/migrations/0003_tag.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/task/migrations/0004_tag_task.py` & `air_drf_relation-0.6.1/task/migrations/0004_tag_task.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/task/tests.py` & `air_drf_relation-0.6.1/task/tests.py`

 * *Files identical despite different names*

### Comparing `air_drf_relation-0.6.0/task/views.py` & `air_drf_relation-0.6.1/task/views.py`

 * *Files identical despite different names*


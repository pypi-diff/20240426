# Comparing `tmp/dbt-mysql-1.7.0.tar.gz` & `tmp/dbt-mysql-1.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-mysql-1.7.0.tar", last modified: Fri Apr 26 16:39:57 2024, max compression
+gzip compressed data, was "dbt-mysql-1.7.0a1.tar", last modified: Sun Jan 21 18:38:18 2024, max compression
```

## Comparing `dbt-mysql-1.7.0.tar` & `dbt-mysql-1.7.0a1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.272966 dbt-mysql-1.7.0/
--rw-r--r--   0 wallace   (1000) wallace   (1000)    11357 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/LICENSE
--rw-r--r--   0 wallace   (1000) wallace   (1000)       47 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/MANIFEST.in
--rw-r--r--   0 wallace   (1000) wallace   (1000)     9295 2024-04-26 16:39:57.272966 dbt-mysql-1.7.0/PKG-INFO
--rw-r--r--   0 wallace   (1000) wallace   (1000)     8526 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/README.md
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.256300 dbt-mysql-1.7.0/dbt/
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.256300 dbt-mysql-1.7.0/dbt/adapters/
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.259633 dbt-mysql-1.7.0/dbt/adapters/mariadb/
--rw-r--r--   0 wallace   (1000) wallace   (1000)      557 2024-01-21 15:15:21.000000 dbt-mysql-1.7.0/dbt/adapters/mariadb/__init__.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)       18 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mariadb/__version__.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)      888 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mariadb/column.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)     5900 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mariadb/connections.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)    10740 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mariadb/impl.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)     1347 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mariadb/relation.py
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.262966 dbt-mysql-1.7.0/dbt/adapters/mysql/
--rw-r--r--   0 wallace   (1000) wallace   (1000)      529 2024-01-21 15:15:21.000000 dbt-mysql-1.7.0/dbt/adapters/mysql/__init__.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)       18 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql/__version__.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)      882 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql/column.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)     5751 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql/connections.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)    10854 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql/impl.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)     1329 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql/relation.py
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.262966 dbt-mysql-1.7.0/dbt/adapters/mysql5/
--rw-r--r--   0 wallace   (1000) wallace   (1000)      536 2024-01-21 15:15:21.000000 dbt-mysql-1.7.0/dbt/adapters/mysql5/__init__.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)       18 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql5/__version__.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)      882 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql5/column.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)     5893 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql5/connections.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)    10710 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql5/impl.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)     1331 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/adapters/mysql5/relation.py
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.259633 dbt-mysql-1.7.0/dbt/include/
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.262966 dbt-mysql-1.7.0/dbt/include/mariadb/
--rw-r--r--   0 wallace   (1000) wallace   (1000)       52 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/dbt/include/mariadb/__init__.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)       75 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mariadb/dbt_project.yml
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.266300 dbt-mysql-1.7.0/dbt/include/mariadb/macros/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     5016 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/include/mariadb/macros/adapters.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)     1666 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mariadb/macros/catalog.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.256300 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.266300 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/incremental/
--rw-r--r--   0 wallace   (1000) wallace   (1000)      872 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/incremental/helpers.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)     2202 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/incremental/incremental.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.266300 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/seed/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     1113 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.266300 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/snapshot/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     6014 2024-01-11 21:00:20.000000 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)      892 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)      227 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.266300 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/test/
--rw-r--r--   0 wallace   (1000) wallace   (1000)      515 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/test/test.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)      571 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mariadb/sample_profiles.yml
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.266300 dbt-mysql-1.7.0/dbt/include/mysql/
--rw-r--r--   0 wallace   (1000) wallace   (1000)       52 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/dbt/include/mysql/__init__.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)       73 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql/dbt_project.yml
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.266300 dbt-mysql-1.7.0/dbt/include/mysql/macros/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     4605 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/include/mysql/macros/adapters.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)     1695 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql/macros/catalog.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.259633 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.269633 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/incremental/
--rw-r--r--   0 wallace   (1000) wallace   (1000)      872 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/incremental/helpers.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)     2200 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/incremental/incremental.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.269633 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/seed/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     1113 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.269633 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/snapshot/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     4141 2024-01-11 21:00:20.000000 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)      888 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)      225 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.269633 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/test/
--rw-r--r--   0 wallace   (1000) wallace   (1000)      513 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/test/test.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)      567 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql/sample_profiles.yml
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.269633 dbt-mysql-1.7.0/dbt/include/mysql5/
--rw-r--r--   0 wallace   (1000) wallace   (1000)       52 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/dbt/include/mysql5/__init__.py
--rw-r--r--   0 wallace   (1000) wallace   (1000)       74 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql5/dbt_project.yml
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.269633 dbt-mysql-1.7.0/dbt/include/mysql5/macros/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     4633 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/dbt/include/mysql5/macros/adapters.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)     1665 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql5/macros/catalog.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.259633 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.269633 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/incremental/
--rw-r--r--   0 wallace   (1000) wallace   (1000)      872 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/incremental/helpers.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)     2201 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/incremental/incremental.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.269633 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/seed/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     1113 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.272966 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/snapshot/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     6015 2024-01-11 21:00:20.000000 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)      890 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)      226 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.272966 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/test/
--rw-r--r--   0 wallace   (1000) wallace   (1000)      514 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/test/test.sql
--rw-r--r--   0 wallace   (1000) wallace   (1000)      569 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0/dbt/include/mysql5/sample_profiles.yml
-drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-04-26 16:39:57.272966 dbt-mysql-1.7.0/dbt_mysql.egg-info/
--rw-r--r--   0 wallace   (1000) wallace   (1000)     9295 2024-04-26 16:39:57.000000 dbt-mysql-1.7.0/dbt_mysql.egg-info/PKG-INFO
--rw-r--r--   0 wallace   (1000) wallace   (1000)     2721 2024-04-26 16:39:57.000000 dbt-mysql-1.7.0/dbt_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 wallace   (1000) wallace   (1000)        1 2024-04-26 16:39:57.000000 dbt-mysql-1.7.0/dbt_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 wallace   (1000) wallace   (1000)        1 2024-01-11 21:07:29.000000 dbt-mysql-1.7.0/dbt_mysql.egg-info/not-zip-safe
--rw-r--r--   0 wallace   (1000) wallace   (1000)       46 2024-04-26 16:39:57.000000 dbt-mysql-1.7.0/dbt_mysql.egg-info/requires.txt
--rw-r--r--   0 wallace   (1000) wallace   (1000)        4 2024-04-26 16:39:57.000000 dbt-mysql-1.7.0/dbt_mysql.egg-info/top_level.txt
--rw-r--r--   0 wallace   (1000) wallace   (1000)       38 2024-04-26 16:39:57.272966 dbt-mysql-1.7.0/setup.cfg
--rw-r--r--   0 wallace   (1000) wallace   (1000)     2956 2024-04-26 16:39:28.000000 dbt-mysql-1.7.0/setup.py
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.932946 dbt-mysql-1.7.0a1/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)    11357 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/LICENSE
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       47 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/MANIFEST.in
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     8725 2024-01-21 18:38:18.932946 dbt-mysql-1.7.0a1/PKG-INFO
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     8030 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/README.md
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.919613 dbt-mysql-1.7.0a1/dbt/
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.919613 dbt-mysql-1.7.0a1/dbt/adapters/
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.926280 dbt-mysql-1.7.0a1/dbt/adapters/mariadb/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      557 2024-01-21 15:15:21.000000 dbt-mysql-1.7.0a1/dbt/adapters/mariadb/__init__.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       20 2024-01-21 18:38:14.000000 dbt-mysql-1.7.0a1/dbt/adapters/mariadb/__version__.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      888 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/adapters/mariadb/column.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     5688 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/adapters/mariadb/connections.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)    10740 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/adapters/mariadb/impl.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     1347 2024-01-21 18:19:40.000000 dbt-mysql-1.7.0a1/dbt/adapters/mariadb/relation.py
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.926280 dbt-mysql-1.7.0a1/dbt/adapters/mysql/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      529 2024-01-21 15:15:21.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql/__init__.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       20 2024-01-21 18:38:14.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql/__version__.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      882 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql/column.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     5539 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql/connections.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)    10854 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql/impl.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     1329 2024-01-21 18:19:40.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql/relation.py
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.926280 dbt-mysql-1.7.0a1/dbt/adapters/mysql5/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      536 2024-01-21 15:15:21.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql5/__init__.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       20 2024-01-21 18:38:14.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql5/__version__.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      882 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql5/column.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     5681 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql5/connections.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)    10710 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql5/impl.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     1331 2024-01-21 18:19:40.000000 dbt-mysql-1.7.0a1/dbt/adapters/mysql5/relation.py
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.922946 dbt-mysql-1.7.0a1/dbt/include/
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.926280 dbt-mysql-1.7.0a1/dbt/include/mariadb/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       52 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/__init__.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       75 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/dbt_project.yml
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.926280 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     5016 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/adapters.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     1666 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/catalog.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.922946 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.926280 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/incremental/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      872 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/incremental/helpers.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     2202 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/incremental/incremental.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/seed/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     1113 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/snapshot/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     6014 2024-01-11 21:00:20.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      892 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      227 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/test/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      515 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/test/test.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      571 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mariadb/sample_profiles.yml
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mysql/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       52 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/__init__.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       73 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/dbt_project.yml
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     4605 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/adapters.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     1695 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/catalog.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.922946 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/incremental/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      872 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/incremental/helpers.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     2200 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/incremental/incremental.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/seed/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     1113 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/snapshot/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     4141 2024-01-11 21:00:20.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      888 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      225 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/test/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      513 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/test/test.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      567 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql/sample_profiles.yml
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mysql5/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       52 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/__init__.py
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       74 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/dbt_project.yml
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.929613 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     4633 2024-01-21 18:24:22.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/adapters.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     1665 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/catalog.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.922946 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.932946 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/incremental/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      872 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/incremental/helpers.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     2201 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/incremental/incremental.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.932946 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/seed/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     1113 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.932946 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/snapshot/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     6015 2024-01-11 21:00:20.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      890 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      226 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.932946 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/test/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      514 2024-01-11 21:01:03.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/test/test.sql
+-rw-r--r--   0 wallace   (1000) wallace   (1000)      569 2024-01-11 20:51:33.000000 dbt-mysql-1.7.0a1/dbt/include/mysql5/sample_profiles.yml
+drwxr-xr-x   0 wallace   (1000) wallace   (1000)        0 2024-01-21 18:38:18.932946 dbt-mysql-1.7.0a1/dbt_mysql.egg-info/
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     8725 2024-01-21 18:38:18.000000 dbt-mysql-1.7.0a1/dbt_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     2721 2024-01-21 18:38:18.000000 dbt-mysql-1.7.0a1/dbt_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 wallace   (1000) wallace   (1000)        1 2024-01-21 18:38:18.000000 dbt-mysql-1.7.0a1/dbt_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 wallace   (1000) wallace   (1000)        1 2024-01-11 21:07:29.000000 dbt-mysql-1.7.0a1/dbt_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       53 2024-01-21 18:38:18.000000 dbt-mysql-1.7.0a1/dbt_mysql.egg-info/requires.txt
+-rw-r--r--   0 wallace   (1000) wallace   (1000)        4 2024-01-21 18:38:18.000000 dbt-mysql-1.7.0a1/dbt_mysql.egg-info/top_level.txt
+-rw-r--r--   0 wallace   (1000) wallace   (1000)       38 2024-01-21 18:38:18.932946 dbt-mysql-1.7.0a1/setup.cfg
+-rw-r--r--   0 wallace   (1000) wallace   (1000)     2945 2024-01-21 18:38:14.000000 dbt-mysql-1.7.0a1/setup.py
```

### Comparing `dbt-mysql-1.7.0/LICENSE` & `dbt-mysql-1.7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/PKG-INFO` & `dbt-mysql-1.7.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-mysql
-Version: 1.7.0
+Version: 1.7.0a1
 Summary: The MySQL adapter plugin for dbt
 Home-page: https://github.com/dbeatty10/dbt-mysql
 Author: Doug Beatty
 Author-email: doug.beatty@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -12,16 +12,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.7.0
-Requires-Dist: mysql-connector-python>=8.0.0
 
 # dbt-mysql
 
 [![Tests and Code Checks](https://github.com/dbeatty10/dbt-mysql/actions/workflows/main.yml/badge.svg)](https://github.com/dbeatty10/dbt-mysql/actions/workflows/main.yml)
 [![Integration Tests Badge](https://github.com/dbeatty10/dbt-mysql/actions/workflows/integration.yml/badge.svg)](https://github.com/dbeatty10/dbt-mysql/actions/workflows/integration.yml)
 
 This plugin ports [dbt](https://getdbt.com) functionality to MySQL and MariaDB.
@@ -103,29 +101,25 @@
       type: mysql
       server: localhost
       port: 3306
       schema: analytics
       username: your_mysql_username
       password: your_mysql_password
       ssl_disabled: True
-      charset: utf8mb4
-      collation: utf8mb4_0900_ai_ci
 ```
 
 | Option          | Description                                                                         | Required?                                                          | Example                                        |
 | --------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------ | ---------------------------------------------- |
-| type            | The specific adapter to use                                                         | Required                                                           | `mysql`, `mysql5` or `mariadb`                 |
+| type            | The specific adapter to use                                                         | Required                                                           | `mysql`, `mysql5` or `mariadb`                            |
 | server          | The server (hostname) to connect to                                                 | Required                                                           | `yourorg.mysqlhost.com`                        |
 | port            | The port to use                                                                     | Optional                                                           | `3306`                                         |
 | schema          | Specify the schema (database) to build models into                                  | Required                                                           | `analytics`                                    |
 | username        | The username to use to connect to the server                                        | Required                                                           | `dbt_admin`                                    |
 | password        | The password to use for authenticating to the server                                | Required                                                           | `correct-horse-battery-staple`                 |
 | ssl_disabled    | Set to enable or disable TLS connectivity to mysql5.x                               | Optional                                                           | `True` or `False`                              |
-| charset         | Specify charset to be used by a connection                                          | Optional                                                           | `utf8mb4`                                      |
-| collation       | Set to enable or disable TLS connectivity to mysql5.x                               | Optional                                                           | `utf8mb4_0900_ai_ci`                           |
 
 ### Notes
 
 Conflicting terminology is used between:
 - dbt
 - Database management systems (DBMS) like MySQL, Postgres, and Snowflake
 - metadata in the ANSI-standard `information_schema`
```

### Comparing `dbt-mysql-1.7.0/README.md` & `dbt-mysql-1.7.0a1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,29 +82,25 @@
       type: mysql
       server: localhost
       port: 3306
       schema: analytics
       username: your_mysql_username
       password: your_mysql_password
       ssl_disabled: True
-      charset: utf8mb4
-      collation: utf8mb4_0900_ai_ci
 ```
 
 | Option          | Description                                                                         | Required?                                                          | Example                                        |
 | --------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------ | ---------------------------------------------- |
-| type            | The specific adapter to use                                                         | Required                                                           | `mysql`, `mysql5` or `mariadb`                 |
+| type            | The specific adapter to use                                                         | Required                                                           | `mysql`, `mysql5` or `mariadb`                            |
 | server          | The server (hostname) to connect to                                                 | Required                                                           | `yourorg.mysqlhost.com`                        |
 | port            | The port to use                                                                     | Optional                                                           | `3306`                                         |
 | schema          | Specify the schema (database) to build models into                                  | Required                                                           | `analytics`                                    |
 | username        | The username to use to connect to the server                                        | Required                                                           | `dbt_admin`                                    |
 | password        | The password to use for authenticating to the server                                | Required                                                           | `correct-horse-battery-staple`                 |
 | ssl_disabled    | Set to enable or disable TLS connectivity to mysql5.x                               | Optional                                                           | `True` or `False`                              |
-| charset         | Specify charset to be used by a connection                                          | Optional                                                           | `utf8mb4`                                      |
-| collation       | Set to enable or disable TLS connectivity to mysql5.x                               | Optional                                                           | `utf8mb4_0900_ai_ci`                           |
 
 ### Notes
 
 Conflicting terminology is used between:
 - dbt
 - Database management systems (DBMS) like MySQL, Postgres, and Snowflake
 - metadata in the ANSI-standard `information_schema`
```

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mariadb/__init__.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mariadb/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mariadb/column.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mariadb/column.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mariadb/connections.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql5/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,51 +12,50 @@
 from dataclasses import dataclass
 from typing import Optional, Union
 
 logger = AdapterLogger("mysql")
 
 
 @dataclass(init=False)
-class MariaDBCredentials(Credentials):
+class MySQLCredentials(Credentials):
     server: str = ""
     unix_socket: Optional[str] = None
     port: Optional[int] = None
     database: Optional[str] = None  # type: ignore[assignment]
     schema: str = ""
     username: Optional[str] = None
     password: Optional[str] = None
     charset: Optional[str] = None
     ssl_disabled: Optional[bool] = None
-    collation: Optional[str] = None
 
     _ALIASES = {
         "UID": "username",
         "user": "username",
         "PWD": "password",
         "host": "server",
     }
 
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
             self.database = None
 
     def __post_init__(self):
-        # Database and schema are treated as the same thing
+        # mysql classifies database and schema as the same thing
         if self.database is not None and self.database != self.schema:
             raise dbt.exceptions.DbtRuntimeError(
                 f"    schema: {self.schema} \n"
                 f"    database: {self.database} \n"
-                f"On MariaDB, database must be omitted"
-                f" or have the same value as schema."
+                f"On MySQL, database must be omitted or have the same value as"
+                f" schema."
             )
 
     @property
     def type(self):
-        return "mariadb"
+        return "mysql5"
 
     @property
     def unique_field(self):
         return self.schema
 
     def _connection_keys(self):
         """
@@ -68,16 +67,16 @@
             "port",
             "database",
             "schema",
             "user",
         )
 
 
-class MariaDBConnectionManager(SQLConnectionManager):
-    TYPE = "mariadb"
+class MySQLConnectionManager(SQLConnectionManager):
+    TYPE = "mysql5"
 
     @classmethod
     def open(cls, connection):
         if connection.state == "open":
             logger.debug("Connection is already open, skipping open.")
             return connection
 
@@ -95,20 +94,14 @@
             kwargs["host"] = credentials.server
         elif credentials.unix_socket:
             kwargs["unix_socket"] = credentials.unix_socket
 
         if credentials.port:
             kwargs["port"] = credentials.port
 
-        if credentials.charset:
-            kwargs["charset"] = credentials.charset
-
-        if credentials.collation:
-            kwargs["collation"] = credentials.collation
-
         try:
             connection.handle = mysql.connector.connect(**kwargs)
             connection.state = "open"
         except mysql.connector.Error:
             try:
                 logger.debug(
                     "Failed connection without supplying the `database`. "
@@ -118,15 +111,15 @@
                 # Try again with the database included
                 kwargs["database"] = credentials.schema
 
                 connection.handle = mysql.connector.connect(**kwargs)
                 connection.state = "open"
             except mysql.connector.Error as e:
                 logger.debug(
-                    "Got an error when attempting to open a MariaDB " "connection: '{}'".format(e)
+                    "Got an error when attempting to open a mysql " "connection: '{}'".format(e)
                 )
 
                 connection.handle = None
                 connection.state = "fail"
 
                 raise dbt.exceptions.FailedToConnectError(str(e))
 
@@ -141,15 +134,15 @@
 
     @contextmanager
     def exception_handler(self, sql):
         try:
             yield
 
         except mysql.connector.DatabaseError as e:
-            logger.debug("MariaDB error: {}".format(str(e)))
+            logger.debug("MySQL error: {}".format(str(e)))
 
             try:
                 self.rollback_if_open()
             except mysql.connector.Error:
                 logger.debug("Failed to release connection!")
                 pass
```

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mariadb/impl.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mariadb/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mariadb/relation.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mariadb/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql/__init__.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql/column.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql/column.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql/connections.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql/connections.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     unix_socket: Optional[str] = None
     port: Optional[int] = None
     database: Optional[str] = None  # type: ignore[assignment]
     schema: str = ""
     username: Optional[str] = None
     password: Optional[str] = None
     charset: Optional[str] = None
-    collation: Optional[str] = None
 
     _ALIASES = {
         "UID": "username",
         "user": "username",
         "PWD": "password",
         "host": "server",
     }
@@ -91,20 +90,14 @@
             kwargs["host"] = credentials.server
         elif credentials.unix_socket:
             kwargs["unix_socket"] = credentials.unix_socket
 
         if credentials.port:
             kwargs["port"] = credentials.port
 
-        if credentials.charset:
-            kwargs["charset"] = credentials.charset
-
-        if credentials.collation:
-            kwargs["collation"] = credentials.collation
-
         try:
             connection.handle = mysql.connector.connect(**kwargs)
             connection.state = "open"
         except mysql.connector.Error:
             try:
                 logger.debug(
                     "Failed connection without supplying the `database`. "
```

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql/impl.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql/relation.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql5/__init__.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql5/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql5/column.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql5/column.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql5/connections.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mariadb/connections.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,51 +12,50 @@
 from dataclasses import dataclass
 from typing import Optional, Union
 
 logger = AdapterLogger("mysql")
 
 
 @dataclass(init=False)
-class MySQLCredentials(Credentials):
+class MariaDBCredentials(Credentials):
     server: str = ""
     unix_socket: Optional[str] = None
     port: Optional[int] = None
     database: Optional[str] = None  # type: ignore[assignment]
     schema: str = ""
     username: Optional[str] = None
     password: Optional[str] = None
     charset: Optional[str] = None
     ssl_disabled: Optional[bool] = None
-    collation: Optional[str] = None
 
     _ALIASES = {
         "UID": "username",
         "user": "username",
         "PWD": "password",
         "host": "server",
     }
 
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
             self.database = None
 
     def __post_init__(self):
-        # mysql classifies database and schema as the same thing
+        # Database and schema are treated as the same thing
         if self.database is not None and self.database != self.schema:
             raise dbt.exceptions.DbtRuntimeError(
                 f"    schema: {self.schema} \n"
                 f"    database: {self.database} \n"
-                f"On MySQL, database must be omitted or have the same value as"
-                f" schema."
+                f"On MariaDB, database must be omitted"
+                f" or have the same value as schema."
             )
 
     @property
     def type(self):
-        return "mysql5"
+        return "mariadb"
 
     @property
     def unique_field(self):
         return self.schema
 
     def _connection_keys(self):
         """
@@ -68,16 +67,16 @@
             "port",
             "database",
             "schema",
             "user",
         )
 
 
-class MySQLConnectionManager(SQLConnectionManager):
-    TYPE = "mysql5"
+class MariaDBConnectionManager(SQLConnectionManager):
+    TYPE = "mariadb"
 
     @classmethod
     def open(cls, connection):
         if connection.state == "open":
             logger.debug("Connection is already open, skipping open.")
             return connection
 
@@ -95,20 +94,14 @@
             kwargs["host"] = credentials.server
         elif credentials.unix_socket:
             kwargs["unix_socket"] = credentials.unix_socket
 
         if credentials.port:
             kwargs["port"] = credentials.port
 
-        if credentials.charset:
-            kwargs["charset"] = credentials.charset
-
-        if credentials.collation:
-            kwargs["collation"] = credentials.collation
-
         try:
             connection.handle = mysql.connector.connect(**kwargs)
             connection.state = "open"
         except mysql.connector.Error:
             try:
                 logger.debug(
                     "Failed connection without supplying the `database`. "
@@ -118,15 +111,15 @@
                 # Try again with the database included
                 kwargs["database"] = credentials.schema
 
                 connection.handle = mysql.connector.connect(**kwargs)
                 connection.state = "open"
             except mysql.connector.Error as e:
                 logger.debug(
-                    "Got an error when attempting to open a mysql " "connection: '{}'".format(e)
+                    "Got an error when attempting to open a MariaDB " "connection: '{}'".format(e)
                 )
 
                 connection.handle = None
                 connection.state = "fail"
 
                 raise dbt.exceptions.FailedToConnectError(str(e))
 
@@ -141,15 +134,15 @@
 
     @contextmanager
     def exception_handler(self, sql):
         try:
             yield
 
         except mysql.connector.DatabaseError as e:
-            logger.debug("MySQL error: {}".format(str(e)))
+            logger.debug("MariaDB error: {}".format(str(e)))
 
             try:
                 self.rollback_if_open()
             except mysql.connector.Error:
                 logger.debug("Failed to release connection!")
                 pass
```

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql5/impl.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql5/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/adapters/mysql5/relation.py` & `dbt-mysql-1.7.0a1/dbt/adapters/mysql5/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mariadb/macros/adapters.sql` & `dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mariadb/macros/catalog.sql` & `dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/incremental/helpers.sql` & `dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/incremental/incremental.sql` & `dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/seed/seed.sql` & `dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/snapshot/snapshot.sql` & `dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mariadb/macros/materializations/test/test.sql` & `dbt-mysql-1.7.0a1/dbt/include/mariadb/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mariadb/sample_profiles.yml` & `dbt-mysql-1.7.0a1/dbt/include/mariadb/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql/macros/adapters.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql/macros/catalog.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/incremental/helpers.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/incremental/incremental.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/seed/seed.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/snapshot/snapshot.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql/macros/materializations/test/test.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql/sample_profiles.yml` & `dbt-mysql-1.7.0a1/dbt/include/mysql/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql5/macros/adapters.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql5/macros/catalog.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/incremental/helpers.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/incremental/incremental.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/seed/seed.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/snapshot/snapshot.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql5/macros/materializations/test/test.sql` & `dbt-mysql-1.7.0a1/dbt/include/mysql5/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt/include/mysql5/sample_profiles.yml` & `dbt-mysql-1.7.0a1/dbt/include/mysql5/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/dbt_mysql.egg-info/PKG-INFO` & `dbt-mysql-1.7.0a1/dbt_mysql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-mysql
-Version: 1.7.0
+Version: 1.7.0a1
 Summary: The MySQL adapter plugin for dbt
 Home-page: https://github.com/dbeatty10/dbt-mysql
 Author: Doug Beatty
 Author-email: doug.beatty@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -12,16 +12,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.7.0
-Requires-Dist: mysql-connector-python>=8.0.0
 
 # dbt-mysql
 
 [![Tests and Code Checks](https://github.com/dbeatty10/dbt-mysql/actions/workflows/main.yml/badge.svg)](https://github.com/dbeatty10/dbt-mysql/actions/workflows/main.yml)
 [![Integration Tests Badge](https://github.com/dbeatty10/dbt-mysql/actions/workflows/integration.yml/badge.svg)](https://github.com/dbeatty10/dbt-mysql/actions/workflows/integration.yml)
 
 This plugin ports [dbt](https://getdbt.com) functionality to MySQL and MariaDB.
@@ -103,29 +101,25 @@
       type: mysql
       server: localhost
       port: 3306
       schema: analytics
       username: your_mysql_username
       password: your_mysql_password
       ssl_disabled: True
-      charset: utf8mb4
-      collation: utf8mb4_0900_ai_ci
 ```
 
 | Option          | Description                                                                         | Required?                                                          | Example                                        |
 | --------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------ | ---------------------------------------------- |
-| type            | The specific adapter to use                                                         | Required                                                           | `mysql`, `mysql5` or `mariadb`                 |
+| type            | The specific adapter to use                                                         | Required                                                           | `mysql`, `mysql5` or `mariadb`                            |
 | server          | The server (hostname) to connect to                                                 | Required                                                           | `yourorg.mysqlhost.com`                        |
 | port            | The port to use                                                                     | Optional                                                           | `3306`                                         |
 | schema          | Specify the schema (database) to build models into                                  | Required                                                           | `analytics`                                    |
 | username        | The username to use to connect to the server                                        | Required                                                           | `dbt_admin`                                    |
 | password        | The password to use for authenticating to the server                                | Required                                                           | `correct-horse-battery-staple`                 |
 | ssl_disabled    | Set to enable or disable TLS connectivity to mysql5.x                               | Optional                                                           | `True` or `False`                              |
-| charset         | Specify charset to be used by a connection                                          | Optional                                                           | `utf8mb4`                                      |
-| collation       | Set to enable or disable TLS connectivity to mysql5.x                               | Optional                                                           | `utf8mb4_0900_ai_ci`                           |
 
 ### Notes
 
 Conflicting terminology is used between:
 - dbt
 - Database management systems (DBMS) like MySQL, Postgres, and Snowflake
 - metadata in the ANSI-standard `information_schema`
```

### Comparing `dbt-mysql-1.7.0/dbt_mysql.egg-info/SOURCES.txt` & `dbt-mysql-1.7.0a1/dbt_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-mysql-1.7.0/setup.py` & `dbt-mysql-1.7.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     print("Error: dbt requires setuptools v40.1.0 or higher.")
     print('Please upgrade setuptools with "pip install --upgrade setuptools" ' "and try again")
     sys.exit(1)
 
 
 # pull long description from README
 this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
+with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 # get this package's version from dbt/adapters/<name>/__version__.py
 def _get_plugin_version_dict():
     _version_path = os.path.join(this_directory, "dbt", "adapters", "mysql", "__version__.py")
     _semver = r"""(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)"""
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-mysql"
-package_version = "1.7.0"
+package_version = "1.7.0a1"
 dbt_core_version = _get_dbt_core_version()
 description = """The MySQL adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
@@ -64,15 +64,15 @@
     author="Doug Beatty",
     author_email="doug.beatty@gmail.com",
     url="https://github.com/dbeatty10/dbt-mysql",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-core~={}".format(dbt_core_version),
-        "mysql-connector-python>=8.0.0",
+        "mysql-connector-python>=8.0.0,<8.1",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```


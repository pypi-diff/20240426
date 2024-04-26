# Comparing `tmp/pydiverse_pipedag-0.9.0.tar.gz` & `tmp/pydiverse_pipedag-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_pipedag-0.9.0.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.9.1.tar", max compression
```

## Comparing `pydiverse_pipedag-0.9.0.tar` & `pydiverse_pipedag-0.9.1.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0     1517 2024-04-17 10:05:40.314924 pydiverse_pipedag-0.9.0/LICENSE
--rw-r--r--   0        0        0     5623 2024-04-17 10:05:40.314924 pydiverse_pipedag-0.9.0/docs/package/README.md
--rw-r--r--   0        0        0     3912 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       13 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      629 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      857 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       97 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     6613 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0      393 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/__init__.py
--rw-r--r--   0        0        0     6102 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/base.py
--rw-r--r--   0        0        0    13646 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/database.py
--rw-r--r--   0        0        0     2756 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/filelock.py
--rw-r--r--   0        0        0      769 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/nolock.py
--rw-r--r--   0        0        0     3983 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/zookeeper.py
--rw-r--r--   0        0        0      233 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    30931 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0      108 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/__init__.py
--rw-r--r--   0        0        0     3455 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/base.py
--rw-r--r--   0        0        0     6892 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/parquet.py
--rw-r--r--   0        0        0     6757 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0      103 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/__init__.py
--rw-r--r--   0        0        0    41541 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/ddl.py
--rw-r--r--   0        0        0      187 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
--rw-r--r--   0        0        0     4411 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
--rw-r--r--   0        0        0    10717 2024-04-17 10:05:40.318924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
--rw-r--r--   0        0        0    12665 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
--rw-r--r--   0        0        0     5490 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
--rw-r--r--   0        0        0    30118 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/hooks.py
--rw-r--r--   0        0        0     4617 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/reflection.py
--rw-r--r--   0        0        0    62186 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/sql.py
--rw-r--r--   0        0        0       81 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     8887 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/util/dtype.py
--rw-r--r--   0        0        0      433 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0    12059 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    27776 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      408 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0    26497 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/config.py
--rw-r--r--   0        0        0    51959 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     7891 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/group_node.py
--rw-r--r--   0        0        0     4552 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     8529 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     8768 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      135 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/debug/__init__.py
--rw-r--r--   0        0        0      493 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      654 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     3123 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/dask.py
--rw-r--r--   0        0        0     7269 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1981 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1191 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/__init__.py
--rw-r--r--   0        0        0      620 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/cli.py
--rw-r--r--   0        0        0        0 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/__init__.py
--rw-r--r--   0        0        0     1741 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/clear_metadata.py
--rw-r--r--   0        0        0     2795 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/delete_schemas.py
--rw-r--r--   0        0        0      258 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     2735 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0    24375 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0    38201 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     4453 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/debug.py
--rw-r--r--   0        0        0     3837 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/details.py
--rw-r--r--   0        0        0     2074 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    21432 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0      213 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0     9273 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/computation_tracing.py
--rw-r--r--   0        0        0     2061 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1848 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      944 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1129 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/hashing.py
--rw-r--r--   0        0        0     3816 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     7992 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     5375 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/json.py
--rw-r--r--   0        0        0     1377 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     2847 2024-04-17 10:05:40.322924 pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/structlog.py
--rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-04-26 13:54:34.519514 pydiverse_pipedag-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5623 2024-04-26 13:54:34.519514 pydiverse_pipedag-0.9.1/docs/package/README.md
+-rw-r--r--   0        0        0     3912 2024-04-26 13:54:34.523514 pydiverse_pipedag-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-04-26 13:54:34.523514 pydiverse_pipedag-0.9.1/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      629 2024-04-26 13:54:34.523514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      857 2024-04-26 13:54:34.523514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       97 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     6613 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0      393 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/__init__.py
+-rw-r--r--   0        0        0     6102 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/base.py
+-rw-r--r--   0        0        0    13646 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/database.py
+-rw-r--r--   0        0        0     2756 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/filelock.py
+-rw-r--r--   0        0        0      769 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/nolock.py
+-rw-r--r--   0        0        0     3983 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/zookeeper.py
+-rw-r--r--   0        0        0      233 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    30931 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0      108 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/__init__.py
+-rw-r--r--   0        0        0     3455 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/base.py
+-rw-r--r--   0        0        0     7777 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/parquet.py
+-rw-r--r--   0        0        0     6757 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0      103 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/__init__.py
+-rw-r--r--   0        0        0    41933 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/ddl.py
+-rw-r--r--   0        0        0      230 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
+-rw-r--r--   0        0        0     4411 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
+-rw-r--r--   0        0        0    10717 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
+-rw-r--r--   0        0        0    12826 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
+-rw-r--r--   0        0        0     5490 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
+-rw-r--r--   0        0        0     3777 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/snowflake.py
+-rw-r--r--   0        0        0    30134 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/hooks.py
+-rw-r--r--   0        0        0     4617 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/reflection.py
+-rw-r--r--   0        0        0    62658 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/sql.py
+-rw-r--r--   0        0        0       81 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     9164 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/util/dtype.py
+-rw-r--r--   0        0        0      433 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0    12059 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    27776 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      408 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    26497 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0    51959 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     7891 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/group_node.py
+-rw-r--r--   0        0        0     4552 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     8529 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     8768 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      135 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/debug/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     3123 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/dask.py
+-rw-r--r--   0        0        0     7269 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1981 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1191 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/__init__.py
+-rw-r--r--   0        0        0      620 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/cli.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/__init__.py
+-rw-r--r--   0        0        0     1741 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/clear_metadata.py
+-rw-r--r--   0        0        0     2795 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/delete_schemas.py
+-rw-r--r--   0        0        0      258 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     2735 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0    24375 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0    38201 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     4453 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/debug.py
+-rw-r--r--   0        0        0     3837 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/details.py
+-rw-r--r--   0        0        0     2074 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    21432 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0      213 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     9273 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/computation_tracing.py
+-rw-r--r--   0        0        0     2061 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1848 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      944 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1129 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/hashing.py
+-rw-r--r--   0        0        0     3816 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     7992 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     5375 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/json.py
+-rw-r--r--   0        0        0     1377 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2847 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.9.1/PKG-INFO
```

### Comparing `pydiverse_pipedag-0.9.0/LICENSE` & `pydiverse_pipedag-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/docs/package/README.md` & `pydiverse_pipedag-0.9.1/docs/package/README.md`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/pyproject.toml` & `pydiverse_pipedag-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.9.0"
+version = "0.9.1"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
```

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/__init__.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/blob.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/base.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/database.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/database.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/filelock.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/nolock.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/nolock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/lock/zookeeper.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/zookeeper.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/base.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/cache/parquet.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/parquet.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,32 +106,50 @@
     def retrieve(
         cls,
         store: ParquetTableCache,
         table: Table,
         stage_name: str,
         as_type: type[pd.DataFrame],
     ) -> pd.DataFrame:
-        if PandasTableHook.pd_version < Version("2.0"):
-            return cls._retrieve(store, table, use_nullable_dtype=True)
-
         # Determine dtype backend for pandas >= 2.0
         # [this is similar to the PandasTableHook found in SQLTableStore]
 
         backend_str = "numpy"
         if hook_args := ConfigContext.get().table_hook_args.get("pandas", None):
             if dtype_backend := hook_args.get("dtype_backend", None):
                 backend_str = dtype_backend
 
         if isinstance(as_type, tuple):
             backend_str = as_type[1]
         elif isinstance(as_type, dict):
             backend_str = as_type["backend"]
 
-        dtype_backend = {"arrow": "pyarrow", "numpy": "numpy_nullable"}
-        return cls._retrieve(store, table, dtype_backend=dtype_backend[backend_str])
+        if PandasTableHook.pd_version < Version("2.0"):
+            # for use_nullable_dtypes=False, returned types are mostly numpy backed
+            # extension dtypes
+            ret = cls._retrieve(
+                store, table, use_nullable_dtypes=backend_str != "arrow"
+            )
+            # use_nullable_dtypes=False may still return string[python] even though we
+            # expect and sometimes get string[pyarrow]
+            for col in ret.dtypes[ret.dtypes == "string[python]"].index:
+                ret[col] = ret[col].astype(pd.StringDtype("pyarrow"))
+        else:
+            dtype_backend_map = {"arrow": "pyarrow", "numpy": "numpy_nullable"}
+            ret = cls._retrieve(
+                store, table, dtype_backend=dtype_backend_map[backend_str]
+            )
+
+        # Prefer StringDtype("pyarrow") over ArrowDtype(pa.string()) for now.
+        # We need to check this choice with future versions of pandas/pyarrow.
+        for col in ret.dtypes[
+            (ret.dtypes == "large_string[pyarrow]") | (ret.dtypes == "string[pyarrow]")
+        ].index:
+            ret[col] = ret[col].astype(pd.StringDtype("pyarrow"))
+        return ret
 
     @classmethod
     def _retrieve(cls, store, table, **pandas_kwargs):
         path = store.get_table_path(table, ".parquet")
         return pd.read_parquet(path, **pandas_kwargs)
```

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/ddl.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/ddl.py`

 * *Files 1% similar despite different names*

```diff
@@ -863,14 +863,23 @@
     _ = kw
     from_table = compiler.preparer.quote(rename_table.from_name)
     to_table = compiler.preparer.quote(rename_table.to_name)
     schema = compiler.preparer.format_schema(rename_table.schema.get())
     return f"RENAME TABLE {schema}.{from_table} TO {to_table}"
 
 
+@compiles(RenameTable, "snowflake")
+def visit_rename_table(rename_table: RenameTable, compiler, **kw):
+    _ = kw
+    from_table = compiler.preparer.quote(rename_table.from_name)
+    to_table = compiler.preparer.quote(rename_table.to_name)
+    schema = compiler.preparer.format_schema(rename_table.schema.get())
+    return f"ALTER TABLE {schema}.{from_table} RENAME TO {schema}.{to_table}"
+
+
 @compiles(DropTable)
 def visit_drop_table(drop: DropTable, compiler, **kw):
     return _visit_drop_anything(drop, "TABLE", compiler, **kw)
 
 
 @compiles(DropTable, "mssql")
 def visit_drop_table(drop: DropTable, compiler, **kw):
```

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from typing import Any
 
 import pandas as pd
 import sqlalchemy as sa
 import sqlalchemy.dialects.mssql
 
 from pydiverse.pipedag.backend.table.sql.ddl import (
-    AddIndex,
-    AddPrimaryKey,
     ChangeColumnTypes,
     CreateAlias,
     _mssql_update_definition,
 )
 from pydiverse.pipedag.backend.table.sql.hooks import IbisTableHook, PandasTableHook
 from pydiverse.pipedag.backend.table.sql.reflection import PipedagMSSqlReflection
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
@@ -75,52 +73,21 @@
         self.max_query_print_length = max_query_print_length
 
         super().__init__(*args, **kwargs)
 
     def _init_database(self):
         self._init_database_with_database("master", {"isolation_level": "AUTOCOMMIT"})
 
-    def add_primary_key(
-        self,
-        table_name: str,
-        schema: Schema,
-        key_columns: list[str],
-        *,
-        name: str | None = None,
-    ):
-        self.execute(AddPrimaryKey(table_name, schema, key_columns, name))
-
-    def add_index(
-        self,
-        table_name: str,
-        schema: Schema,
-        index_columns: list[str],
-        name: str | None = None,
-    ):
-        sql_types = self.reflect_sql_types(index_columns, table_name, schema)
-        if any(
-            [
-                isinstance(_type, sa.String) and _type.length is None
-                for _type in sql_types
-            ]
-        ):
-            # impose some varchar(max) limit to allow use in primary key / index
-            self.execute(
-                ChangeColumnTypes(
-                    table_name, schema, index_columns, sql_types, cap_varchar_max=1024
-                )
-            )
-        self.execute(AddIndex(table_name, schema, index_columns, name))
-
     def dialect_requests_empty_creation(self, table: Table, is_sql: bool) -> bool:
         _ = is_sql
         return (
             table.nullable is not None
             or table.non_nullable is not None
             or (table.primary_key is not None and len(table.primary_key) > 0)
+            or (table.indexes is not None and len(table.indexes) > 0)
         )
 
     def get_forced_nullability_columns(
         self, table: Table, table_cols: Iterable[str], report_nullable_cols=False
     ) -> tuple[list[str], list[str]]:
         # mssql dialect has literals as non-nullable types by default, so we also need
         # the list of nullable columns as well
@@ -186,16 +153,40 @@
                         schema,
                         key_columns,
                         sql_types,
                         nullable=False,
                         cap_varchar_max=1024,
                     )
                 )
-            self.add_table_primary_key(table, schema)
+                index_columns = set()  # type: set[str]
+                if table.indexes is not None:
+                    for index in table.indexes:
+                        index_columns |= set(index)
+                index_columns_list = list(index_columns)
+                sql_types = self.reflect_sql_types(
+                    index_columns_list, table.name, schema
+                )
+                index_str_max_columns = [
+                    col
+                    for _type, col in zip(sql_types, index_columns_list)
+                    if isinstance(_type, sa.String) and _type.length is None
+                ]
+                if len(index_str_max_columns) > 0:
+                    # impose some varchar(max) limit to allow use in primary key / index
+                    self.execute(
+                        ChangeColumnTypes(
+                            table.name,
+                            schema,
+                            index_str_max_columns,
+                            sql_types,
+                            cap_varchar_max=1024,
+                        )
+                    )
         if on_empty_table is None or not on_empty_table:
+            self.add_table_primary_key(table, schema)
             self.add_table_indexes(table, schema)
 
     def execute_raw_sql(self, raw_sql: RawSql):
         if self.disable_pytsql:
             self.__execute_raw_sql_fallback(raw_sql)
         else:
             self.__execute_raw_sql_pytsql(raw_sql)
```

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/hooks.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,17 +465,15 @@
     def _execute_query_retrieve(
         cls,
         store: SQLTableStore,
         query: Any,
         dtypes: dict[str, DType],
         backend: PandasDTypeBackend,
     ) -> pd.DataFrame:
-        dtypes = {
-            name: dtype.to_pandas(backend=backend) for name, dtype in dtypes.items()
-        }
+        dtypes = {name: dtype.to_pandas(backend) for name, dtype in dtypes.items()}
 
         with store.engine.connect() as conn:
             if PandasTableHook.pd_version >= Version("2.0"):
                 df = pd.read_sql(query, con=conn, dtype=dtypes)
             else:
                 df = pd.read_sql(query, con=conn)
                 for col, dtype in dtypes.items():
@@ -567,15 +565,15 @@
         as_type: type[polars.DataFrame],
     ) -> polars.DataFrame:
         query = cls._read_db_query(store, table, stage_name)
         query = cls._compile_query(store, query)
         connection_uri = store.engine_url.render_as_string(hide_password=False)
         try:
             return cls._execute_query(query, connection_uri)
-        except RuntimeError as e:
+        except (RuntimeError, ModuleNotFoundError) as e:
             logger = structlog.get_logger(logger_name=cls.__name__)
             logger.error(
                 "Fallback via Pandas since Polars failed to execute query on "
                 "database %s: %s",
                 store.engine_url.render_as_string(hide_password=True),
                 e,
             )
@@ -601,15 +599,15 @@
         return str(query.compile(store.engine, compile_kwargs={"literal_binds": True}))
 
     @classmethod
     def _execute_query(cls, query: str, connection_uri: str):
         try:
             df = polars.read_database(query, connection_uri)
             return df
-        except RuntimeError as e:
+        except (RuntimeError, ModuleNotFoundError) as e:
             logger = structlog.get_logger(logger_name=cls.__name__)
             engine = sa.create_engine(connection_uri)
             logger.error(
                 "Fallback via Pandas since Polars failed to execute query on "
                 "database %s: %s",
                 engine.url.render_as_string(hide_password=True),
                 e,
```

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/reflection.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/reflection.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/sql/sql.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,17 @@
         used to connect to the database.
 
         This URL may contain placeholders like ``{name}`` or ``{instance_id}``
         (additional ones can be defined in the ``url_attrs_file``) or
         environment variables like ``{$USER}`` which get substituted with their
         respective values.
 
+        Attention: passwords including special characters like ``@`` or ``:`` need
+        to be URL encoded.
+
     :param url_attrs_file:
         Filename of a yaml file which is read shortly before rendering the final
         engine URL and which is used to replace custom placeholders in ``url``.
 
         Just like ``url``, this value may also contain placeholders and environment
         variables which get substituted.
 
@@ -343,38 +346,45 @@
             return
 
         raise NotImplementedError(
             "create_database_if_not_exists is not implemented for this engine"
         )
 
     def _init_database_with_database(
-        self, database: str, execution_options: dict = None
+        self,
+        database: str,
+        execution_options: dict = None,
+        create_database: str | None = None,
+        disable_exists_check=False,
     ):
         if not self.create_database_if_not_exists:
             return
 
         if execution_options is None:
             execution_options = {}
 
-        try:
-            # Check if database exists
-            with self.engine.connect() as conn:
-                conn.exec_driver_sql("SELECT 1")
-            return
-        except sa.exc.DBAPIError:
-            # Database doesn't exist
-            pass
+        if not disable_exists_check:
+            try:
+                # Check if database exists
+                with self.engine.connect() as conn:
+                    conn.exec_driver_sql("SELECT 1")
+                return
+            except sa.exc.DBAPIError:
+                # Database doesn't exist
+                pass
 
         # Create new database using temporary engine object
         tmp_db_url = self.engine_url.set(database=database)
         tmp_engine = sa.create_engine(tmp_db_url, execution_options=execution_options)
 
         try:
+            if create_database is None:
+                create_database = self.engine_url.database
             with tmp_engine.connect() as conn:
-                conn.execute(CreateDatabase(self.engine_url.database))
+                conn.execute(CreateDatabase(create_database))
         except sa.exc.DBAPIError:
             # This happens if multiple instances try to create the database
             # at the same time.
             with self.engine.connect() as conn:
                 # Verify database actually exists
                 conn.exec_driver_sql("SELECT 1")
 
@@ -384,27 +394,29 @@
 
     def _create_engine(self):
         kwargs = {}
         if self._default_isolation_level() is not None:
             kwargs["isolation_level"] = self._default_isolation_level()
 
         # future=True enables SQLAlchemy 2.0 behaviour with version 1.4
+        # However, it does not support pd.read_sql_table
         return sa.create_engine(
             self.engine_url,
-            future=True,
+            # future=True,
             pool_size=self.sqlalchemy_pool_size,
             pool_timeout=self.squalchemy_pool_timeout,
             **kwargs,
         )
 
     @contextmanager
     def engine_connect(self) -> sa.Connection:
         with self.engine.connect() as conn:
             yield conn
-            conn.commit()
+            if sa.__version__ >= "2.0.0":
+                conn.commit()
 
     def get_schema(self, name: str) -> Schema:
         return Schema(name, self.schema_prefix, self.schema_suffix)
 
     def _execute(
         self, query, conn: sa.engine.Connection, truncate_printed_select=False
     ):
```

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/backend/table/util/dtype.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/util/dtype.py`

 * *Files 10% similar despite different names*

```diff
@@ -207,20 +207,26 @@
             DType.DATE: sa.Date(),
             DType.TIME: sa.Time(),
             DType.DATETIME: sa.DateTime(),
         }[self]
 
     def to_pandas(self, backend: PandasDTypeBackend = PandasDTypeBackend.ARROW):
         if backend == PandasDTypeBackend.NUMPY:
-            return self.to_pandas_nullable()
+            return self.to_pandas_nullable(backend)
         if backend == PandasDTypeBackend.ARROW:
+            if self == DType.STRING:
+                return pd.StringDtype(storage="pyarrow")
             return pd.ArrowDtype(self.to_arrow())
 
-    def to_pandas_nullable(self):
+    def to_pandas_nullable(
+        self, backend: PandasDTypeBackend = PandasDTypeBackend.ARROW
+    ):
         if self == DType.TIME:
+            if backend == PandasDTypeBackend.ARROW:
+                return pd.ArrowDtype(self.to_arrow())
             raise TypeError("pandas doesn't have a native time dtype")
 
         return {
             DType.INT8: pd.Int8Dtype(),
             DType.INT16: pd.Int16Dtype(),
             DType.INT32: pd.Int32Dtype(),
             DType.INT64: pd.Int64Dtype(),
```

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/context.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/run_context.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/config.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/config.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/flow.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/flow.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/group_node.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/group_node.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/result.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/stage.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/task.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/dask.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/dask.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/cli.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/cli.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/clear_metadata.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/clear_metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/management/commands/delete_schemas.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/delete_schemas.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/container.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/container.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/core.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/core.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/debug.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/debug.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/details.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/details.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/store.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/computation_tracing.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/computation_tracing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/hashing.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/hashing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/import_.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/json.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/json.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/naming.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/src/pydiverse/pipedag/util/structlog.py` & `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/structlog.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.0/PKG-INFO` & `pydiverse_pipedag-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.9.0
+Version: 0.9.1
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```


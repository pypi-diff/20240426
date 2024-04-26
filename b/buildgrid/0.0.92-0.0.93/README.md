# Comparing `tmp/buildgrid-0.0.92.tar.gz` & `tmp/buildgrid-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildgrid-0.0.92.tar", last modified: Thu Apr 18 10:44:10 2024, max compression
+gzip compressed data, was "buildgrid-0.0.93.tar", last modified: Fri Apr 26 14:31:28 2024, max compression
```

## Comparing `buildgrid-0.0.92.tar` & `buildgrid-0.0.93.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.959592 buildgrid-0.0.92/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-18 10:43:42.000000 buildgrid-0.0.92/BuildGrid.doap
--rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-18 10:43:42.000000 buildgrid-0.0.92/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    11338 2024-04-18 10:43:42.000000 buildgrid-0.0.92/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-04-18 10:43:42.000000 buildgrid-0.0.92/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6265 2024-04-18 10:44:10.959592 buildgrid-0.0.92/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-18 10:43:42.000000 buildgrid-0.0.92/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.855591 buildgrid-0.0.92/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.856591 buildgrid-0.0.92/buildgrid/_app/
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5661 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.859591 buildgrid-0.0.92/buildgrid/_app/commands/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_browser_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     3170 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10608 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_cas.py
--rw-rw-rw-   0 root         (0) root         (0)     8817 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)    12570 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_janitor.py
--rw-rw-rw-   0 root         (0) root         (0)     4842 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_logstream.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_operation.py
--rw-rw-rw-   0 root         (0) root         (0)     8166 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/cmd_server.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/commands/rpc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.860591 buildgrid-0.0.92/buildgrid/_app/settings/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   110917 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     8691 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/reference.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.860591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.861591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/with-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.861591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/clients/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/clients/asset-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2785 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.862591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/connections/
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/connections/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/connections/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.862591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/misc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/misc/channel.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.862591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/scheduler/memory.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3907 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/scheduler/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.864591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      971 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/bots.yaml
--rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/bytestream.yaml
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/cas.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1557 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/execution.yaml
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/platform-queues.yml
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.867591 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/disk.yaml
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/lru.yaml
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/redis-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      601 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/remote.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/replicated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      592 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/s3.yaml
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/sharded.yaml
--rw-rw-rw-   0 root         (0) root         (0)      530 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/sql-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/sql.yaml
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/with-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4776 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.867591 buildgrid-0.0.92/buildgrid/_protos/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.868591 buildgrid-0.0.92/buildgrid/_protos/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.868591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.868591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.868591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.870591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7795 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    27103 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    15404 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    15550 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.871591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.873591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30140 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   136470 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    47588 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    47884 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.873591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.875591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2066 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7844 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.877591 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.879591 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1944 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4156 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.879591 buildgrid-0.0.92/buildgrid/_protos/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.884591 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10940 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3824 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9955 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2881 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.885591 buildgrid-0.0.92/buildgrid/_protos/google/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.891591 buildgrid-0.0.92/buildgrid/_protos/google/api/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2291 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18246 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.893591 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7478 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     8880 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     8996 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.893591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.894591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.898591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5933 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18014 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2545 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5408 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6758 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.898591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.904591 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    23457 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7140 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7256 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6133 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    21890 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5337 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9321 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     4498 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2751 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    11299 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.905591 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5084 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7984 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7133 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.910591 buildgrid-0.0.92/buildgrid/_protos/google/rpc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    13407 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4774 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1573 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_types.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.910591 buildgrid-0.0.92/buildgrid/browser/
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/browser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4469 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/browser/app.py
--rw-rw-rw-   0 root         (0) root         (0)    34436 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/browser/rest_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/browser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.911591 buildgrid-0.0.92/buildgrid/cleanup/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9520 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/cleanup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.912591 buildgrid-0.0.92/buildgrid/cleanup/janitor/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3318 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/index.py
--rw-rw-rw-   0 root         (0) root         (0)     4565 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/cleanup/janitor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.915591 buildgrid-0.0.92/buildgrid/client/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5099 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/auth_token_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/authentication.py
--rwxrwxrwx   0 root         (0) root         (0)     1650 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    41408 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/cas.py
--rw-rw-rw-   0 root         (0) root         (0)    13926 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/interceptors.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/logstream.py
--rw-rw-rw-   0 root         (0) root         (0)     3410 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/client/retrier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.917591 buildgrid-0.0.92/buildgrid/server/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.918591 buildgrid-0.0.92/buildgrid/server/actioncache/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.920591 buildgrid-0.0.92/buildgrid/server/actioncache/caches/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5564 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/action_cache_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     5593 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4197 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6534 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/redis_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6573 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/remote_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    11662 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/s3_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/caches/write_once_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     4045 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/actioncache/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.922591 buildgrid-0.0.92/buildgrid/server/auth/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/auth/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.923591 buildgrid-0.0.92/buildgrid/server/bots/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/bots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/bots/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7343 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/bots/job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)     5647 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/bots/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.923591 buildgrid-0.0.92/buildgrid/server/build_events/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/build_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6045 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/build_events/service.py
--rw-rw-rw-   0 root         (0) root         (0)     7213 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/build_events/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.924591 buildgrid-0.0.92/buildgrid/server/capabilities/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/capabilities/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7113 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/capabilities/instance.py
--rwxrwxrwx   0 root         (0) root         (0)     3342 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/capabilities/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.925591 buildgrid-0.0.92/buildgrid/server/cas/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21869 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/instance.py
--rw-rw-rw-   0 root         (0) root         (0)    11124 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.927591 buildgrid-0.0.92/buildgrid/server/cas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.928591 buildgrid-0.0.92/buildgrid/server/cas/storage/index/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/index_abc.py
--rw-rw-rw-   0 root         (0) root         (0)    13464 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/redis.py
--rw-rw-rw-   0 root         (0) root         (0)    38426 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.929592 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     4436 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/lru_memory_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/remote.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/replicated.py
--rw-rw-rw-   0 root         (0) root         (0)    14426 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     6002 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/sharded.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/size_differentiated.py
--rw-rw-rw-   0 root         (0) root         (0)     9519 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/sql.py
--rw-rw-rw-   0 root         (0) root         (0)     8154 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/storage_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     7796 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/cas/storage/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/context.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.930591 buildgrid-0.0.92/buildgrid/server/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9599 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/execution/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7517 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/execution/service.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/job_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    18121 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/metrics_names.py
--rw-rw-rw-   0 root         (0) root         (0)    14482 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19548 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.931591 buildgrid-0.0.92/buildgrid/server/operations/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.932592 buildgrid-0.0.92/buildgrid/server/operations/filtering/
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/filter_grammar.lark
--rw-rw-rw-   0 root         (0) root         (0)     5769 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/interpreter.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/filtering/sanitizer.py
--rw-rw-rw-   0 root         (0) root         (0)     4802 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/operations/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.933591 buildgrid-0.0.92/buildgrid/server/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.934591 buildgrid-0.0.92/buildgrid/server/persistence/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.934591 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/README
--rw-rw-rw-   0 root         (0) root         (0)     2919 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/env.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.939592 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
--rw-rw-rw-   0 root         (0) root         (0)     2422 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1191 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
--rw-rw-rw-   0 root         (0) root         (0)     4625 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
--rw-rw-rw-   0 root         (0) root         (0)    78610 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/impl.py
--rw-rw-rw-   0 root         (0) root         (0)     8915 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/notifier.py
--rw-rw-rw-   0 root         (0) root         (0)    10298 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/persistence/sql/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.939592 buildgrid-0.0.92/buildgrid/server/redis/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/redis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6197 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/redis/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/request_metadata_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.940591 buildgrid-0.0.92/buildgrid/server/s3/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/s3/s3utils.py
--rw-rw-rw-   0 root         (0) root         (0)    30687 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/server.py
--rw-rw-rw-   0 root         (0) root         (0)     6126 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/servicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.940591 buildgrid-0.0.92/buildgrid/server/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/sql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22206 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/sql/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     6225 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/sql/sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.941592 buildgrid-0.0.92/buildgrid/server/utils/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/utils/async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/utils/context.py
--rw-rw-rw-   0 root         (0) root         (0)    10885 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/server/utils/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5450 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    12244 2024-04-18 10:43:42.000000 buildgrid-0.0.92/buildgrid/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.954592 buildgrid-0.0.92/buildgrid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6265 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21169 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      995 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-18 10:44:10.000000 buildgrid-0.0.92/buildgrid.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.850591 buildgrid-0.0.92/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.946592 buildgrid-0.0.92/data/config/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/all-in-one.yml
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/artifacts.yml
--rwxrwxrwx   0 root         (0) root         (0)     1351 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/basic-with-disk.yml
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/bots-interface.yml
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/default.yml
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/index-sqlite-no-execution.yml
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/index-sqlite.yml
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/logstream.yml
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/monitoring-controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/multi-layer-storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/redis-cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/s3-indexed-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/storage-redis.yml
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/storage-s3.yml
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/with-metering.yml
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-18 10:43:42.000000 buildgrid-0.0.92/data/config/with-pgbouncer.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.946592 buildgrid-0.0.92/docs/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.946592 buildgrid-0.0.92/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.948592 buildgrid-0.0.92/docs/source/data/
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/basic-disk-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/bazel-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/buildstream-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      446 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/cas-and-ac.yml
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/cas-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/execution-and-bots.yml
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/data/sqlite-index-cas-only.yml
--rw-rw-rw-   0 root         (0) root         (0)     1425 2024-04-18 10:43:42.000000 buildgrid-0.0.92/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5120 2024-04-18 10:43:42.000000 buildgrid-0.0.92/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-18 10:44:10.960592 buildgrid-0.0.92/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      643 2024-04-18 10:43:42.000000 buildgrid-0.0.92/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.950592 buildgrid-0.0.92/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.851591 buildgrid-0.0.92/tests/auth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:44:10.953592 buildgrid-0.0.92/tests/auth/data/
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/auth.yaml
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwks-valid.json
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-conflicting.secret
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-matching.secret
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-hs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-conflicting.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-jwk-encrypted.token
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-matching.priv.key
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-matching.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/auth/data/jwt-rs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)     3829 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15407 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_execution_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     2199 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)    12358 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_multithreaded_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_request_metadata_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32384 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    10567 2024-04-18 10:43:42.000000 buildgrid-0.0.92/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.819027 buildgrid-0.0.93/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-26 14:31:00.000000 buildgrid-0.0.93/BuildGrid.doap
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-26 14:31:00.000000 buildgrid-0.0.93/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11338 2024-04-26 14:31:00.000000 buildgrid-0.0.93/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-04-26 14:31:00.000000 buildgrid-0.0.93/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6931 2024-04-26 14:31:28.819027 buildgrid-0.0.93/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-26 14:31:00.000000 buildgrid-0.0.93/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.713609 buildgrid-0.0.93/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.715443 buildgrid-0.0.93/buildgrid/_app/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5661 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.718193 buildgrid-0.0.93/buildgrid/_app/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_browser_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10608 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_cas.py
+-rw-rw-rw-   0 root         (0) root         (0)     8817 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)    12570 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_janitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_operation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8166 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/cmd_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/commands/rpc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.719109 buildgrid-0.0.93/buildgrid/_app/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   110917 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     8691 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/reference.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.719109 buildgrid-0.0.93/buildgrid/_app/settings/schemas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.720026 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/with-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.720943 buildgrid-0.0.93/buildgrid/_app/settings/schemas/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/clients/asset-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.720943 buildgrid-0.0.93/buildgrid/_app/settings/schemas/connections/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/connections/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/connections/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.720943 buildgrid-0.0.93/buildgrid/_app/settings/schemas/misc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/misc/channel.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.721859 buildgrid-0.0.93/buildgrid/_app/settings/schemas/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/scheduler/memory.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/scheduler/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.723693 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      971 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/bots.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/bytestream.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/cas.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/execution.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/platform-queues.yml
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.726443 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/disk.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/lru.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/redis-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      601 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/remote.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/replicated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/s3.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/sharded.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/sql-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/sql.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/with-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4776 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.726443 buildgrid-0.0.93/buildgrid/_protos/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.726443 buildgrid-0.0.93/buildgrid/_protos/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.727359 buildgrid-0.0.93/buildgrid/_protos/build/bazel/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.727359 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.727359 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:31:01.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.730109 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7795 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    27103 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15404 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    15550 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.730109 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.731943 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30140 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   136470 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    47588 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    47884 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.731943 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.733776 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7844 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.735609 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.736526 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 14:31:01.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.736526 buildgrid-0.0.93/buildgrid/_protos/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.741109 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9955 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.742026 buildgrid-0.0.93/buildgrid/_protos/google/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.746610 buildgrid-0.0.93/buildgrid/_protos/google/api/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18246 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.748443 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7478 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     8880 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     8996 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.748443 buildgrid-0.0.93/buildgrid/_protos/google/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.749359 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.753943 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18014 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5408 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6758 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.753943 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.759443 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    23457 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7140 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7256 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21890 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5337 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9321 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.762193 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7133 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.766776 buildgrid-0.0.93/buildgrid/_protos/google/rpc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    13407 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4774 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.767693 buildgrid-0.0.93/buildgrid/browser/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/browser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/browser/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    34436 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/browser/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/browser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.767693 buildgrid-0.0.93/buildgrid/cleanup/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9520 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/cleanup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.768610 buildgrid-0.0.93/buildgrid/cleanup/janitor/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3318 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     4565 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/cleanup/janitor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.771360 buildgrid-0.0.93/buildgrid/client/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5099 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/auth_token_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/authentication.py
+-rwxrwxrwx   0 root         (0) root         (0)     1650 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    41408 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/cas.py
+-rw-rw-rw-   0 root         (0) root         (0)    13926 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/interceptors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3410 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/client/retrier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.775026 buildgrid-0.0.93/buildgrid/server/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.775943 buildgrid-0.0.93/buildgrid/server/actioncache/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.777776 buildgrid-0.0.93/buildgrid/server/actioncache/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5564 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/action_cache_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5593 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4197 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6534 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/redis_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6573 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/remote_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    11662 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/s3_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/caches/write_once_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/actioncache/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.778693 buildgrid-0.0.93/buildgrid/server/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/auth/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.779610 buildgrid-0.0.93/buildgrid/server/bots/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/bots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11154 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/bots/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7343 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/bots/job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)     5647 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/bots/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.780526 buildgrid-0.0.93/buildgrid/server/build_events/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/build_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/build_events/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7213 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/build_events/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.781443 buildgrid-0.0.93/buildgrid/server/capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/capabilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7113 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/capabilities/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     3342 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/capabilities/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.781443 buildgrid-0.0.93/buildgrid/server/cas/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21869 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)    11124 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.785110 buildgrid-0.0.93/buildgrid/server/cas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.786027 buildgrid-0.0.93/buildgrid/server/cas/storage/index/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/index_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13464 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)    38426 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.786943 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/lru_memory_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/remote.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/replicated.py
+-rw-rw-rw-   0 root         (0) root         (0)    14426 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     6002 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/sharded.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/size_differentiated.py
+-rw-rw-rw-   0 root         (0) root         (0)     9519 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8154 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/storage_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7796 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/cas/storage/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.787860 buildgrid-0.0.93/buildgrid/server/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9599 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/execution/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7517 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/execution/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/job_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    18121 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/metrics_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    14482 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19548 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.787860 buildgrid-0.0.93/buildgrid/server/operations/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.789693 buildgrid-0.0.93/buildgrid/server/operations/filtering/
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/filter_grammar.lark
+-rw-rw-rw-   0 root         (0) root         (0)     5769 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/interpreter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/filtering/sanitizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4802 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/operations/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.789693 buildgrid-0.0.93/buildgrid/server/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.790610 buildgrid-0.0.93/buildgrid/server/persistence/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.791526 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/README
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.797026 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
+-rw-rw-rw-   0 root         (0) root         (0)     4625 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    79385 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     8915 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    10298 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/persistence/sql/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.797026 buildgrid-0.0.93/buildgrid/server/redis/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/redis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6197 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/redis/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/request_metadata_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.797943 buildgrid-0.0.93/buildgrid/server/s3/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/s3/s3utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    30687 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     6126 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/servicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.798860 buildgrid-0.0.93/buildgrid/server/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/sql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22206 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/sql/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/sql/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.799777 buildgrid-0.0.93/buildgrid/server/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/utils/async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/utils/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    10885 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/server/utils/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    12244 2024-04-26 14:31:00.000000 buildgrid-0.0.93/buildgrid/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.811693 buildgrid-0.0.93/buildgrid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6931 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21169 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 14:31:28.000000 buildgrid-0.0.93/buildgrid.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.709026 buildgrid-0.0.93/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.803443 buildgrid-0.0.93/data/config/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/all-in-one.yml
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/artifacts.yml
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/basic-with-disk.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/bots-interface.yml
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/default.yml
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/index-sqlite-no-execution.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/index-sqlite.yml
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/logstream.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/monitoring-controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/multi-layer-storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/redis-cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/s3-indexed-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/storage-redis.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/storage-s3.yml
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/with-metering.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-26 14:31:01.000000 buildgrid-0.0.93/data/config/with-pgbouncer.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.803443 buildgrid-0.0.93/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.804360 buildgrid-0.0.93/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.806193 buildgrid-0.0.93/docs/source/data/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/basic-disk-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/bazel-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/buildstream-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/cas-and-ac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/cas-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/execution-and-bots.yml
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/data/sqlite-index-cas-only.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2024-04-26 14:31:01.000000 buildgrid-0.0.93/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2024-04-26 14:31:01.000000 buildgrid-0.0.93/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-26 14:31:28.819943 buildgrid-0.0.93/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      643 2024-04-26 14:31:01.000000 buildgrid-0.0.93/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.808943 buildgrid-0.0.93/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.709943 buildgrid-0.0.93/tests/auth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:31:28.811693 buildgrid-0.0.93/tests/auth/data/
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/auth.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwks-valid.json
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-conflicting.secret
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-matching.secret
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-hs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-conflicting.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-jwk-encrypted.token
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-matching.priv.key
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-matching.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/auth/data/jwt-rs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)     3829 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15407 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_execution_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_multithreaded_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_request_metadata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32384 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    10567 2024-04-26 14:31:01.000000 buildgrid-0.0.93/tests/test_utils.py
```

### Comparing `buildgrid-0.0.92/BuildGrid.doap` & `buildgrid-0.0.93/BuildGrid.doap`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/CONTRIBUTING.rst` & `buildgrid-0.0.93/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/LICENSE` & `buildgrid-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/PKG-INFO` & `buildgrid-0.0.93/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.92
+Version: 0.0.93
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -80,14 +80,28 @@
 Requires-Dist: memray; extra == "dev"
 Provides-Extra: mypy
 Requires-Dist: mypy; extra == "mypy"
 Requires-Dist: grpc-stubs>=1.53; extra == "mypy"
 Requires-Dist: boto3-stubs; extra == "mypy"
 Requires-Dist: mypy-boto3-s3; extra == "mypy"
 Requires-Dist: sqlalchemy2-stubs<=0.0.2a22; extra == "mypy"
+Requires-Dist: types-aiofiles; extra == "mypy"
+Requires-Dist: types-cachetools; extra == "mypy"
+Requires-Dist: types-docutils; extra == "mypy"
+Requires-Dist: types-jsonschema; extra == "mypy"
+Requires-Dist: types-protobuf; extra == "mypy"
+Requires-Dist: types-psycopg2; extra == "mypy"
+Requires-Dist: types-pycurl; extra == "mypy"
+Requires-Dist: types-Pygments; extra == "mypy"
+Requires-Dist: types-pyOpenSSL; extra == "mypy"
+Requires-Dist: types-python-dateutil; extra == "mypy"
+Requires-Dist: types-redis; extra == "mypy"
+Requires-Dist: types-requests; extra == "mypy"
+Requires-Dist: types-setuptools; extra == "mypy"
+Requires-Dist: types-urllib3; extra == "mypy"
 Provides-Extra: all
 Requires-Dist: buildgrid[auth,browser,database,dev,docs,mypy,redis,tests]; extra == "all"
 
 .. image:: https://gitlab.com/BuildGrid/buildgrid/badges/master/pipeline.svg
     :target: https://gitlab.com/BuildGrid/buildgrid/-/commits/master
     :alt: pipeline status
```

### Comparing `buildgrid-0.0.92/README.rst` & `buildgrid-0.0.93/README.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/__init__.py` & `buildgrid-0.0.93/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/__init__.py` & `buildgrid-0.0.93/buildgrid/_app/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/cli.py` & `buildgrid-0.0.93/buildgrid/_app/cli.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/__init__.py` & `buildgrid-0.0.93/buildgrid/_app/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_actioncache.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_browser_backend.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_browser_backend.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_capabilities.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_cas.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_cleanup.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_execute.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_execute.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_janitor.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_janitor.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_logstream.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_operation.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_operation.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/cmd_server.py` & `buildgrid-0.0.93/buildgrid/_app/commands/cmd_server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/commands/rpc_utils.py` & `buildgrid-0.0.93/buildgrid/_app/commands/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/__init__.py` & `buildgrid-0.0.93/buildgrid/_app/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/parser.py` & `buildgrid-0.0.93/buildgrid/_app/settings/parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/reference.yml` & `buildgrid-0.0.93/buildgrid/_app/settings/reference.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/config.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/config.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/connections/sql.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/connections/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/misc/channel.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/misc/channel.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/scheduler/sql.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/scheduler/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/action-cache.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/bots.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/bots.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/execution.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/execution.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/remote.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/remote.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/s3.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/s3.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_app/settings/schemas/storage/sql-index.yaml` & `buildgrid-0.0.93/buildgrid/_app/settings/schemas/storage/sql-index.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_enums.py` & `buildgrid-0.0.93/buildgrid/_enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_exceptions.py` & `buildgrid-0.0.93/buildgrid/_exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py` & `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py` & `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py` & `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py` & `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/__init__.py` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2.py` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi` & `buildgrid-0.0.93/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_types.py` & `buildgrid-0.0.93/buildgrid/_types.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/_version.py` & `buildgrid-0.0.93/buildgrid/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.0.92"
+__version__ = "0.0.93"
```

### Comparing `buildgrid-0.0.92/buildgrid/browser/__init__.py` & `buildgrid-0.0.93/buildgrid/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/browser/app.py` & `buildgrid-0.0.93/buildgrid/browser/app.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/browser/rest_api.py` & `buildgrid-0.0.93/buildgrid/browser/rest_api.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/browser/utils.py` & `buildgrid-0.0.93/buildgrid/browser/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/cleanup/__init__.py` & `buildgrid-0.0.93/buildgrid/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/cleanup/cleanup.py` & `buildgrid-0.0.93/buildgrid/cleanup/cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/cleanup/janitor/__init__.py` & `buildgrid-0.0.93/buildgrid/cleanup/janitor/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/cleanup/janitor/config.py` & `buildgrid-0.0.93/buildgrid/cleanup/janitor/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/cleanup/janitor/index.py` & `buildgrid-0.0.93/buildgrid/cleanup/janitor/index.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/cleanup/janitor/s3.py` & `buildgrid-0.0.93/buildgrid/cleanup/janitor/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/cleanup/janitor/utils.py` & `buildgrid-0.0.93/buildgrid/cleanup/janitor/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/__init__.py` & `buildgrid-0.0.93/buildgrid/client/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/actioncache.py` & `buildgrid-0.0.93/buildgrid/client/actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/asset.py` & `buildgrid-0.0.93/buildgrid/client/asset.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/auth_token_loader.py` & `buildgrid-0.0.93/buildgrid/client/auth_token_loader.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/authentication.py` & `buildgrid-0.0.93/buildgrid/client/authentication.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/capabilities.py` & `buildgrid-0.0.93/buildgrid/client/capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/cas.py` & `buildgrid-0.0.93/buildgrid/client/cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/channel.py` & `buildgrid-0.0.93/buildgrid/client/channel.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/interceptors.py` & `buildgrid-0.0.93/buildgrid/client/interceptors.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/logstream.py` & `buildgrid-0.0.93/buildgrid/client/logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/client/retrier.py` & `buildgrid-0.0.93/buildgrid/client/retrier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/__init__.py` & `buildgrid-0.0.93/buildgrid/server/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/__init__.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/caches/__init__.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/caches/action_cache_abc.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/caches/action_cache_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/caches/lru_cache.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/caches/lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/caches/mirrored_cache.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/caches/mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/caches/redis_cache.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/caches/remote_cache.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/caches/remote_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/caches/s3_cache.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/caches/s3_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/caches/with_cache.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/caches/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/caches/write_once_cache.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/caches/write_once_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/instance.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/actioncache/service.py` & `buildgrid-0.0.93/buildgrid/server/actioncache/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/auth/__init__.py` & `buildgrid-0.0.93/buildgrid/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/auth/config.py` & `buildgrid-0.0.93/buildgrid/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/auth/enums.py` & `buildgrid-0.0.93/buildgrid/server/auth/enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/auth/exceptions.py` & `buildgrid-0.0.93/buildgrid/server/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/auth/manager.py` & `buildgrid-0.0.93/buildgrid/server/auth/manager.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/bots/__init__.py` & `buildgrid-0.0.93/buildgrid/server/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/bots/instance.py` & `buildgrid-0.0.93/buildgrid/server/bots/instance.py`

 * *Files 26% similar despite different names*

```diff
@@ -94,112 +94,128 @@
             raise InvalidArgumentError("Bot's id must be set by client.")
 
         # Create new record
         bot_session.name = self.scheduler.add_bot_entry(
             bot_session_id=bot_session.bot_id, bot_session_status=bot_session.status
         )
 
-        LOGGER.info(f"Opened BotSession name=[{bot_session.name}] for bot_id=[{bot_session.bot_id}].")
-
+        LOGGER.info(f"Created new BotSession. Requesting leases. {self._bot_log_tags(bot_session)}")
         self._request_leases(bot_session, context, deadline=deadline)
-
-        leases = ",".join(lease.id[:8] for lease in bot_session.leases)
-        LOGGER.debug(
-            f"Leases assigned to newly opened BotSession name=[{bot_session.name}] "
-            f"for bot_id=[{bot_session.bot_id}]: [{leases}]."
-        )
-
-        # Update status for bot session
         self._assign_deadline_for_botsession(bot_session)
 
+        LOGGER.debug(f"Completed CreateBotSession. {self._bot_log_tags(bot_session)}")
         return bot_session
 
     update_bot_session_ignored_exceptions = (RetriableError,)
 
     @DurationMetric(BOTS_UPDATE_BOT_SESSION_TIME_METRIC_NAME, instanced=True)
     @ExceptionCounter(
         BOTS_UPDATE_BOT_SESSION_EXCEPTION_COUNT_METRIC_NAME, ignored_exceptions=update_bot_session_ignored_exceptions
     )
     def update_bot_session(
         self, bot_session: BotSession, context: CancellationContext, deadline: Optional[float] = None
     ) -> Tuple[BotSession, List[Tuple[str, bytes]]]:
         """Client updates the server. Any changes in state to the Lease should be
         registered server side. Assigns available leases with work.
         """
+        LOGGER.debug(f"Beginning initial lease synchronization. {self._bot_log_tags(bot_session)}")
 
         orig_lease: Optional[Lease] = None
         if bot_session.leases:
             orig_lease = bot_session.leases.pop()
+
         if updated_lease := self.scheduler.synchronize_bot_lease(
             bot_session.name, bot_session.bot_id, bot_session.status, orig_lease
         ):
             bot_session.leases.append(updated_lease)
 
+        LOGGER.debug(f"Completed initial lease synchronization. {self._bot_log_tags(bot_session)}")
+
         # Don't request new leases if a lease was removed. This mitigates situations where the scheduler
         # is updated with the new state of the lease, but a fault thereafter causes the worker to retry
         # the old UpdateBotSession call
         if not orig_lease and not updated_lease:
             self._request_leases(bot_session, context, deadline=deadline)
 
         metadata = self.scheduler.get_metadata_for_leases(bot_session.leases)
-
-        leases = ",".join(lease.id[:8] for lease in bot_session.leases)
-        LOGGER.debug(
-            f"Sending BotSession update for name=[{bot_session.name}], "
-            f"bot_id=[{bot_session.bot_id}]: leases=[{leases}]."
-        )
-
         self._assign_deadline_for_botsession(bot_session)
 
+        LOGGER.debug(f"Completed UpdateBotSession. {self._bot_log_tags(bot_session)}")
         return bot_session, metadata
 
     def count_bots(self) -> int:
         return self.scheduler.count_bots()
 
     def count_bots_by_status(self, status: BotStatus) -> int:
         return self.scheduler.count_bots_by_status(status)
 
     def _assign_deadline_for_botsession(self, bot_session: BotSession) -> None:
-        bot_session.expire_time.FromDatetime(self.scheduler.get_bot_expiry_time(bot_session.name, bot_session.bot_id))
+        bot_session.expire_time.FromDatetime(
+            self.scheduler.refresh_bot_expiry_time(bot_session.name, bot_session.bot_id)
+        )
 
     def _request_leases(
         self,
         bot_session: BotSession,
         context: CancellationContext,
         deadline: Optional[float] = None,
     ) -> None:
-        # Only send one lease at a time currently.
-        if bot_session.status != BotStatus.OK.value or bot_session.leases:
+        # We do not assign new leases if we are not in the OK state.
+        if bot_session.status != BotStatus.OK.value:
+            LOGGER.debug(f"BotSession not healthy. Skipping lease request. {self._bot_log_tags(bot_session)}")
             return
 
-        # If no deadline is set default to the max we allow workers to
-        # long-poll for work
+        # Only send one lease at a time currently. If any leases are set we can abort the request.
+        if bot_session.leases:
+            LOGGER.debug(f"BotSession already assigned. Skipping lease request. {self._bot_log_tags(bot_session)}")
+            return
+
+        # If no deadline is set default to the max we allow workers to long-poll for work
         if deadline is None:
             deadline = MAX_WORKER_TTL
 
         # If the specified bot session keepalive timeout is greater than the
         # deadline it can result in active bot sessions being reaped
         deadline = min(deadline, self.scheduler.bot_session_keepalive_timeout)
 
-        # Use 80% of the given deadline to give time to respond
-        # but no less than NETWORK_TIMEOUT
+        # Use 80% of the given deadline to give time to respond but no less than NETWORK_TIMEOUT
         ttl = deadline * 0.8
         if ttl < NETWORK_TIMEOUT:
             LOGGER.info(
-                f"BotSession name=[{bot_session.name}] expires in less time than "
-                f"NETWORK_TIMEOUT=[{NETWORK_TIMEOUT}], no leases will be assigned"
+                f"BotSession expires in less time than NETWORK_TIMEOUT=[{NETWORK_TIMEOUT}],"
+                f" no leases will be assigned. {self._bot_log_tags(bot_session)}"
             )
             return
 
         # Wait for an update to the bot session and then resynchronize the lease.
+        LOGGER.debug(f"Waiting for job assignment. {self._bot_log_tags(bot_session)} deadline=[{deadline:.2f}]")
         with self._job_assigner.assignment_context(bot_session) as event:
             context.on_cancel(event.set)
             event.wait(ttl)
 
+        # This is a best-effort check the see if the original request is still alive. Depending on
+        # network and proxy configurations, this status may not accurately reflect the state of the
+        # client connection. If we know for certain that the request is no longer being monitored,
+        # we can exit now to avoid state changes not being acked by the bot.
+        if context.is_cancelled():
+            LOGGER.debug(f"Bot request cancelled. Skipping lease synchronization. {self._bot_log_tags(bot_session)}")
+            return
+
+        # In the case that we had a timeout, we can return without post lease synchronization. This
+        # helps deal with the case of uncommunicated cancellations from the bot request. If the bot
+        # is actually still waiting on work, this will be immediately followed up by a new request
+        # from the worker, where the initial synchronization will begin a bot ack for the pending
+        # job. In the case that the request has been abandoned, it avoids competing updates to the
+        # database records in the corresponding bots session.
+        if not event.is_set():
+            LOGGER.debug(f"Bot assignment timeout. Skipping lease synchronization. {self._bot_log_tags(bot_session)}")
+            return
+
         # Synchronize the lease again to pick up db changes.
+        LOGGER.debug(f"Synchronizing leases after job assignment wait. {self._bot_log_tags(bot_session)}")
         if lease := self.scheduler.synchronize_bot_lease(
             bot_session.name, bot_session.bot_id, bot_session.status, None
         ):
             bot_session.leases.append(lease)
 
     def _reap_expired_sessions_loop(self, shutdown_requested: threading.Event) -> None:
         LOGGER.info(
@@ -210,7 +226,21 @@
             try:
                 while self.scheduler.reap_expired_sessions():
                     if shutdown_requested.is_set():
                         break
             except Exception as exception:
                 LOGGER.exception(exception)
             shutdown_requested.wait(timeout=self.scheduler.poll_interval)
+
+    def _bot_log_tags(self, bot_session: BotSession) -> str:
+        log_tags = (
+            f"instance_name=[{self._instance_name}]"
+            f" request.bot_name=[{bot_session.name}]"
+            f" request.bot_id=[{bot_session.bot_id}]"
+            f" request.bot_status=[{bot_session.status}]"
+        )
+        if bot_session.leases:
+            lease = bot_session.leases[0]
+            log_tags += f"request.lease_id=[{lease.id}] request.lease_state=[{lease.state}]"
+        else:
+            log_tags += "request.lease_id=[] request.lease_state=[]"
+        return log_tags
```

### Comparing `buildgrid-0.0.92/buildgrid/server/bots/job_assigner.py` & `buildgrid-0.0.93/buildgrid/server/bots/job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/bots/service.py` & `buildgrid-0.0.93/buildgrid/server/bots/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/build_events/__init__.py` & `buildgrid-0.0.93/buildgrid/server/build_events/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/build_events/service.py` & `buildgrid-0.0.93/buildgrid/server/build_events/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/build_events/storage.py` & `buildgrid-0.0.93/buildgrid/server/build_events/storage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/capabilities/__init__.py` & `buildgrid-0.0.93/buildgrid/server/capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/capabilities/instance.py` & `buildgrid-0.0.93/buildgrid/server/capabilities/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/capabilities/service.py` & `buildgrid-0.0.93/buildgrid/server/capabilities/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/__init__.py` & `buildgrid-0.0.93/buildgrid/server/cas/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/instance.py` & `buildgrid-0.0.93/buildgrid/server/cas/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/service.py` & `buildgrid-0.0.93/buildgrid/server/cas/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/__init__.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/disk.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/disk.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/index/__init__.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/index/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/index/index_abc.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/index/index_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/index/redis.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/index/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/lru_memory_cache.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/lru_memory_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/redis.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/remote.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/remote.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/replicated.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/replicated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/s3.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/sharded.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/sharded.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/size_differentiated.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/size_differentiated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/sql.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/storage_abc.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/storage_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/cas/storage/with_cache.py` & `buildgrid-0.0.93/buildgrid/server/cas/storage/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/context.py` & `buildgrid-0.0.93/buildgrid/server/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/controller.py` & `buildgrid-0.0.93/buildgrid/server/controller.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/execution/__init__.py` & `buildgrid-0.0.93/buildgrid/server/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/execution/instance.py` & `buildgrid-0.0.93/buildgrid/server/execution/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/execution/service.py` & `buildgrid-0.0.93/buildgrid/server/execution/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/job_metrics.py` & `buildgrid-0.0.93/buildgrid/server/job_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/metrics_names.py` & `buildgrid-0.0.93/buildgrid/server/metrics_names.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/metrics_utils.py` & `buildgrid-0.0.93/buildgrid/server/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/monitoring.py` & `buildgrid-0.0.93/buildgrid/server/monitoring.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/operations/__init__.py` & `buildgrid-0.0.93/buildgrid/server/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/operations/filtering/__init__.py` & `buildgrid-0.0.93/buildgrid/server/operations/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/operations/filtering/filter.py` & `buildgrid-0.0.93/buildgrid/server/operations/filtering/filter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/operations/filtering/filter_grammar.lark` & `buildgrid-0.0.93/buildgrid/server/operations/filtering/filter_grammar.lark`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/operations/filtering/interpreter.py` & `buildgrid-0.0.93/buildgrid/server/operations/filtering/interpreter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/operations/filtering/parser.py` & `buildgrid-0.0.93/buildgrid/server/operations/filtering/parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/operations/filtering/sanitizer.py` & `buildgrid-0.0.93/buildgrid/server/operations/filtering/sanitizer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/operations/instance.py` & `buildgrid-0.0.93/buildgrid/server/operations/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/operations/service.py` & `buildgrid-0.0.93/buildgrid/server/operations/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/__init__.py` & `buildgrid-0.0.93/buildgrid/server/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/__init__.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/env.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/env.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/script.py.mako` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/impl.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import logging
 import threading
 import uuid
 from contextlib import ExitStack
 from datetime import datetime, timedelta
 from time import time
-from typing import Any, Dict, Iterable, List, NamedTuple, Optional, Set, Tuple, TypedDict, TypeVar, Union, cast
+from typing import Any, Dict, Iterable, List, NamedTuple, Optional, Set, Tuple, TypedDict, TypeVar, Union
 
 from buildgrid_metering.client import SyncMeteringServiceClient
 from buildgrid_metering.models.dataclasses import ComputingUsage, Identity, Usage
 from google.protobuf.any_pb2 import Any as ProtoAny
 from google.protobuf.internal.containers import RepeatedCompositeFieldContainer
 from grpc import Channel
 from sqlalchemy import and_, delete, func, literal_column, or_, select, union, update
@@ -1437,22 +1437,37 @@
             return session.query(BotEntry).filter(self._bot_in_instance()).count()
 
     def count_bots_by_status(self, status: BotStatus) -> int:
         """Count the number of bots with a particular status"""
         with self._sql.session() as session:
             return session.query(BotEntry).filter(self._bot_in_instance(), BotEntry.bot_status == status.value).count()
 
-    def get_bot_expiry_time(self, bot_name: str, bot_id: str) -> datetime:
-        locate_bot_stmt = select(BotEntry).where(
-            BotEntry.name == bot_name, BotEntry.bot_id == bot_id, self._bot_in_instance()
+    def refresh_bot_expiry_time(self, bot_name: str, bot_id: str) -> datetime:
+        """
+        This update is done out-of-band from the main synchronize_bot_lease transaction, as there
+        are cases where we will skip calling the synchronization, but still want the session to be
+        updated such that it does not get reaped. This slightly duplicates the update happening in
+        synchronize_bot_lease, however, that update is still required to not have the job reaped
+        during its job assignment waiting period.
+
+        This method should be called at the end of the update and create bot session methods.
+        The returned datetime should be assigned to the deadline within the returned session proto.
+        """
+
+        locate_bot_stmt = (
+            select(BotEntry)
+            .where(BotEntry.name == bot_name, BotEntry.bot_id == bot_id, self._bot_in_instance())
+            .with_for_update()
         )
-        with self._sql_ro.session() as session:
+        with self._sql.session() as session:
             if bot := session.execute(locate_bot_stmt).scalar():
-                # Note this value will always be set. DB model needs to be updated to reflect.
-                return cast(datetime, bot.expiry_time)
+                now = datetime.utcnow()
+                bot.last_update_timestamp = now
+                bot.expiry_time = now + timedelta(seconds=self.bot_session_keepalive_timeout)
+                return bot.expiry_time
         raise BotSessionClosedError(f"Bot not found to fetch expiry. {bot_name=} {bot_id=}")
 
     def get_metadata_for_leases(self, leases: Iterable[Lease]) -> List[Tuple[str, bytes]]:
         """Return a list of Job metadata for a given list of leases.
 
         Args:
             leases (list): List of leases to get Job metadata for.
```

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/models.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/models.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/notifier.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/notifier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/persistence/sql/utils.py` & `buildgrid-0.0.93/buildgrid/server/persistence/sql/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/redis/__init__.py` & `buildgrid-0.0.93/buildgrid/server/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/redis/provider.py` & `buildgrid-0.0.93/buildgrid/server/redis/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/request_metadata_utils.py` & `buildgrid-0.0.93/buildgrid/server/request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/s3/__init__.py` & `buildgrid-0.0.93/buildgrid/server/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/s3/s3utils.py` & `buildgrid-0.0.93/buildgrid/server/s3/s3utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/server.py` & `buildgrid-0.0.93/buildgrid/server/server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/servicer.py` & `buildgrid-0.0.93/buildgrid/server/servicer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/sql/__init__.py` & `buildgrid-0.0.93/buildgrid/server/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/sql/provider.py` & `buildgrid-0.0.93/buildgrid/server/sql/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/sql/sqlutils.py` & `buildgrid-0.0.93/buildgrid/server/sql/sqlutils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/threading.py` & `buildgrid-0.0.93/buildgrid/server/threading.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/utils/__init__.py` & `buildgrid-0.0.93/buildgrid/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/utils/async_lru_cache.py` & `buildgrid-0.0.93/buildgrid/server/utils/async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/server/utils/context.py` & `buildgrid-0.0.93/buildgrid/server/utils/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import logging
 from threading import Event
 from typing import Callable, List
 
 from grpc import ServicerContext
 
+LOGGER = logging.getLogger(__name__)
+
 
 class CancellationContext:
     def __init__(self, context: ServicerContext) -> None:
         """
         Creates a wrapper for a grpc.ServicerContext which allows determining if a gRPC request has been
         cancelled by the client. Callbacks may be added to this context which will be invoked if the
         underlying grpc.ServicerContext is triggered.
@@ -17,14 +20,15 @@
         self._callbacks: List[Callable[[], None]] = []
         context.add_callback(self._on_callback)
 
     def is_cancelled(self) -> bool:
         return self._event.is_set()
 
     def _on_callback(self) -> None:
+        LOGGER.debug("Request cancelled")
         self._event.set()
         for callback in self._callbacks:
             callback()
 
     def on_cancel(self, callback: Callable[[], None]) -> None:
         self._callbacks.append(callback)
         if self.is_cancelled():
```

### Comparing `buildgrid-0.0.92/buildgrid/server/utils/decorators.py` & `buildgrid-0.0.93/buildgrid/server/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/settings.py` & `buildgrid-0.0.93/buildgrid/settings.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid/utils.py` & `buildgrid-0.0.93/buildgrid/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid.egg-info/PKG-INFO` & `buildgrid-0.0.93/buildgrid.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.92
+Version: 0.0.93
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -80,14 +80,28 @@
 Requires-Dist: memray; extra == "dev"
 Provides-Extra: mypy
 Requires-Dist: mypy; extra == "mypy"
 Requires-Dist: grpc-stubs>=1.53; extra == "mypy"
 Requires-Dist: boto3-stubs; extra == "mypy"
 Requires-Dist: mypy-boto3-s3; extra == "mypy"
 Requires-Dist: sqlalchemy2-stubs<=0.0.2a22; extra == "mypy"
+Requires-Dist: types-aiofiles; extra == "mypy"
+Requires-Dist: types-cachetools; extra == "mypy"
+Requires-Dist: types-docutils; extra == "mypy"
+Requires-Dist: types-jsonschema; extra == "mypy"
+Requires-Dist: types-protobuf; extra == "mypy"
+Requires-Dist: types-psycopg2; extra == "mypy"
+Requires-Dist: types-pycurl; extra == "mypy"
+Requires-Dist: types-Pygments; extra == "mypy"
+Requires-Dist: types-pyOpenSSL; extra == "mypy"
+Requires-Dist: types-python-dateutil; extra == "mypy"
+Requires-Dist: types-redis; extra == "mypy"
+Requires-Dist: types-requests; extra == "mypy"
+Requires-Dist: types-setuptools; extra == "mypy"
+Requires-Dist: types-urllib3; extra == "mypy"
 Provides-Extra: all
 Requires-Dist: buildgrid[auth,browser,database,dev,docs,mypy,redis,tests]; extra == "all"
 
 .. image:: https://gitlab.com/BuildGrid/buildgrid/badges/master/pipeline.svg
     :target: https://gitlab.com/BuildGrid/buildgrid/-/commits/master
     :alt: pipeline status
```

### Comparing `buildgrid-0.0.92/buildgrid.egg-info/SOURCES.txt` & `buildgrid-0.0.93/buildgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/buildgrid.egg-info/requires.txt` & `buildgrid-0.0.93/buildgrid.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -52,14 +52,28 @@
 
 [mypy]
 mypy
 grpc-stubs>=1.53
 boto3-stubs
 mypy-boto3-s3
 sqlalchemy2-stubs<=0.0.2a22
+types-aiofiles
+types-cachetools
+types-docutils
+types-jsonschema
+types-protobuf
+types-psycopg2
+types-pycurl
+types-Pygments
+types-pyOpenSSL
+types-python-dateutil
+types-redis
+types-requests
+types-setuptools
+types-urllib3
 
 [redis]
 fakeredis>=2.10.1
 redis>=4.5.1
 hiredis
 
 [tests]
```

### Comparing `buildgrid-0.0.92/data/config/all-in-one.yml` & `buildgrid-0.0.93/data/config/all-in-one.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/artifacts.yml` & `buildgrid-0.0.93/data/config/artifacts.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/basic-with-disk.yml` & `buildgrid-0.0.93/data/config/basic-with-disk.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/bots-interface.yml` & `buildgrid-0.0.93/data/config/bots-interface.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/cache.yml` & `buildgrid-0.0.93/data/config/cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/controller.yml` & `buildgrid-0.0.93/data/config/controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/default.yml` & `buildgrid-0.0.93/data/config/default.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/index-sqlite-no-execution.yml` & `buildgrid-0.0.93/data/config/index-sqlite-no-execution.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/index-sqlite.yml` & `buildgrid-0.0.93/data/config/index-sqlite.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/monitoring-controller.yml` & `buildgrid-0.0.93/data/config/monitoring-controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/multi-layer-storage.yml` & `buildgrid-0.0.93/data/config/multi-layer-storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/redis-cache.yml` & `buildgrid-0.0.93/data/config/redis-cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/s3-indexed-cas.yml` & `buildgrid-0.0.93/data/config/s3-indexed-cas.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/storage-redis.yml` & `buildgrid-0.0.93/data/config/storage-redis.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/storage-s3.yml` & `buildgrid-0.0.93/data/config/storage-s3.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/storage.yml` & `buildgrid-0.0.93/data/config/storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/with-metering.yml` & `buildgrid-0.0.93/data/config/with-metering.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/data/config/with-pgbouncer.yml` & `buildgrid-0.0.93/data/config/with-pgbouncer.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/docs/Makefile` & `buildgrid-0.0.93/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/docs/source/data/execution-and-bots.yml` & `buildgrid-0.0.93/docs/source/data/execution-and-bots.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/docs/source/data/sqlite-index-cas-only.yml` & `buildgrid-0.0.93/docs/source/data/sqlite-index-cas-only.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/docs/source/index.rst` & `buildgrid-0.0.93/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/pyproject.toml` & `buildgrid-0.0.93/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "setuptools >= 44",
     "wheel >= 0.35",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "buildgrid"
-version = "0.0.92"
+version = "0.0.93"
 requires-python = ">=3.8"
 description = "A remote execution service"
 readme = "README.rst"
 license = {text = "Apache License, Version 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
@@ -120,14 +120,28 @@
 ]
 mypy = [
     "mypy",
     "grpc-stubs >= 1.53",  # Stub only package, should be compatible with CI.
     "boto3-stubs",
     "mypy-boto3-s3",
     "sqlalchemy2-stubs <= 0.0.2a22", # For _ConnectionFairy.dbapi_connection issue caused by 0.0.2.a23
+    "types-aiofiles",
+    "types-cachetools",
+    "types-docutils",
+    "types-jsonschema",
+    "types-protobuf",
+    "types-psycopg2",
+    "types-pycurl",
+    "types-Pygments",
+    "types-pyOpenSSL",
+    "types-python-dateutil",
+    "types-redis",
+    "types-requests",
+    "types-setuptools",
+    "types-urllib3",
 ]
 all = [
     # Use recursive dependencies to group other setups.
     "buildgrid[auth,browser,database,redis,docs,tests,mypy,dev]"
 ]
 
 [tool.setuptools]
```

### Comparing `buildgrid-0.0.92/setup.cfg` & `buildgrid-0.0.93/setup.cfg`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/setup.py` & `buildgrid-0.0.93/setup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/auth/data/auth.yaml` & `buildgrid-0.0.93/tests/auth/data/auth.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/auth/data/jwt-rs256-jwk-encrypted.token` & `buildgrid-0.0.93/tests/auth/data/jwt-rs256-jwk-encrypted.token`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/auth/data/jwt-rs256-matching.priv.key` & `buildgrid-0.0.93/tests/auth/data/jwt-rs256-matching.priv.key`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_async_lru_cache.py` & `buildgrid-0.0.93/tests/test_async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_execution_instance.py` & `buildgrid-0.0.93/tests/test_execution_instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_job_assigner.py` & `buildgrid-0.0.93/tests/test_job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_metrics_utils.py` & `buildgrid-0.0.93/tests/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_mirrored_cache.py` & `buildgrid-0.0.93/tests/test_mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_multithreaded_metrics.py` & `buildgrid-0.0.93/tests/test_multithreaded_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_parser.py` & `buildgrid-0.0.93/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_request_metadata_utils.py` & `buildgrid-0.0.93/tests/test_request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_scheduler.py` & `buildgrid-0.0.93/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.92/tests/test_utils.py` & `buildgrid-0.0.93/tests/test_utils.py`

 * *Files identical despite different names*


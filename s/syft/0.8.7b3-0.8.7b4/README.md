# Comparing `tmp/syft-0.8.7b3.tar.gz` & `tmp/syft-0.8.7b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.7b3.tar", last modified: Thu Apr 25 04:51:07 2024, max compression
+gzip compressed data, was "syft-0.8.7b4.tar", last modified: Thu Apr 25 17:33:35 2024, max compression
```

## Comparing `syft-0.8.7b3.tar` & `syft-0.8.7b4.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.878945 syft-0.8.7b3/
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-25 04:47:09.000000 syft-0.8.7b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 04:47:09.000000 syft-0.8.7b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-25 04:51:07.878945 syft-0.8.7b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-04-25 04:48:32.000000 syft-0.8.7b3/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-25 04:47:09.000000 syft-0.8.7b3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 04:47:09.000000 syft-0.8.7b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-25 04:51:07.878945 syft-0.8.7b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 04:47:09.000000 syft-0.8.7b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.818946 syft-0.8.7b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.822946 syft-0.8.7b3/src/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 04:48:01.000000 syft-0.8.7b3/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-25 04:48:01.000000 syft-0.8.7b3/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.826946 syft-0.8.7b3/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.830946 syft-0.8.7b3/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42664 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37060 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/domain_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/enclave_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/gateway_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    16329 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/sync_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)    19869 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/syncing.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.830946 syft-0.8.7b3/src/syft/custom_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/builder_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/builder_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/builder_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/runner_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/custom_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.830946 syft-0.8.7b3/src/syft/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/exceptions/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/exceptions/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.830946 syft-0.8.7b3/src/syft/img/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/img/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.834946 syft-0.8.7b3/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/enclave.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    62557 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.834946 syft-0.8.7b3/src/syft/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)    24797 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/protocol/data_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/protocol_version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.834946 syft-0.8.7b3/src/syft/protocol/releases/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/releases/0.8.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/releases/0.8.3.json
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/releases/0.8.4.json
--rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/protocol/releases/0.8.6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.838946 syft-0.8.7b3/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/third_party.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/serde/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.838946 syft-0.8.7b3/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.842946 syft-0.8.7b3/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    74147 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.842946 syft-0.8.7b3/src/syft/service/api/
--rw-r--r--   0 runner    (1001) docker     (127)    23394 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20027 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/api/api_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/api/api_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.842946 syft-0.8.7b3/src/syft/service/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/blob_storage/remote_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/blob_storage/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/blob_storage/stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/status_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    56015 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    25589 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/code_history/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code_history/code_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code_history/code_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/code_history/code_history_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28880 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.846946 syft-0.8.7b3/src/syft/service/enclave/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/job/html_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/job/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    32670 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/job/job_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/log/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/log/log_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/metadata/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/network/association_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    29706 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.850946 syft-0.8.7b3/src/syft/service/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/email_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/notifier_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/notifier_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/notifier_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/notifier/smtp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/object_search/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/object_search/migration_state_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/object_search/object_migration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/output/
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/output/output_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27131 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.854946 syft-0.8.7b3/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/queue_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.858945 syft-0.8.7b3/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50424 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.858945 syft-0.8.7b3/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.858945 syft-0.8.7b3/src/syft/service/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52902 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/diff_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/resolve_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/sync_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/sync_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/sync/sync_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.858945 syft-0.8.7b3/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21117 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/user/user_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.862945 syft-0.8.7b3/src/syft/service/worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/image_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/image_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/image_registry_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/image_registry_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_image_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_image_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_pool_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_pool_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/service/worker/worker_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/stable_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.866945 syft-0.8.7b3/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.866945 syft-0.8.7b3/src/syft/store/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/blob_storage/on_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/blob_storage/seaweedfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    26587 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37008 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.866945 syft-0.8.7b3/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/cache_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/dicttuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/syft_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    37820 2024-04-25 04:49:43.000000 syft-0.8.7b3/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/syncable_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.870945 syft-0.8.7b3/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/_std_stream_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.870945 syft-0.8.7b3/src/syft/util/notebook_ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.874945 syft-0.8.7b3/src/syft/util/notebook_ui/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/components/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    34995 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-25 04:47:09.000000 syft-0.8.7b3/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:51:07.874945 syft-0.8.7b3/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:48:02.000000 syft-0.8.7b3/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 04:51:07.000000 syft-0.8.7b3/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.699789 syft-0.8.7b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-25 17:30:03.000000 syft-0.8.7b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 17:30:03.000000 syft-0.8.7b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-25 17:33:35.699789 syft-0.8.7b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-04-25 17:31:23.000000 syft-0.8.7b4/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-25 17:30:03.000000 syft-0.8.7b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 17:30:03.000000 syft-0.8.7b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-25 17:33:35.703789 syft-0.8.7b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 17:30:03.000000 syft-0.8.7b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.643789 syft-0.8.7b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.651789 syft-0.8.7b4/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 17:30:51.000000 syft-0.8.7b4/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-25 17:30:51.000000 syft-0.8.7b4/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.655789 syft-0.8.7b4/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.655789 syft-0.8.7b4/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42850 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37060 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/domain_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/enclave_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/gateway_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16329 2024-04-25 17:32:34.000000 syft-0.8.7b4/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/sync_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19869 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/syncing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.659789 syft-0.8.7b4/src/syft/custom_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/custom_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/custom_worker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/custom_worker/builder_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/custom_worker/builder_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/custom_worker/builder_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/custom_worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/custom_worker/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/custom_worker/runner_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/custom_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.659789 syft-0.8.7b4/src/syft/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/exceptions/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/exceptions/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.659789 syft-0.8.7b4/src/syft/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/img/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.659789 syft-0.8.7b4/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63246 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.659789 syft-0.8.7b4/src/syft/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)    24797 2024-04-25 17:32:34.000000 syft-0.8.7b4/src/syft/protocol/data_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/protocol/protocol_version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.663789 syft-0.8.7b4/src/syft/protocol/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/protocol/releases/0.8.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/protocol/releases/0.8.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/protocol/releases/0.8.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/protocol/releases/0.8.6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.663789 syft-0.8.7b4/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/third_party.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/serde/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.663789 syft-0.8.7b4/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.667789 syft-0.8.7b4/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74149 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-04-25 17:32:34.000000 syft-0.8.7b4/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.667789 syft-0.8.7b4/src/syft/service/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    23496 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20027 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/api/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/api/api_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.667789 syft-0.8.7b4/src/syft/service/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/blob_storage/remote_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.671789 syft-0.8.7b4/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code/status_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56556 2024-04-25 17:32:34.000000 syft-0.8.7b4/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25576 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.671789 syft-0.8.7b4/src/syft/service/code_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.671789 syft-0.8.7b4/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.671789 syft-0.8.7b4/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28880 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.671789 syft-0.8.7b4/src/syft/service/enclave/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.675789 syft-0.8.7b4/src/syft/service/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/job/html_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/job/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32817 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/job/job_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.675789 syft-0.8.7b4/src/syft/service/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/log/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/log/log_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.675789 syft-0.8.7b4/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/metadata/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.675789 syft-0.8.7b4/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/network/association_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29706 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.675789 syft-0.8.7b4/src/syft/service/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notification/email_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.675789 syft-0.8.7b4/src/syft/service/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notifier/notifier_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notifier/notifier_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notifier/notifier_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/notifier/smtp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.679789 syft-0.8.7b4/src/syft/service/object_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/object_search/migration_state_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/object_search/object_migration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.679789 syft-0.8.7b4/src/syft/service/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/output/output_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.679789 syft-0.8.7b4/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27131 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.679789 syft-0.8.7b4/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-04-25 17:32:34.000000 syft-0.8.7b4/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.679789 syft-0.8.7b4/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/queue/queue_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.679789 syft-0.8.7b4/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50592 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.683789 syft-0.8.7b4/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/settings/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.683789 syft-0.8.7b4/src/syft/service/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53412 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/sync/diff_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20942 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/sync/resolve_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/sync/sync_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/sync/sync_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/sync/sync_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.683789 syft-0.8.7b4/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21117 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/user/user_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.687789 syft-0.8.7b4/src/syft/service/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/image_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/image_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/image_registry_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/image_registry_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/worker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/worker_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/worker_image_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/worker_pool_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/worker_pool_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/worker_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/service/worker/worker_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/stable_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.687789 syft-0.8.7b4/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.687789 syft-0.8.7b4/src/syft/store/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26587 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-25 17:32:34.000000 syft-0.8.7b4/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37008 2024-04-25 17:32:34.000000 syft-0.8.7b4/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-25 17:32:34.000000 syft-0.8.7b4/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.691789 syft-0.8.7b4/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/cache_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/dicttuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/syft_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37820 2024-04-25 17:32:34.000000 syft-0.8.7b4/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/syncable_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.695789 syft-0.8.7b4/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/_std_stream_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.695789 syft-0.8.7b4/src/syft/util/notebook_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/notebook_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.695789 syft-0.8.7b4/src/syft/util/notebook_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/notebook_ui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/notebook_ui/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/notebook_ui/components/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34946 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-25 17:30:03.000000 syft-0.8.7b4/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:33:35.695789 syft-0.8.7b4/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-25 17:33:35.000000 syft-0.8.7b4/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-25 17:33:35.000000 syft-0.8.7b4/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:33:35.000000 syft-0.8.7b4/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 17:33:35.000000 syft-0.8.7b4/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:30:52.000000 syft-0.8.7b4/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-25 17:33:35.000000 syft-0.8.7b4/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 17:33:35.000000 syft-0.8.7b4/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.7b3/LICENSE` & `syft-0.8.7b4/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/PKG-INFO` & `syft-0.8.7b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b3
+Version: 0.8.7b4
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

### Comparing `syft-0.8.7b3/PYPI.md` & `syft-0.8.7b4/PYPI.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/README.md` & `syft-0.8.7b4/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/setup.cfg` & `syft-0.8.7b4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.7-beta.3"
+version = attr: "0.8.7-beta.4"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: PYPI.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.7b3/src/syft/VERSION` & `syft-0.8.7b4/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.7-beta.3"
+__version__ = "0.8.7-beta.4"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.7b3/src/syft/__init__.py` & `syft-0.8.7b4/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.7-beta.3"
+__version__ = "0.8.7-beta.4"
 
 # stdlib
 from collections.abc import Callable
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
```

### Comparing `syft-0.8.7b3/src/syft/abstract_node.py` & `syft-0.8.7b4/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/api.py` & `syft-0.8.7b4/src/syft/client/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,21 +369,24 @@
             str_repr = "## API: " + custom_path + "\n"
             str_repr += (
                 "### Description: "
                 + f'<span style="font-weight: lighter;">{endpoint.description}</span><br>'
                 + "\n"
             )
             str_repr += "#### Private Code:\n"
-            str_repr += as_markdown_python_code(endpoint.private_function) + "\n"
+            not_accessible_code = "N / A"
+            private_code_repr = endpoint.private_function or not_accessible_code
+            public_code_repr = endpoint.mock_function or not_accessible_code
+            str_repr += as_markdown_python_code(private_code_repr) + "\n"
             if endpoint.private_helper_functions:
                 str_repr += "##### Helper Functions:\n"
                 for helper_function in endpoint.private_helper_functions:
                     str_repr += as_markdown_python_code(helper_function) + "\n"
             str_repr += "#### Public Code:\n"
-            str_repr += as_markdown_python_code(endpoint.mock_function) + "\n"
+            str_repr += as_markdown_python_code(public_code_repr) + "\n"
             if endpoint.mock_helper_functions:
                 str_repr += "##### Helper Functions:\n"
                 for helper_function in endpoint.mock_helper_functions:
                     str_repr += as_markdown_python_code(helper_function) + "\n"
             return str_repr
         return super()._repr_markdown_()
```

### Comparing `syft-0.8.7b3/src/syft/client/client.py` & `syft-0.8.7b4/src/syft/client/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/connection.py` & `syft-0.8.7b4/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/deploy.py` & `syft-0.8.7b4/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/domain_client.py` & `syft-0.8.7b4/src/syft/client/domain_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/enclave_client.py` & `syft-0.8.7b4/src/syft/client/enclave_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/gateway_client.py` & `syft-0.8.7b4/src/syft/client/gateway_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/registry.py` & `syft-0.8.7b4/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/search.py` & `syft-0.8.7b4/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/sync_decision.py` & `syft-0.8.7b4/src/syft/client/sync_decision.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/syncing.py` & `syft-0.8.7b4/src/syft/client/syncing.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/client/user_settings.py` & `syft-0.8.7b4/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/custom_worker/builder.py` & `syft-0.8.7b4/src/syft/custom_worker/builder.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/custom_worker/builder_docker.py` & `syft-0.8.7b4/src/syft/custom_worker/builder_docker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/custom_worker/builder_k8s.py` & `syft-0.8.7b4/src/syft/custom_worker/builder_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/custom_worker/builder_types.py` & `syft-0.8.7b4/src/syft/custom_worker/builder_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/custom_worker/config.py` & `syft-0.8.7b4/src/syft/custom_worker/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,8 +175,11 @@
                 kwargs["fileobj"] = io.BytesIO(self.dockerfile.encode("utf-8"))
                 _, logs = client.images.build(
                     tag=tag,
                     **kwargs,
                 )
                 return SyftSuccess(message=iterator_to_string(iterator=logs))
         except Exception as e:
-            return SyftError(message=f"Failed to build: {e}")
+            # stdlib
+            import traceback
+
+            return SyftError(message=f"Failed to build: {e} {traceback.format_exc()}")
```

### Comparing `syft-0.8.7b3/src/syft/custom_worker/k8s.py` & `syft-0.8.7b4/src/syft/custom_worker/k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/custom_worker/runner_k8s.py` & `syft-0.8.7b4/src/syft/custom_worker/runner_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/custom_worker/utils.py` & `syft-0.8.7b4/src/syft/custom_worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/exceptions/exception.py` & `syft-0.8.7b4/src/syft/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/gevent_patch.py` & `syft-0.8.7b4/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/img/logo.png` & `syft-0.8.7b4/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.7b4/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/node/credentials.py` & `syft-0.8.7b4/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/node/node.py` & `syft-0.8.7b4/src/syft/node/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # future
 from __future__ import annotations
 
 # stdlib
 from collections import OrderedDict
+from collections import defaultdict
 from collections.abc import Callable
 from datetime import datetime
 from functools import partial
 import hashlib
 import os
 from pathlib import Path
 import shutil
@@ -459,14 +460,17 @@
     def stop(self) -> None:
         for consumer_list in self.queue_manager.consumers.values():
             for c in consumer_list:
                 c.close()
         for p in self.queue_manager.producers.values():
             p.close()
 
+        self.queue_manager.producers.clear()
+        self.queue_manager.consumers.clear()
+
         NodeRegistry.remove_node(self.id)
 
     def close(self) -> None:
         self.stop()
 
     def cleanup(self) -> None:
         self.stop()
@@ -563,14 +567,26 @@
             address=address,
             service_name=service_name,
             worker_stash=self.worker_stash,
             syft_worker_id=syft_worker_id,
         )
         consumer.run()
 
+    def remove_consumer_with_id(self, syft_worker_id: UID) -> None:
+        for _, consumers in self.queue_manager.consumers.items():
+            # Grab the list of consumers for the given queue
+            consumer_to_pop = None
+            for consumer_idx, consumer in enumerate(consumers):
+                if consumer.syft_worker_id == syft_worker_id:
+                    consumer.close()
+                    consumer_to_pop = consumer_idx
+                    break
+            if consumer_to_pop is not None:
+                consumers.pop(consumer_to_pop)
+
     @classmethod
     def named(
         cls,
         *,  # Trasterisk
         name: str,
         processes: int = 0,
         reset: bool = False,
```

### Comparing `syft-0.8.7b3/src/syft/node/routes.py` & `syft-0.8.7b4/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/node/run.py` & `syft-0.8.7b4/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/node/server.py` & `syft-0.8.7b4/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/node/worker_settings.py` & `syft-0.8.7b4/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/protocol/data_protocol.py` & `syft-0.8.7b4/src/syft/protocol/data_protocol.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/protocol/protocol_version.json` & `syft-0.8.7b4/src/syft/protocol/protocol_version.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/protocol/releases/0.8.2.json` & `syft-0.8.7b4/src/syft/protocol/releases/0.8.2.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/protocol/releases/0.8.3.json` & `syft-0.8.7b4/src/syft/protocol/releases/0.8.3.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/protocol/releases/0.8.4.json` & `syft-0.8.7b4/src/syft/protocol/releases/0.8.4.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/protocol/releases/0.8.6.json` & `syft-0.8.7b4/src/syft/protocol/releases/0.8.6.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/array.py` & `syft-0.8.7b4/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/arrow.py` & `syft-0.8.7b4/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/deserialize.py` & `syft-0.8.7b4/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/lib_permissions.py` & `syft-0.8.7b4/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/lib_service_registry.py` & `syft-0.8.7b4/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/mock.py` & `syft-0.8.7b4/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/recursive.py` & `syft-0.8.7b4/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/recursive_primitives.py` & `syft-0.8.7b4/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/serializable.py` & `syft-0.8.7b4/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/serialize.py` & `syft-0.8.7b4/src/syft/serde/serialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/signature.py` & `syft-0.8.7b4/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/serde/third_party.py` & `syft-0.8.7b4/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/action_data_empty.py` & `syft-0.8.7b4/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/action_endpoint.py` & `syft-0.8.7b4/src/syft/service/action/action_endpoint.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/action_graph.py` & `syft-0.8.7b4/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/action_graph_service.py` & `syft-0.8.7b4/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/action_object.py` & `syft-0.8.7b4/src/syft/service/action/action_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1901,15 +1901,15 @@
                     if (
                         self.syft_action_data_cache is not None
                         and hasattr(self.syft_action_data_cache, "_repr_markdown_")
                     )
                     else self.syft_action_data_cache.__repr__()
                 )
 
-        return f"```python\n{res}\n{data_repr_}```\n"
+        return f"```python\n{res}\n{data_repr_}\n```\n"
 
     def _data_repr(self) -> str | None:
         if isinstance(self.syft_action_data_cache, ActionDataEmpty):
             data_repr = self.syft_action_data_repr_
         elif inspect.isclass(self.syft_action_data_cache):
             data_repr = repr_cls(self.syft_action_data_cache)
         else:
```

### Comparing `syft-0.8.7b3/src/syft/service/action/action_permissions.py` & `syft-0.8.7b4/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/action_service.py` & `syft-0.8.7b4/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/action_store.py` & `syft-0.8.7b4/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/action_types.py` & `syft-0.8.7b4/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/numpy.py` & `syft-0.8.7b4/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/pandas.py` & `syft-0.8.7b4/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/plan.py` & `syft-0.8.7b4/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/action/verification.py` & `syft-0.8.7b4/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/api/api.py` & `syft-0.8.7b4/src/syft/service/api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,28 +94,34 @@
         "path",
         "signature",
         "worker_pool",
         "endpoint_timeout",
     ]
 
     def _coll_repr_(self) -> dict[str, Any]:
-        mock_parsed_code = ast.parse(self.mock_function)
-        mock_function_name = [
-            node.name
-            for node in ast.walk(mock_parsed_code)
-            if isinstance(node, ast.FunctionDef)
-        ][0]
-        private_function_name = NOT_ACCESSIBLE_STRING
-        if self.private_function != NOT_ACCESSIBLE_STRING:
+        if self.mock_function:
+            mock_parsed_code = ast.parse(self.mock_function)
+            mock_function_name = [
+                node.name
+                for node in ast.walk(mock_parsed_code)
+                if isinstance(node, ast.FunctionDef)
+            ][0]
+        else:
+            mock_function_name = NOT_ACCESSIBLE_STRING
+
+        if self.private_function:
             private_parsed_code = ast.parse(self.private_function)
             private_function_name = [
                 node.name
                 for node in ast.walk(private_parsed_code)
                 if isinstance(node, ast.FunctionDef)
             ][0]
+        else:
+            private_function_name = NOT_ACCESSIBLE_STRING
+
         worker_pool = "UNSET (DEFAULT)"
         if self.worker_pool is not None:
             worker_pool = self.worker_pool
         return {
             "API path": self.path,
             "Signature": self.path + str(self.signature),
             "Access": self.access,
@@ -553,15 +559,15 @@
                 endpoint_type.view_access or context.credentials == admin_key
             ):
                 context.output[code_field] = decorator_cleanup(endpoint_type.api_code)
                 context.output[helper_function_field] = (
                     endpoint_type.helper_functions.values() or []
                 )
             else:
-                context.output[code_field] = NOT_ACCESSIBLE_STRING
+                context.output[code_field] = None
                 context.output[helper_function_field] = []
         return context
 
     return code_string
 
 
 @transform(TwinAPIAuthedContext, TwinAPIContextView)
```

### Comparing `syft-0.8.7b3/src/syft/service/api/api_service.py` & `syft-0.8.7b4/src/syft/service/api/api_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/api/api_stash.py` & `syft-0.8.7b4/src/syft/service/api/api_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/blob_storage/remote_profile.py` & `syft-0.8.7b4/src/syft/service/blob_storage/remote_profile.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/blob_storage/service.py` & `syft-0.8.7b4/src/syft/service/blob_storage/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/blob_storage/stash.py` & `syft-0.8.7b4/src/syft/service/blob_storage/stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/code/code_parse.py` & `syft-0.8.7b4/src/syft/service/code/code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/code/status_service.py` & `syft-0.8.7b4/src/syft/service/code/status_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/code/user_code.py` & `syft-0.8.7b4/src/syft/service/code/user_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,15 +501,18 @@
                 output_blob = _serialize(output_policy, to_bytes=True)
                 self.output_policy_state = output_blob
                 return output_policy
             else:
                 raise Exception("output_policy is None during init")
 
         try:
-            return _deserialize(self.output_policy_state, from_bytes=True)
+            output_policy = _deserialize(self.output_policy_state, from_bytes=True)
+            output_policy.syft_node_location = self.syft_node_location
+            output_policy.syft_client_verify_key = self.syft_client_verify_key
+            return output_policy
         except Exception as e:
             print(f"Failed to deserialize custom output policy state. {e}")
             return None
 
     @property
     def output_policy(self) -> OutputPolicy | None:  # type: ignore
         if not self.status.approved:
@@ -1482,15 +1485,23 @@
         except Exception as e:
             error_msg = traceback_from_error(e, code_item)
             if context.job is not None:
                 time = datetime.datetime.now().strftime("%d/%m/%y %H:%M:%S")
                 original_print(
                     f"{time} EXCEPTION LOG ({job_id}):\n{error_msg}", file=sys.stderr
                 )
-            if context.node is not None:
+            else:
+                # for local execution
+                time = datetime.datetime.now().strftime("%d/%m/%y %H:%M:%S")
+                original_print(f"{time} EXCEPTION LOG:\n{error_msg}\n", file=sys.stderr)
+            if (
+                context.node is not None
+                and context.job is not None
+                and context.job.log_id is not None
+            ):
                 log_id = context.job.log_id
                 log_service = context.node.get_service("LogService")
                 log_service.append(context=context, uid=log_id, new_err=error_msg)
 
             result_message = (
                 f"Exception encountered while running {code_item.service_func_name}"
                 ", please contact the Node Admin for more info."
```

### Comparing `syft-0.8.7b3/src/syft/service/code/user_code_parse.py` & `syft-0.8.7b4/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/code/user_code_service.py` & `syft-0.8.7b4/src/syft/service/code/user_code_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,15 +546,15 @@
                     return Ok(result.private)
                 else:
                     return Ok(result.mock)
             elif result.is_mock:
                 return Ok(result)
             elif result.syft_action_data_type is Err:
                 # result contains the error but the request was handled correctly
-                return result.syft_action_data
+                return Ok(result)
             elif has_result_read_permission:
                 return Ok(result)
             else:
                 return Ok(result.as_empty())
         except Exception as e:
             # stdlib
             import traceback
```

### Comparing `syft-0.8.7b3/src/syft/service/code/user_code_stash.py` & `syft-0.8.7b4/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/code/utils.py` & `syft-0.8.7b4/src/syft/service/code/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/code_history/code_history.py` & `syft-0.8.7b4/src/syft/service/code_history/code_history.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/code_history/code_history_service.py` & `syft-0.8.7b4/src/syft/service/code_history/code_history_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/code_history/code_history_stash.py` & `syft-0.8.7b4/src/syft/service/code_history/code_history_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/context.py` & `syft-0.8.7b4/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/data_subject/data_subject.py` & `syft-0.8.7b4/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.7b4/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.7b4/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.7b4/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/dataset/dataset.py` & `syft-0.8.7b4/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/dataset/dataset_service.py` & `syft-0.8.7b4/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.7b4/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/enclave/enclave_service.py` & `syft-0.8.7b4/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/job/html_template.py` & `syft-0.8.7b4/src/syft/service/job/html_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 """
 
 logs_html = """<div id="${logs_tab_id}" class="tab-${identifier}" style="background: #F4F3F6;
 border-color: #CFCDD6; border-width: 0.5px; border-style: solid; padding: 24px; gap: 8px; margin-top: 24px;
 display: none;align-items:left">
     <div style="font-size: 12px; font-weight: 400; font: DejaVu Sans Mono, sans-serif; line-height: 16.8px; ">
         <table  style="width:100%; justify-content:left; border-collapse: collapse;">
-        <tr style="width:100%">
-            <td style="text-align: left">
+        <tr style="width:100%; background: rgb(244, 243, 246);">
+            <td style="text-align: left; width:50px;">
                 <span style="margin-right:24px; font-weight:700; align-text: center">
                     #
                 </span>
             </td>
             <td  style="text-align: left">
                 <span style="font-weight:700; align-text: left">
                     Message
```

### Comparing `syft-0.8.7b3/src/syft/service/job/job_service.py` & `syft-0.8.7b4/src/syft/service/job/job_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/job/job_stash.py` & `syft-0.8.7b4/src/syft/service/job/job_stash.py`

 * *Files 1% similar despite different names*

```diff
@@ -605,37 +605,38 @@
         if self.requested_by:
             requesting_user = self.requesting_user
             user_repr = f"{requesting_user.name} {requesting_user.email}"
 
         worker_attr = ""
         if self.job_worker_id:
             worker = self.worker
-            worker_pool_id_button = CopyIDButton(
-                copy_text=str(worker.worker_pool_name), max_width=60
-            )
-            worker_attr = f"""
-                <div style="margin-top: 6px; margin-bottom: 6px;">
-                <span style="font-weight: 700; line-weight: 19.6px; font-size: 14px; font: 'Open Sans'">
-                    Worker Pool:</span>
-                    {worker.name} on worker {worker_pool_id_button.to_html()}
-                </div>
-            """
+            if not isinstance(worker, SyftError):
+                worker_pool_id_button = CopyIDButton(
+                    copy_text=str(worker.worker_pool_name), max_width=60
+                )
+                worker_attr = f"""
+                    <div style="margin-top: 6px; margin-bottom: 6px;">
+                    <span style="font-weight: 700; line-weight: 19.6px; font-size: 14px; font: 'Open Sans'">
+                        Worker Pool:</span>
+                        {worker.name} on worker {worker_pool_id_button.to_html()}
+                    </div>
+                """
 
-        logs = self.logs(_print=False, stderr=False)
+        logs = self.logs(_print=False)
         logs_lines = logs.split("\n") if logs else []
         logs_lines_html = ""
         for i, line in enumerate(logs_lines):
             logs_lines_html += f"""
-                <tr style="width:100%">
-                    <td style="text-align: left;">
+                <tr style="width:100%; background: rgb(244, 243, 246);">
+                    <td style="text-align: left; width: 50px;">
                         <div style="margin-right:24px; align-text: center">
                             {i}
                         </div>
                     </td>
-                    <td style="text-align: left;">
+                    <td style="text-align: left; overflow: hidden;">
                         <div style="align-text: left">
                             {line}
                         </div>
                     </td>
                 </tr>
             """
 
@@ -673,15 +674,15 @@
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
         )
         if self.resolved:
             return self.resolve
 
         if not job_only and self.result is not None:
-            self.result.wait()
+            self.result.wait(timeout)
 
         if api is None:
             raise ValueError(
                 f"Can't access Syft API. You must login to {self.syft_node_location}"
             )
         print_warning = True
         counter = 0
```

### Comparing `syft-0.8.7b3/src/syft/service/log/log.py` & `syft-0.8.7b4/src/syft/service/log/log.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/log/log_service.py` & `syft-0.8.7b4/src/syft/service/log/log_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/log/log_stash.py` & `syft-0.8.7b4/src/syft/service/log/log_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/metadata/metadata_service.py` & `syft-0.8.7b4/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/metadata/migrations.py` & `syft-0.8.7b4/src/syft/service/metadata/migrations.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/metadata/node_metadata.py` & `syft-0.8.7b4/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/network/association_request.py` & `syft-0.8.7b4/src/syft/service/network/association_request.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/network/network_service.py` & `syft-0.8.7b4/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/network/node_peer.py` & `syft-0.8.7b4/src/syft/service/network/node_peer.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/network/routes.py` & `syft-0.8.7b4/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/notification/email_templates.py` & `syft-0.8.7b4/src/syft/service/notification/email_templates.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/notification/notification_service.py` & `syft-0.8.7b4/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/notification/notification_stash.py` & `syft-0.8.7b4/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/notification/notifications.py` & `syft-0.8.7b4/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/notifier/notifier.py` & `syft-0.8.7b4/src/syft/service/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/notifier/notifier_service.py` & `syft-0.8.7b4/src/syft/service/notifier/notifier_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/notifier/notifier_stash.py` & `syft-0.8.7b4/src/syft/service/notifier/notifier_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/notifier/smtp_client.py` & `syft-0.8.7b4/src/syft/service/notifier/smtp_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/object_search/migration_state_service.py` & `syft-0.8.7b4/src/syft/service/object_search/migration_state_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/object_search/object_migration_state.py` & `syft-0.8.7b4/src/syft/service/object_search/object_migration_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/output/output_service.py` & `syft-0.8.7b4/src/syft/service/output/output_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/policy/policy.py` & `syft-0.8.7b4/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/policy/policy_service.py` & `syft-0.8.7b4/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.7b4/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/project/project.py` & `syft-0.8.7b4/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/project/project_service.py` & `syft-0.8.7b4/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/project/project_stash.py` & `syft-0.8.7b4/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/queue/base_queue.py` & `syft-0.8.7b4/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/queue/queue.py` & `syft-0.8.7b4/src/syft/service/queue/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,19 +196,23 @@
         )
 
         result: Any = call_method(context, *queue_item.args, **queue_item.kwargs)
 
         status = Status.COMPLETED
         job_status = JobStatus.COMPLETED
 
-        if isinstance(result, Ok):
+        if isinstance(result.ok().syft_action_data, Err):
+            status = Status.ERRORED
+            job_status = JobStatus.ERRORED
             result = result.ok()
         elif isinstance(result, SyftError) or isinstance(result, Err):
             status = Status.ERRORED
             job_status = JobStatus.ERRORED
+        elif isinstance(result, Ok):
+            result = result.ok()
     except Exception as e:  # nosec
         status = Status.ERRORED
         job_status = JobStatus.ERRORED
         # stdlib
 
         raise e
         # result = SyftError(
```

### Comparing `syft-0.8.7b3/src/syft/service/queue/queue_service.py` & `syft-0.8.7b4/src/syft/service/queue/queue_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/queue/queue_stash.py` & `syft-0.8.7b4/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/queue/zmq_queue.py` & `syft-0.8.7b4/src/syft/service/queue/zmq_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,28 +384,37 @@
             # TODO: fix the mypy issue
             logger.error(  # type: ignore[unreachable]
                 f"Worker stash is not defined for ZMQProducer : {self.queue_name} - {self.id}"
             )
             return
 
         try:
+            # Check if worker is present in the database
+            worker = self.worker_stash.get_by_uid(
+                credentials=self.worker_stash.partition.root_verify_key,
+                uid=syft_worker_id,
+            )
+            if worker.is_ok() and worker.ok() is None:
+                return
+
             res = self.worker_stash.update_consumer_state(
                 credentials=self.worker_stash.partition.root_verify_key,
                 worker_uid=syft_worker_id,
                 consumer_state=consumer_state,
             )
             if res.is_err():
                 logger.error(
-                    "Failed to update consumer state for worker id={} error={}",
+                    "Failed to update consumer state for worker id={} to state: {} error={}",
                     syft_worker_id,
+                    consumer_state,
                     res.err(),
                 )
         except Exception as e:
             logger.error(
-                f"Failed to update consumer state for worker id: {syft_worker_id}. Error: {e}"
+                f"Failed to update consumer state for worker id: {syft_worker_id} to state {consumer_state}. Error: {e}"
             )
 
     def worker_waiting(self, worker: Worker) -> None:
         """This worker is now waiting for work."""
         # Queue to broker and service waiting lists
         if worker not in self.waiting:
             self.waiting.append(worker)
@@ -568,17 +577,18 @@
             worker.service.waiting.remove(worker)
 
         if worker in self.waiting:
             self.waiting.remove(worker)
 
         self.workers.pop(worker.identity, None)
 
-        self.update_consumer_state_for_worker(
-            worker.syft_worker_id, ConsumerState.DETACHED
-        )
+        if worker.syft_worker_id is not None:
+            self.update_consumer_state_for_worker(
+                worker.syft_worker_id, ConsumerState.DETACHED
+            )
 
     @property
     def alive(self) -> bool:
         return not self.socket.closed
 
 
 @serializable(attrs=["_subscriber"])
@@ -629,15 +639,19 @@
 
     def post_init(self) -> None:
         self.thread: threading.Thread | None = None
         self.heartbeat_t = Timeout(HEARTBEAT_INTERVAL_SEC)
         self.producer_ping_t = Timeout(PRODUCER_TIMEOUT_SEC)
         self.reconnect_to_producer()
 
+    def disconnect_from_producer(self) -> None:
+        self.send_to_producer(QueueMsgProtocol.W_DISCONNECT)
+
     def close(self) -> None:
+        self.disconnect_from_producer()
         self._stop.set()
         try:
             self.poller.unregister(self.socket)
         except Exception as e:
             logger.exception("Failed to unregister worker. {}", e)
         finally:
             if self.thread is not None:
```

### Comparing `syft-0.8.7b3/src/syft/service/request/request.py` & `syft-0.8.7b4/src/syft/service/request/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -873,14 +873,19 @@
                 job_id=job.id,
                 input_ids=input_ids,
             )
             if isinstance(res, SyftError):
                 return res
 
         job_info.result = action_object
+        job_info.status = (
+            JobStatus.ERRORED
+            if isinstance(action_object.syft_action_data, Err)
+            else JobStatus.COMPLETED
+        )
 
         existing_result = job.result.id if job.result is not None else None
         print(
             f"Job({job.id}) Setting new result {existing_result} -> {job_info.result.id}"
         )
         job.apply_info(job_info)
```

### Comparing `syft-0.8.7b3/src/syft/service/request/request_service.py` & `syft-0.8.7b4/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/request/request_stash.py` & `syft-0.8.7b4/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/response.py` & `syft-0.8.7b4/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/service.py` & `syft-0.8.7b4/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/settings/settings.py` & `syft-0.8.7b4/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/settings/settings_service.py` & `syft-0.8.7b4/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/settings/settings_stash.py` & `syft-0.8.7b4/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/sync/diff_state.py` & `syft-0.8.7b4/src/syft/service/sync/diff_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,15 +797,22 @@
                     result.append(diff)
                     result += flatten_dict(child)
                 return result
 
         return flatten_dict(self.get_visual_hierarchy())
 
     def _repr_html_(self) -> str:
-        diffs = self.flatten_visual_hierarchy()
+        try:
+            diffs = self.flatten_visual_hierarchy()
+        except Exception as _:
+            return SyftError(
+                message=html.escape(
+                    "Could not render batch, please use resolve_single(<batch>) instead."
+                )
+            )._repr_html_()
 
         return f"""
 <h2> ObjectBatchDiff </h2>
 {diffs._repr_html_()}
 """
 
     def status_badge(self) -> dict[str, str]:
@@ -872,19 +879,26 @@
         self.dependents = dependents
         return self
 
     @property
     def root(self) -> ObjectDiff:
         return self.root_diff
 
-    def __repr__(self) -> str:
-        return f"""{self.hierarchy_str('low')}
-
-{self.hierarchy_str('high')}
-"""
+    def __repr__(self) -> Any:
+        try:
+            return f"""{self.hierarchy_str('low')}
+
+    {self.hierarchy_str('high')}
+    """
+        except Exception as _:
+            return SyftError(
+                message=html.escape(
+                    "Could not render batch, please use resolve_single(<batch>) instead."
+                )
+            )._repr_html_()
 
     def _repr_markdown_(self, wrap_as_python: bool = True, indent: int = 0) -> str:
         return ""  # Turns off the _repr_markdown_ of SyftObject
 
     def _get_visual_hierarchy(
         self, node: ObjectDiff, visited: set[UID] | None = None
     ) -> dict[ObjectDiff, dict]:
```

### Comparing `syft-0.8.7b3/src/syft/service/sync/resolve_widget.py` & `syft-0.8.7b4/src/syft/service/sync/resolve_widget.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/sync/sync_service.py` & `syft-0.8.7b4/src/syft/service/sync/sync_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/sync/sync_stash.py` & `syft-0.8.7b4/src/syft/service/sync/sync_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/sync/sync_state.py` & `syft-0.8.7b4/src/syft/service/sync/sync_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/user/user.py` & `syft-0.8.7b4/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/user/user_roles.py` & `syft-0.8.7b4/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/user/user_service.py` & `syft-0.8.7b4/src/syft/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/user/user_stash.py` & `syft-0.8.7b4/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/warnings.py` & `syft-0.8.7b4/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/image_identifier.py` & `syft-0.8.7b4/src/syft/service/worker/image_identifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/image_registry.py` & `syft-0.8.7b4/src/syft/service/worker/image_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/image_registry_service.py` & `syft-0.8.7b4/src/syft/service/worker/image_registry_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/image_registry_stash.py` & `syft-0.8.7b4/src/syft/service/worker/image_registry_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/utils.py` & `syft-0.8.7b4/src/syft/service/worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/worker.py` & `syft-0.8.7b4/src/syft/service/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/worker_image.py` & `syft-0.8.7b4/src/syft/service/worker/worker_image.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/worker_image_service.py` & `syft-0.8.7b4/src/syft/service/worker/worker_image_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/worker_image_stash.py` & `syft-0.8.7b4/src/syft/service/worker/worker_image_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/worker_pool.py` & `syft-0.8.7b4/src/syft/service/worker/worker_pool.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/worker_pool_service.py` & `syft-0.8.7b4/src/syft/service/worker/worker_pool_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/worker_pool_stash.py` & `syft-0.8.7b4/src/syft/service/worker/worker_pool_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/service/worker/worker_service.py` & `syft-0.8.7b4/src/syft/service/worker/worker_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,14 +204,17 @@
                 docker_container = _get_worker_container(client, worker)
                 if isinstance(docker_container, SyftError):
                     return docker_container
 
                 stopped = _stop_worker_container(worker, docker_container, force)
                 if stopped is not None:
                     return stopped
+        else:
+            # kill the in memory worker thread
+            context.node.remove_consumer_with_id(syft_worker_id=worker.id)
 
         # remove the worker from the pool
         try:
             worker_linked_object = next(
                 obj for obj in worker_pool.worker_list if obj.object_uid == uid
             )
             worker_pool.worker_list.remove(worker_linked_object)
```

### Comparing `syft-0.8.7b3/src/syft/service/worker/worker_stash.py` & `syft-0.8.7b4/src/syft/service/worker/worker_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/blob_storage/__init__.py` & `syft-0.8.7b4/src/syft/store/blob_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/blob_storage/on_disk.py` & `syft-0.8.7b4/src/syft/store/blob_storage/on_disk.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/blob_storage/seaweedfs.py` & `syft-0.8.7b4/src/syft/store/blob_storage/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/dict_document_store.py` & `syft-0.8.7b4/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/document_store.py` & `syft-0.8.7b4/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/kv_document_store.py` & `syft-0.8.7b4/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/linked_obj.py` & `syft-0.8.7b4/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/locks.py` & `syft-0.8.7b4/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/mongo_client.py` & `syft-0.8.7b4/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/mongo_codecs.py` & `syft-0.8.7b4/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/mongo_document_store.py` & `syft-0.8.7b4/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/store/sqlite_document_store.py` & `syft-0.8.7b4/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/blob_storage.py` & `syft-0.8.7b4/src/syft/types/blob_storage.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/datetime.py` & `syft-0.8.7b4/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/dicttuple.py` & `syft-0.8.7b4/src/syft/types/dicttuple.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/grid_url.py` & `syft-0.8.7b4/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/identity.py` & `syft-0.8.7b4/src/syft/types/identity.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/syft_metaclass.py` & `syft-0.8.7b4/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/syft_migration.py` & `syft-0.8.7b4/src/syft/types/syft_migration.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/syft_object.py` & `syft-0.8.7b4/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/syncable_object.py` & `syft-0.8.7b4/src/syft/types/syncable_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/transforms.py` & `syft-0.8.7b4/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/twin_object.py` & `syft-0.8.7b4/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/types/uid.py` & `syft-0.8.7b4/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/_std_stream_capture.py` & `syft-0.8.7b4/src/syft/util/_std_stream_capture.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/autoreload.py` & `syft-0.8.7b4/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/decorators.py` & `syft-0.8.7b4/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/experimental_flags.py` & `syft-0.8.7b4/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/filterwarnings.py` & `syft-0.8.7b4/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/fonts.py` & `syft-0.8.7b4/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/logger.py` & `syft-0.8.7b4/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/markdown.py` & `syft-0.8.7b4/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/notebook_ui/components/base.py` & `syft-0.8.7b4/src/syft/util/notebook_ui/components/base.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/notebook_ui/components/sync.py` & `syft-0.8.7b4/src/syft/util/notebook_ui/components/sync.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.7b4/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,24 +243,23 @@
         position: relative;
     }
 
     .grid-std-cells${uid} {
         grid-column: ${grid_template_cell_columns};
         display: flex;
         justify-content: center;
-        align-items: center; width: 100%; height: 100%;
+        align-items: center;
     }
 
     .grid-index-cells {
         grid-column: span 1;
         /* tmp fix to make left col stand out (fix with font-family) */
         font-weight: 600;
         background-color: var(--secondary-color) !important;
         color: var(--tertiary-color);
-        height: 100%;
     }
 
     .center-content-cell{
         margin: auto;
     }
 
     .grid-header {
```

### Comparing `syft-0.8.7b3/src/syft/util/schema.py` & `syft-0.8.7b4/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/telemetry.py` & `syft-0.8.7b4/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/trace_decorator.py` & `syft-0.8.7b4/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/util.py` & `syft-0.8.7b4/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft/util/version_compare.py` & `syft-0.8.7b4/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft.egg-info/PKG-INFO` & `syft-0.8.7b4/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b3
+Version: 0.8.7b4
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

### Comparing `syft-0.8.7b3/src/syft.egg-info/SOURCES.txt` & `syft-0.8.7b4/src/syft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b3/src/syft.egg-info/requires.txt` & `syft-0.8.7b4/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*


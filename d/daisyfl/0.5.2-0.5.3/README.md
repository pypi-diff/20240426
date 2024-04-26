# Comparing `tmp/daisyfl-0.5.2.tar.gz` & `tmp/daisyfl-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daisyfl-0.5.2.tar", max compression
+gzip compressed data, was "daisyfl-0.5.3.tar", max compression
```

## Comparing `daisyfl-0.5.2.tar` & `daisyfl-0.5.3.tar`

### file list

```diff
@@ -1,84 +1,94 @@
--rw-r--r--   0        0        0    11358 2023-06-29 08:05:35.674456 daisyfl-0.5.2/LICENSE
--rw-r--r--   0        0        0     1158 2023-06-29 08:05:35.676455 daisyfl-0.5.2/README.md
--rw-r--r--   0        0        0     3681 2023-09-26 09:03:04.835189 daisyfl-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1093 2023-06-29 08:05:35.860456 daisyfl-0.5.2/src/py/daisyfl/__init__.py
--rw-r--r--   0        0        0     1171 2023-06-29 08:05:35.866456 daisyfl-0.5.2/src/py/daisyfl/client/__init__.py
--rw-r--r--   0        0        0     9951 2023-08-17 04:39:34.231418 daisyfl-0.5.2/src/py/daisyfl/client/app.py
--rw-r--r--   0        0        0     3733 2023-06-29 08:05:35.872456 daisyfl-0.5.2/src/py/daisyfl/client/client.py
--rw-r--r--   0        0        0     1363 2023-06-29 08:05:35.874456 daisyfl-0.5.2/src/py/daisyfl/client/client_api_handler.py
--rw-r--r--   0        0        0     3780 2023-06-29 08:05:35.876456 daisyfl-0.5.2/src/py/daisyfl/client/client_operator_manager.py
--rw-r--r--   0        0        0     3367 2023-06-29 08:05:35.880456 daisyfl-0.5.2/src/py/daisyfl/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      714 2023-06-29 08:05:35.882456 daisyfl-0.5.2/src/py/daisyfl/client/grpc_client/__init__.py
--rw-r--r--   0        0        0    10410 2023-09-25 09:17:24.107816 daisyfl-0.5.2/src/py/daisyfl/client/grpc_client/connection.py
--rw-r--r--   0        0        0     6704 2023-06-29 08:05:35.889456 daisyfl-0.5.2/src/py/daisyfl/client/grpc_client/message_handler.py
--rw-r--r--   0        0        0     5084 2023-06-29 08:05:35.893456 daisyfl-0.5.2/src/py/daisyfl/client/numpy_client.py
--rw-r--r--   0        0        0     6741 2023-09-26 08:40:07.938896 daisyfl-0.5.2/src/py/daisyfl/client/trainer.py
--rw-r--r--   0        0        0     1663 2023-06-29 08:05:35.898456 daisyfl-0.5.2/src/py/daisyfl/client/zone_client.py
--rw-r--r--   0        0        0     6479 2023-09-23 09:03:38.187049 daisyfl-0.5.2/src/py/daisyfl/common/__init__.py
--rw-r--r--   0        0        0     1830 2023-06-29 08:05:35.904456 daisyfl-0.5.2/src/py/daisyfl/common/dp.py
--rw-r--r--   0        0        0     3482 2023-06-29 08:05:35.906456 daisyfl-0.5.2/src/py/daisyfl/common/logger.py
--rw-r--r--   0        0        0     1421 2023-06-29 08:05:35.908456 daisyfl-0.5.2/src/py/daisyfl/common/metadata.py
--rw-r--r--   0        0        0     3938 2023-06-29 08:05:35.909456 daisyfl-0.5.2/src/py/daisyfl/common/parameter.py
--rw-r--r--   0        0        0    17846 2023-09-25 08:31:06.627441 daisyfl-0.5.2/src/py/daisyfl/common/serde.py
--rw-r--r--   0        0        0     4173 2023-09-23 11:29:51.230991 daisyfl-0.5.2/src/py/daisyfl/common/typing.py
--rw-r--r--   0        0        0        0 2023-06-29 08:05:35.920456 daisyfl-0.5.2/src/py/daisyfl/operator/__init__.py
--rw-r--r--   0        0        0        0 2023-09-13 12:39:09.613077 daisyfl-0.5.2/src/py/daisyfl/operator/base/__init__.py
--rw-r--r--   0        0        0     1162 2023-09-13 12:39:09.616077 daisyfl-0.5.2/src/py/daisyfl/operator/base/client_logic.py
--rw-r--r--   0        0        0     5991 2023-09-26 08:40:21.633929 daisyfl-0.5.2/src/py/daisyfl/operator/base/server_logic.py
--rw-r--r--   0        0        0        0 2023-06-29 08:05:35.929456 daisyfl-0.5.2/src/py/daisyfl/operator/base_async/__init__.py
--rw-r--r--   0        0        0     1162 2023-06-29 08:05:35.931456 daisyfl-0.5.2/src/py/daisyfl/operator/base_async/client_logic.py
--rw-r--r--   0        0        0     5588 2023-09-26 04:13:09.849625 daisyfl-0.5.2/src/py/daisyfl/operator/base_async/server_logic.py
--rw-r--r--   0        0        0     1987 2023-06-29 08:05:35.935456 daisyfl-0.5.2/src/py/daisyfl/operator/msg_demo/client_logic.py
--rw-r--r--   0        0        0      381 2023-06-29 08:05:35.937456 daisyfl-0.5.2/src/py/daisyfl/operator/msg_demo/msg.py
--rw-r--r--   0        0        0     5581 2023-09-13 13:55:56.200088 daisyfl-0.5.2/src/py/daisyfl/operator/msg_demo/server_logic.py
--rw-r--r--   0        0        0      961 2023-06-29 08:05:35.940456 daisyfl-0.5.2/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
--rw-r--r--   0        0        0     6063 2023-09-13 13:59:05.075455 daisyfl-0.5.2/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
--rw-r--r--   0        0        0    12137 2023-06-29 08:05:35.944456 daisyfl-0.5.2/src/py/daisyfl/operator/sec_agg/client_logic.py
--rw-r--r--   0        0        0     1755 2023-06-29 08:05:35.946456 daisyfl-0.5.2/src/py/daisyfl/operator/sec_agg/common.py
--rw-r--r--   0        0        0    10070 2023-06-29 08:05:35.948456 daisyfl-0.5.2/src/py/daisyfl/operator/sec_agg/primitives.py
--rw-r--r--   0        0        0    22417 2023-09-13 14:20:58.112964 daisyfl-0.5.2/src/py/daisyfl/operator/sec_agg/server_logic.py
--rw-r--r--   0        0        0     1456 2023-06-29 08:05:35.953456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/__init__.py
--rw-r--r--   0        0        0     3016 2023-06-29 08:05:35.955456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/aggregate.py
--rw-r--r--   0        0        0     4538 2023-06-29 08:05:35.958456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     5155 2023-09-13 13:45:13.402829 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     6134 2023-06-29 08:05:35.962456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6993 2023-06-29 08:05:35.966456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7245 2023-06-29 08:05:35.970456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedadam.py
--rw-r--r--   0        0        0    13142 2023-09-13 13:42:47.692541 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedasync.py
--rw-r--r--   0        0        0    12484 2023-09-13 13:37:48.280949 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedavg.py
--rw-r--r--   0        0        0    11003 2023-09-13 13:43:08.543583 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedavg_android.py
--rw-r--r--   0        0        0     9115 2023-06-29 08:05:35.982456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedavgm.py
--rw-r--r--   0        0        0     5513 2023-06-29 08:05:35.986456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedopt.py
--rw-r--r--   0        0        0     7263 2023-06-29 08:05:35.987456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedyogi.py
--rw-r--r--   0        0        0    10980 2023-07-24 06:30:47.907550 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/qfedavg.py
--rw-r--r--   0        0        0     7867 2023-06-29 08:05:35.991456 daisyfl-0.5.2/src/py/daisyfl/operator/strategy/strategy.py
--rw-r--r--   0        0        0      826 2023-06-29 08:05:35.993456 daisyfl-0.5.2/src/py/daisyfl/operator/utils/__init__.py
--rw-r--r--   0        0        0     7395 2023-09-13 13:22:53.462175 daisyfl-0.5.2/src/py/daisyfl/operator/utils/op_tools.py
--rw-r--r--   0        0        0      676 2023-06-29 08:05:35.997456 daisyfl-0.5.2/src/py/daisyfl/proto/__init__.py
--rw-r--r--   0        0        0    75628 2023-09-25 08:37:05.130152 daisyfl-0.5.2/src/py/daisyfl/proto/transport_pb2.py
--rw-r--r--   0        0        0    27462 2023-09-25 08:37:05.131152 daisyfl-0.5.2/src/py/daisyfl/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2631 2023-09-25 08:37:05.133152 daisyfl-0.5.2/src/py/daisyfl/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      781 2023-09-25 08:37:05.134152 daisyfl-0.5.2/src/py/daisyfl/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0     1064 2023-06-29 08:05:36.010456 daisyfl-0.5.2/src/py/daisyfl/server/__init__.py
--rw-r--r--   0        0        0     5085 2023-09-12 10:01:05.667910 daisyfl-0.5.2/src/py/daisyfl/server/app.py
--rw-r--r--   0        0        0    10011 2023-09-13 08:58:19.604620 daisyfl-0.5.2/src/py/daisyfl/server/client_manager.py
--rw-r--r--   0        0        0     2745 2023-09-13 08:59:13.253707 daisyfl-0.5.2/src/py/daisyfl/server/client_proxy.py
--rw-r--r--   0        0        0     1053 2023-09-07 10:43:07.719590 daisyfl-0.5.2/src/py/daisyfl/server/criterion.py
--rw-r--r--   0        0        0      714 2023-06-29 08:05:36.025456 daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/__init__.py
--rw-r--r--   0        0        0    18614 2023-09-26 07:35:12.794946 daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     7183 2023-09-26 08:40:58.031016 daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4998 2023-09-26 08:28:42.194238 daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11290 2023-09-12 10:00:55.739885 daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     3626 2023-08-16 05:52:52.731108 daisyfl-0.5.2/src/py/daisyfl/server/history.py
--rw-r--r--   0        0        0    17280 2023-09-26 08:40:35.832963 daisyfl-0.5.2/src/py/daisyfl/server/server.py
--rw-r--r--   0        0        0     8452 2023-09-13 13:25:38.615503 daisyfl-0.5.2/src/py/daisyfl/server/server_api_handler.py
--rw-r--r--   0        0        0     4560 2023-06-29 08:05:36.049456 daisyfl-0.5.2/src/py/daisyfl/server/server_operator_manager.py
--rw-r--r--   0        0        0    15035 2023-09-26 08:40:43.520981 daisyfl-0.5.2/src/py/daisyfl/server/task_manager.py
--rw-r--r--   0        0        0     1273 2023-06-29 08:05:36.055456 daisyfl-0.5.2/src/py/daisyfl/simulation/__init__.py
--rw-r--r--   0        0        0     7335 2023-06-29 08:05:36.058456 daisyfl-0.5.2/src/py/daisyfl/simulation/app.py
--rw-r--r--   0        0        0      727 2023-06-29 08:05:36.060456 daisyfl-0.5.2/src/py/daisyfl/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     4661 2023-06-29 08:05:36.062456 daisyfl-0.5.2/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0      859 2023-06-29 08:05:36.064456 daisyfl-0.5.2/src/py/daisyfl/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-06-29 08:05:36.066456 daisyfl-0.5.2/src/py/daisyfl/utils/dynamic_loader.py
--rw-r--r--   0        0        0     2786 2023-09-26 09:04:12.997681 daisyfl-0.5.2/setup.py
--rw-r--r--   0        0        0     3321 2023-09-26 09:04:12.997915 daisyfl-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-29 08:05:35.674456 daisyfl-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1158 2023-06-29 08:05:35.676455 daisyfl-0.5.3/README.md
+-rw-r--r--   0        0        0     3661 2024-04-26 05:13:26.088018 daisyfl-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1111 2023-11-21 11:52:29.519203 daisyfl-0.5.3/src/py/daisyfl/__init__.py
+-rw-r--r--   0        0        0     1104 2023-11-20 08:34:06.412956 daisyfl-0.5.3/src/py/daisyfl/client/__init__.py
+-rw-r--r--   0        0        0     9364 2023-12-13 13:44:59.431555 daisyfl-0.5.3/src/py/daisyfl/client/app.py
+-rw-r--r--   0        0        0     3733 2023-06-29 08:05:35.872456 daisyfl-0.5.3/src/py/daisyfl/client/client.py
+-rw-r--r--   0        0        0     6076 2023-12-22 12:07:38.857965 daisyfl-0.5.3/src/py/daisyfl/client/client_operator_manager.py
+-rw-r--r--   0        0        0     3367 2023-06-29 08:05:35.880456 daisyfl-0.5.3/src/py/daisyfl/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      714 2023-06-29 08:05:35.882456 daisyfl-0.5.3/src/py/daisyfl/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8101 2023-12-31 06:11:58.509748 daisyfl-0.5.3/src/py/daisyfl/client/grpc_client/c2z_connection.py
+-rw-r--r--   0        0        0     7282 2023-12-13 12:50:56.104293 daisyfl-0.5.3/src/py/daisyfl/client/grpc_client/message_handler.py
+-rw-r--r--   0        0        0      714 2023-11-20 06:10:47.345624 daisyfl-0.5.3/src/py/daisyfl/client/grpc_server/__init__.py
+-rw-r--r--   0        0        0     6697 2023-12-22 10:39:27.248147 daisyfl-0.5.3/src/py/daisyfl/client/grpc_server/client_service_servicer.py
+-rw-r--r--   0        0        0    11539 2023-12-13 13:40:04.304894 daisyfl-0.5.3/src/py/daisyfl/client/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     5084 2023-06-29 08:05:35.893456 daisyfl-0.5.3/src/py/daisyfl/client/numpy_client.py
+-rw-r--r--   0        0        0     6741 2023-11-20 07:04:25.836645 daisyfl-0.5.3/src/py/daisyfl/client/trainer.py
+-rw-r--r--   0        0        0     7008 2023-12-13 10:51:06.003226 daisyfl-0.5.3/src/py/daisyfl/common/__init__.py
+-rw-r--r--   0        0        0     1830 2023-06-29 08:05:35.904456 daisyfl-0.5.3/src/py/daisyfl/common/dp.py
+-rw-r--r--   0        0        0     3482 2023-06-29 08:05:35.906456 daisyfl-0.5.3/src/py/daisyfl/common/logger.py
+-rw-r--r--   0        0        0     1421 2023-06-29 08:05:35.908456 daisyfl-0.5.3/src/py/daisyfl/common/metadata.py
+-rw-r--r--   0        0        0     3938 2023-06-29 08:05:35.909456 daisyfl-0.5.3/src/py/daisyfl/common/parameter.py
+-rw-r--r--   0        0        0    21639 2023-12-13 13:34:09.701100 daisyfl-0.5.3/src/py/daisyfl/common/serde.py
+-rw-r--r--   0        0        0     4406 2024-03-01 07:25:02.972703 daisyfl-0.5.3/src/py/daisyfl/common/typing.py
+-rw-r--r--   0        0        0      780 2023-11-21 11:32:38.898258 daisyfl-0.5.3/src/py/daisyfl/master/__init__.py
+-rw-r--r--   0        0        0     4254 2023-12-11 09:57:59.166782 daisyfl-0.5.3/src/py/daisyfl/master/app.py
+-rw-r--r--   0        0        0      714 2023-11-21 11:24:57.268752 daisyfl-0.5.3/src/py/daisyfl/master/grpc_server/__init__.py
+-rw-r--r--   0        0        0    11657 2023-12-07 13:56:13.483749 daisyfl-0.5.3/src/py/daisyfl/master/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0    17594 2023-12-11 09:58:06.437795 daisyfl-0.5.3/src/py/daisyfl/master/grpc_server/master_service_servicer.py
+-rw-r--r--   0        0        0     8167 2023-11-20 13:14:28.397410 daisyfl-0.5.3/src/py/daisyfl/master/server_api_handler.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:05:35.920456 daisyfl-0.5.3/src/py/daisyfl/operator/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-13 12:39:09.613077 daisyfl-0.5.3/src/py/daisyfl/operator/base/__init__.py
+-rw-r--r--   0        0        0     1868 2023-12-13 16:57:04.764940 daisyfl-0.5.3/src/py/daisyfl/operator/base/client_logic.py
+-rw-r--r--   0        0        0     5991 2023-09-26 08:40:21.633929 daisyfl-0.5.3/src/py/daisyfl/operator/base/server_logic.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:05:35.929456 daisyfl-0.5.3/src/py/daisyfl/operator/base_async/__init__.py
+-rw-r--r--   0        0        0     1872 2023-12-13 14:53:54.257853 daisyfl-0.5.3/src/py/daisyfl/operator/base_async/client_logic.py
+-rw-r--r--   0        0        0     5588 2023-09-26 04:13:09.849625 daisyfl-0.5.3/src/py/daisyfl/operator/base_async/server_logic.py
+-rw-r--r--   0        0        0     2020 2023-12-11 09:43:08.762129 daisyfl-0.5.3/src/py/daisyfl/operator/msg_demo/client_logic.py
+-rw-r--r--   0        0        0      381 2023-06-29 08:05:35.937456 daisyfl-0.5.3/src/py/daisyfl/operator/msg_demo/msg.py
+-rw-r--r--   0        0        0     5587 2023-11-22 07:08:45.848904 daisyfl-0.5.3/src/py/daisyfl/operator/msg_demo/server_logic.py
+-rw-r--r--   0        0        0     6068 2023-11-22 07:09:41.481096 daisyfl-0.5.3/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
+-rw-r--r--   0        0        0    12170 2023-12-11 09:42:56.065106 daisyfl-0.5.3/src/py/daisyfl/operator/sec_agg/client_logic.py
+-rw-r--r--   0        0        0     1755 2023-06-29 08:05:35.946456 daisyfl-0.5.3/src/py/daisyfl/operator/sec_agg/common.py
+-rw-r--r--   0        0        0    10070 2023-06-29 08:05:35.948456 daisyfl-0.5.3/src/py/daisyfl/operator/sec_agg/primitives.py
+-rw-r--r--   0        0        0    22421 2023-11-22 07:10:14.596211 daisyfl-0.5.3/src/py/daisyfl/operator/sec_agg/server_logic.py
+-rw-r--r--   0        0        0     1456 2023-06-29 08:05:35.953456 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/__init__.py
+-rw-r--r--   0        0        0     3016 2023-06-29 08:05:35.955456 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/aggregate.py
+-rw-r--r--   0        0        0     4536 2023-11-22 07:23:55.288060 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     5153 2023-11-20 13:15:31.362650 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     6133 2023-11-20 11:16:01.913437 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6992 2023-11-20 11:15:56.197413 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7244 2023-11-20 11:15:55.086408 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedadam.py
+-rw-r--r--   0        0        0    13140 2023-11-20 13:15:23.497620 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedasync.py
+-rw-r--r--   0        0        0    12482 2023-11-20 13:15:22.779617 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedavg.py
+-rw-r--r--   0        0        0    11001 2023-11-20 13:15:21.523613 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     9113 2023-11-20 13:15:20.606609 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedavgm.py
+-rw-r--r--   0        0        0     5513 2023-06-29 08:05:35.986456 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedopt.py
+-rw-r--r--   0        0        0     7262 2023-11-20 11:15:41.655352 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedyogi.py
+-rw-r--r--   0        0        0    10978 2023-11-20 13:15:19.037603 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7865 2023-11-20 13:15:15.606590 daisyfl-0.5.3/src/py/daisyfl/operator/strategy/strategy.py
+-rw-r--r--   0        0        0      826 2023-06-29 08:05:35.993456 daisyfl-0.5.3/src/py/daisyfl/operator/utils/__init__.py
+-rw-r--r--   0        0        0     7436 2024-01-03 05:43:56.053114 daisyfl-0.5.3/src/py/daisyfl/operator/utils/op_tools.py
+-rw-r--r--   0        0        0      676 2023-06-29 08:05:35.997456 daisyfl-0.5.3/src/py/daisyfl/proto/__init__.py
+-rw-r--r--   0        0        0    93672 2023-12-13 16:02:24.488350 daisyfl-0.5.3/src/py/daisyfl/proto/transport_pb2.py
+-rw-r--r--   0        0        0    34015 2023-12-13 16:02:24.490350 daisyfl-0.5.3/src/py/daisyfl/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2631 2023-12-13 16:02:24.492350 daisyfl-0.5.3/src/py/daisyfl/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      781 2023-12-13 16:02:24.493350 daisyfl-0.5.3/src/py/daisyfl/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1273 2023-06-29 08:05:36.055456 daisyfl-0.5.3/src/py/daisyfl/simulation/__init__.py
+-rw-r--r--   0        0        0     7339 2023-11-22 07:45:45.788581 daisyfl-0.5.3/src/py/daisyfl/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-06-29 08:05:36.060456 daisyfl-0.5.3/src/py/daisyfl/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     4660 2023-11-20 11:15:22.290271 daisyfl-0.5.3/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0      859 2023-06-29 08:05:36.064456 daisyfl-0.5.3/src/py/daisyfl/utils/__init__.py
+-rw-r--r--   0        0        0    10125 2024-01-03 11:58:12.584626 daisyfl-0.5.3/src/py/daisyfl/utils/client_manager.py
+-rw-r--r--   0        0        0     2802 2023-12-08 07:31:46.598605 daisyfl-0.5.3/src/py/daisyfl/utils/client_proxy.py
+-rw-r--r--   0        0        0     3051 2023-11-20 07:36:37.994775 daisyfl-0.5.3/src/py/daisyfl/utils/connection.py
+-rw-r--r--   0        0        0     1053 2023-11-20 11:15:18.498255 daisyfl-0.5.3/src/py/daisyfl/utils/criterion.py
+-rw-r--r--   0        0        0      121 2023-06-29 08:05:36.066456 daisyfl-0.5.3/src/py/daisyfl/utils/dynamic_loader.py
+-rw-r--r--   0        0        0     7183 2023-09-26 08:40:58.031016 daisyfl-0.5.3/src/py/daisyfl/utils/grpc_bridge.py
+-rw-r--r--   0        0        0     5247 2023-12-07 12:43:45.841111 daisyfl-0.5.3/src/py/daisyfl/utils/grpc_client_proxy.py
+-rw-r--r--   0        0        0     3626 2023-08-16 05:52:52.731108 daisyfl-0.5.3/src/py/daisyfl/utils/history.py
+-rw-r--r--   0        0        0     2148 2023-12-22 10:37:17.699036 daisyfl-0.5.3/src/py/daisyfl/utils/model_sync.py
+-rw-r--r--   0        0        0    20405 2023-12-08 12:49:21.725067 daisyfl-0.5.3/src/py/daisyfl/utils/server.py
+-rw-r--r--   0        0        0     4560 2023-11-20 13:17:04.765005 daisyfl-0.5.3/src/py/daisyfl/utils/server_operator_manager.py
+-rw-r--r--   0        0        0    14834 2024-03-19 07:31:42.931909 daisyfl-0.5.3/src/py/daisyfl/utils/task_manager.py
+-rw-r--r--   0        0        0      774 2023-11-21 11:32:59.344325 daisyfl-0.5.3/src/py/daisyfl/zone/__init__.py
+-rw-r--r--   0        0        0     4527 2023-12-07 14:08:36.500273 daisyfl-0.5.3/src/py/daisyfl/zone/app.py
+-rw-r--r--   0        0        0     3761 2023-11-21 13:12:09.140468 daisyfl-0.5.3/src/py/daisyfl/zone/grpc_client/message_handler.py
+-rw-r--r--   0        0        0     7953 2023-11-21 12:49:25.201050 daisyfl-0.5.3/src/py/daisyfl/zone/grpc_client/z2m_connection.py
+-rw-r--r--   0        0        0      714 2023-11-21 11:29:32.740649 daisyfl-0.5.3/src/py/daisyfl/zone/grpc_server/__init__.py
+-rw-r--r--   0        0        0    11647 2023-12-07 13:55:24.714649 daisyfl-0.5.3/src/py/daisyfl/zone/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0    17594 2023-12-08 07:19:54.288089 daisyfl-0.5.3/src/py/daisyfl/zone/grpc_server/zone_service_servicer.py
+-rw-r--r--   0        0        0     6925 2023-11-21 12:51:54.143532 daisyfl-0.5.3/src/py/daisyfl/zone/zone_entry.py
+-rw-r--r--   0        0        0     2871 2024-04-26 05:28:45.819656 daisyfl-0.5.3/setup.py
+-rw-r--r--   0        0        0     3286 2024-04-26 05:28:45.819902 daisyfl-0.5.3/PKG-INFO
```

### Comparing `daisyfl-0.5.2/LICENSE` & `daisyfl-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/README.md` & `daisyfl-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/pyproject.toml` & `daisyfl-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "daisyfl"
-version = "0.5.2"
+version = "0.5.3"
 description = "Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing"
 license = "Apache-2.0"
 authors = ["tcfwbper <b05208031@ntu.edu.tw>"]
 readme = "README.md"
 homepage = "https://github.com/Intelligent-Systems-Lab/daisy"
 repository = "https://github.com/Intelligent-Systems-Lab/daisy"
 documentation = "https://github.com/Intelligent-Systems-Lab/daisy/tree/main/doc/daisy"
@@ -47,15 +47,14 @@
 python = "^3.8"
 # Mandatory dependencies
 numpy = "^1.21.0"
 grpcio = "^1.43.0"
 protobuf = "^3.19.0"
 importlib-metadata = { version = "^4.0.0", markers = "python_version < '3.8'" }
 iterators = "^0.0.2"
-urllib3 = "1.26.15"
 dataclasses-json = "^0.5.7"
 # Optional dependencies
 ray = { extras = ["default"], version = "~2.0.0", optional = true }
 Flask = "^2.2.2"
 pycryptodome = "^3.16.0"
 cryptography = "^38.0.4"
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower main package."""
 
 import sys
 
-from . import client, server, simulation
+from . import client, zone, master, simulation
 
 __all__ = [
     "client",
-    "server",
+    "zone",
+    "master",
     "simulation",
 ]
 
 # pylint: disable=import-error, no-name-in-module
 if sys.version_info < (3, 8):
     import importlib_metadata
 else:
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/client/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/client/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,18 +17,16 @@
 
 from .app import ClientLike as ClientLike
 from .app import start_client as start_client
 from .app import start_numpy_client as start_numpy_client
 from .app import to_client as to_client
 from .client import Client as Client
 from .numpy_client import NumPyClient as NumPyClient
-from .zone_client import ZoneClient as ZoneClient
 
 __all__ = [
     "Client",
     "ClientLike",
     "NumPyClient",
-    "ZoneClient"
     "start_client",
     "start_numpy_client",
     "to_client",
 ]
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/client/app.py` & `daisyfl-0.5.3/src/py/daisyfl/client/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     GRPC_MAX_MESSAGE_LENGTH,
     CURRENT_ROUND,
     FIT_SAMPLES,
     EVALUATE_SAMPLES,
     LOSS,
     METRICS,
     CLIENT_OPERATOR,
-    ZONE_CLIENT_OPERATOR,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
     IS_ZONE,
     CREDENTIAL,
     metadata_to_dict,
     dict_to_metadata,
     CID,
@@ -51,17 +50,17 @@
     GetPropertiesRes,
     NDArrays,
     Status,
     Report,
 )
 
 from .client import Client
-from .client_api_handler import ClientListener
 from .trainer import Trainer
-from .grpc_client.connection import gRPCConnection
+from .grpc_client.c2z_connection import C2ZConnection
+from .grpc_server.grpc_server import start_grpc_server
 from .grpc_client.message_handler import set_client_operator_manager
 from daisyfl.client.client_operator_manager import ClientOperatorManager
 from .numpy_client import NumPyClient
 from .numpy_client import has_evaluate as numpyclient_has_evaluate
 from .numpy_client import has_fit as numpyclient_has_fit
 from .numpy_client import has_get_parameters as numpyclient_has_get_parameters
 from .numpy_client import has_get_properties as numpyclient_has_get_properties
@@ -94,110 +93,92 @@
 
 
 ClientLike = Union[Client, NumPyClient]
 
 
 def start_client(
     *,
+    server_address: str,
     parent_address: str,
     client: Client,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[bytes] = None,
-    api_ip: str = None,
-    api_port: int = None,
     metadata: Tuple = None,
-    _zone: bool = False,
 ) -> None:
     # client_operator_manager
-    client_operator_manager = ClientOperatorManager(client=client)
-    operator_key = ZONE_CLIENT_OPERATOR if _zone else CLIENT_OPERATOR
-    client_operator_manager.set_operator_key(key=operator_key)
+    client_operator_manager = ClientOperatorManager(client=client, server_address=server_address,)
     set_client_operator_manager(client_operator_manager)
 
     # check metadata
     if metadata is None:
         metadata = ()
-    ## zone: process metadata
-    if _zone:
-        metadata_dict = metadata_to_dict(metadata=metadata, _check_required=False)
-        metadata_dict[IS_ZONE] = "is_zone"
-        if metadata_dict.__contains__(CREDENTIAL):
-            log(WARNING, "CREDENTIAL is defined in the metadata of a zone. It will be ignored.")
-            del metadata_dict[CREDENTIAL]
-        if not metadata_dict.__contains__(CID):
-            metadata_dict[CID] = str(uuid.uuid4())
+        log(WARNING, "Metadata is not defined. Use uuid as CID and \"default_credential\" as CREDENTIAL")
+        metadata_dict[CREDENTIAL] = "default_credential"
+        metadata_dict[CID] = str(uuid.uuid4())
         metadata = dict_to_metadata(metadata_dict)
-    ## client: check metadata
     else:
         metadata_dict = metadata_to_dict(metadata=metadata)
         metadata = dict_to_metadata(metadata_dict)
 
-    # declare instances: Trainer, gRPCConnection, ClientListener
+    # declare instances:
     trainer = Trainer()
-    connector = gRPCConnection(
+    connector = C2ZConnection(
         parent_address=parent_address,
         max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
         metadata=metadata,
         trainer=trainer,
     )
-    listener = ClientListener(
-        ip=api_ip,
-        port=api_port,
-        connector=connector,
-        trainer=trainer,
-    )
+    client_operator_manager.set_connector(connector)
     trainer.set_connector(connector=connector)
 
-    # start threads: ClientListener, gRPCConnection, Trainer
-    
-    ## ClientListener
-    listener_thread = threading.Thread(target=listener.run, args=())
-    listener_thread.setDaemon(True)
-    listener_thread.start()
-    ## gRPCConnection
+    # start threads: gRPCServer, C2ZConnection, Trainer
+    ## gRPCServer
+    grpc_server = start_grpc_server(
+        server_address=server_address,
+        model_sync_fn=client_operator_manager.model_sync_fn,
+        shutdown_fn=trainer.shutdown,
+        reservation_fn=client_operator_manager.reservation_fn,
+    )
+    log(INFO, "gRPCServer for C2C is running.")
+
+    ## C2ZConnection
     connector_thread = threading.Thread(target=connector.run, args=())
     connector_thread.setDaemon(True)
     connector_thread.start()
     ### check
     threading.Event().wait(timeout=1)
-    if not listener_thread.is_alive():
-        log(ERROR, "ClientListener failed")
-        exit(1)
     if not connector_thread.is_alive():
-        log(ERROR, "gRPCConnection failed")
+        log(ERROR, "C2ZConnection failed")
         exit(1)
     ## Trainer
     trainer.run()
 
+    # shutdown
+    client_operator_manager.shutdown()
+
 
 def start_numpy_client(
     *,
+    server_address: str,
     parent_address: str,
     client: NumPyClient,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[bytes] = None,
-    api_ip: str = None,
-    api_port: int = None,
     metadata: Tuple = None,
-    _zone: bool = False
 ) -> None:
     # Start
     start_client(
+        server_address=server_address,
         parent_address=parent_address,
         client=_wrap_numpy_client(client=client),
         grpc_max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
-        api_ip=api_ip,
-        api_port=api_port,
         metadata=metadata,
-        _zone=_zone,
     )
-    if _zone:
-        client.shutdown()
 
 
 # wrap numpy_client to client
 def to_client(client_like: ClientLike) -> Client:
     """Take any Client-like object and return it as a Client."""
     if isinstance(client_like, NumPyClient):
         return _wrap_numpy_client(client=client_like)
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/client/client.py` & `daisyfl-0.5.3/src/py/daisyfl/client/client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/client/dpfedavg_numpy_client.py` & `daisyfl-0.5.3/src/py/daisyfl/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/client/grpc_client/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/client/grpc_client/connection.py` & `daisyfl-0.5.3/src/py/daisyfl/client/grpc_client/c2z_connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 from contextlib import contextmanager
 from logging import DEBUG, INFO, WARNING, ERROR
 from queue import Queue
 from typing import Callable, Iterator, Optional, Tuple, Any, Dict, List
 from daisyfl.common import FitRes, Status, Parameters, Code
+from daisyfl.utils.connection import grpc_connection
 
 import grpc
 from threading import Condition, Event, Lock
 
 from daisyfl.common import (
     HANDOVER,
     ROOT_CERTIFICATES,
@@ -68,30 +69,25 @@
     if handover:
         metadata_dict[HANDOVER] = "handover"
     elif metadata_dict.__contains__(HANDOVER):
         del metadata_dict[HANDOVER]
     
     return dict_to_metadata(metadata_dict)
 
-def on_channel_state_change(channel_connectivity: str) -> None:
-    """Log channel connectivity."""
-    log(DEBUG, channel_connectivity)
 
-class gRPCConnection:
+class C2ZConnection:
     def __init__(self,
         # for grpc_connection
         parent_address: str = None,
         max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
         root_certificates: Optional[bytes] = None,
         metadata: Tuple = (),
         # sync up
         trainer = None,
     ):
-        # channel
-        self._on_channel_state_change: Callable = on_channel_state_change
         # transmission
         self.send: Callable = None
         self.receive: Callable = None
         # for grpc_connection
         self._parent_address: str = parent_address
         self._max_message_length: int = max_message_length
         self._root_certificates: Optional[bytes] = root_certificates
@@ -116,15 +112,16 @@
     def run(self,):
         while True:
             # Wait for Trainer ready and for reconnection
             log(DEBUG, "Connector idling")
             self.event_reconn.wait()
             log(DEBUG, "Connector reconnecting")
             try:
-                with self.grpc_connection() as conn:
+                self._metadata = process_metadata(metadata=self._metadata, anchor=self._anchor, root_certificates=self._root_certificates, handover=self.check_handover())
+                with grpc_connection(self._parent_address, self._metadata, self._root_certificates) as conn:
                     send, receive = conn
                     self.receive = receive
                     self.send = send
                     # send ClientStatus
                     status_code = self._trainer.get_trainer_status_code()
                     if status_code == 1:
                         client_status = serde.client_status_to_proto(ClientStatus(status=CLIENT_IDLING))
@@ -142,66 +139,14 @@
                     # Wait for ConnectionFail
                     self.event_disconn.wait()
                     log(DEBUG, "Connector's term")
                     Event().wait(timeout=self.sleep_duration)
             except:
                 log(INFO, "Sleep for " + str(self.sleep_duration) + " seconds")
                 Event().wait(timeout=self.sleep_duration)
-    
-    @contextmanager
-    def grpc_connection(
-        self,
-    ) -> Iterator[Tuple[Callable[[], ServerMessage], Callable[[ClientMessage], None]]]:
-        # Possible options:
-        # https://github.com/grpc/grpc/blob/v1.43.x/include/grpc/impl/codegen/grpc_types.h
-        channel_options = [
-            ("grpc.max_send_message_length", self._max_message_length),
-            ("grpc.max_receive_message_length", self._max_message_length),
-        ]
-
-        if self._root_certificates is not None:
-            ssl_channel_credentials = grpc.ssl_channel_credentials(self._root_certificates)
-            channel = grpc.secure_channel(
-                self._parent_address, ssl_channel_credentials, options=channel_options
-            )
-            log(INFO, "Opened secure gRPC connection using certificates")
-        else:
-            channel = grpc.insecure_channel(self._parent_address, options=channel_options)
-            log(INFO, "Opened insecure gRPC connection (no certificates were passed)")
-
-        channel.subscribe(on_channel_state_change)
-
-        
-        stub = FlowerServiceStub(channel)
-        q: Queue[ClientMessage] = Queue(maxsize=1)
-        time_iterator = TimeoutIterator(iterator=iter(q.get, None), reset_on_next=True)
-        
-        self._metadata = process_metadata(metadata=self._metadata, anchor=self._anchor, root_certificates=self._root_certificates, handover=self.check_handover())
-        server_message_iterator: Iterator[ServerMessage] = stub.Join(time_iterator, metadata=self._metadata)
-        timeout_iterator = TimeoutIterator(iterator=server_message_iterator, reset_on_next=True)
-
-        def receive_fn(timeout: Optional[int] = None) -> Tuple[ServerMessage, bool]:        
-            if timeout is not None:
-                timeout_iterator.set_timeout(float(timeout))
-            server_message = next(timeout_iterator)
-            if server_message is timeout_iterator.get_sentinel():
-                return server_message, False
-            return server_message, True
-        receive: Callable[[Optional[int]], Tuple[ServerMessage, bool]] = receive_fn
-        send: Callable[[ClientMessage], None] = lambda msg: q.put(msg, block=False)
-
-        try:
-            yield send, receive
-        finally:
-            # Release Iterator to avoid leaking memory
-            time_iterator.interrupt()
-            send(self.sentinel)
-            # Make sure to have a final
-            channel.close()
-            log(DEBUG, "gRPC channel closed")
 
     def set_anchor(self, reset: bool = True) -> None:
         if reset:
             self._anchor = None
         else:    
             self._anchor = self._parent_address
 
@@ -271,7 +216,13 @@
         ###
         if new_parent_address is not None:
             self._parent_address = new_parent_address
         ###
         self._busy = False
         with self._cnd_api:
             self._cnd_api.notify_all()
+
+    def get_metadata(self,) -> Tuple:
+        return self._metadata
+    
+def get_connector() -> C2ZConnection:
+    _connector = None
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/client/grpc_client/message_handler.py` & `daisyfl-0.5.3/src/py/daisyfl/client/grpc_client/message_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Handle server messages by calling appropriate client methods."""
 
 
-from typing import Tuple
+from typing import Tuple, Union
 
 from daisyfl.client.client import (
     Client,
     has_evaluate,
     has_fit,
     has_get_parameters,
     has_get_properties,
 )
 from daisyfl.client.client_operator_manager import ClientOperatorManager
-from daisyfl.common import serde, typing
+from daisyfl.common import serde, typing, FitRes, ChainTransferSignal
 from daisyfl.common.typing import Parameters
 from daisyfl.proto.transport_pb2 import ClientMessage, Reason, ServerMessage
 
 # pylint: disable=missing-function-docstring
 
 
 class UnknownServerMessage(Exception):
@@ -64,14 +64,16 @@
         return _reconnect(server_msg.reconnect_ins)
     if field == "get_properties_ins":
         return _get_properties(server_msg.get_properties_ins)
     if field == "get_parameters_ins":
         return _get_parameters(server_msg.get_parameters_ins)
     if field == "fit_ins":
         return _fit(server_msg.fit_ins)
+    if field == "chain_proceeding_signal":
+        return _fit(server_msg.chain_proceeding_signal)
     if field == "evaluate_ins":
         return _evaluate(server_msg.evaluate_ins)
     raise UnknownServerMessage()
 
 
 def _reconnect(
     reconnect_msg: ServerMessage.ReconnectIns,
@@ -142,24 +144,33 @@
     # Request parameters
     get_parameters_res = client.get_parameters(get_parameters_ins)
     # Serialize response
     get_parameters_res_proto = serde.get_parameters_res_to_proto(get_parameters_res)
     return ClientMessage(get_parameters_res=get_parameters_res_proto)
 
 
-def _fit(fit_msg: ServerMessage.FitIns) -> ClientMessage:
+def _fit(fit_msg: Union[ServerMessage.FitIns, ServerMessage.ChainProceedingSignal]) -> ClientMessage:
     client_operator_manager = get_client_operator_manager()
 
     # Deserialize fit instruction
-    fit_ins = serde.fit_ins_from_proto(fit_msg)
+    if isinstance(fit_msg, ServerMessage.FitIns):
+        ins = serde.fit_ins_from_proto(fit_msg)
+    elif isinstance(fit_msg, ServerMessage.ChainProceedingSignal):
+        ins = serde.chain_proceeding_signal_from_proto(fit_msg)
     # Perform fit
-    fit_res = client_operator_manager.fit(fit_ins)
+    res = client_operator_manager.fit(ins)
     # Serialize fit result
-    fit_res_proto = serde.fit_res_to_proto(fit_res)
-    return ClientMessage(fit_res=fit_res_proto)
+    if isinstance(res, FitRes):
+        fit_res_proto = serde.fit_res_to_proto(res)
+        cm = ClientMessage(fit_res=fit_res_proto)
+    elif isinstance(res, ChainTransferSignal):
+        cts_proto = serde.chain_transfer_signal_to_proto(cts=res)
+        cm = ClientMessage(chain_transfer_signal=cts_proto)
+    
+    return cm
 
 
 def _evaluate(evaluate_msg: ServerMessage.EvaluateIns) -> ClientMessage:
     client_operator_manager = get_client_operator_manager()
     
     # Deserialize evaluate instruction
     evaluate_ins = serde.evaluate_ins_from_proto(evaluate_msg)
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/client/numpy_client.py` & `daisyfl-0.5.3/src/py/daisyfl/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/client/trainer.py` & `daisyfl-0.5.3/src/py/daisyfl/client/trainer.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/common/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/common/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .typing import FitIns as FitIns
 from .typing import FitRes as FitRes
 from .typing import ClientStatus as ClientStatus
 from .typing import ServerReceivedSignal as ServerReceivedSignal
 from .typing import ClientUploadingSignal as ClientUploadingSignal
 from .typing import ServerStatus as ServerStatus
 from .typing import ClientRoamingSignal as ClientRoamingSignal
+from .typing import Shutdown as Shutdown
 from .typing import GetParametersIns as GetParametersIns
 from .typing import GetParametersRes as GetParametersRes
 from .typing import GetPropertiesIns as GetPropertiesIns
 from .typing import GetPropertiesRes as GetPropertiesRes
 from .typing import Metrics as Metrics
 from .typing import MetricsAggregationFn as MetricsAggregationFn
 from .typing import NDArray as NDArray
@@ -57,14 +58,20 @@
 from .typing import Element as Element
 from .typing import Status as Status
 from .typing import Task as Task
 from .typing import Report as Report
 from .typing import Type as Type
 from .typing import CheckResults as CheckResults
 from .typing import CurrentReturns as CurrentReturns
+from .typing import ModelSyncMessage as ModelSyncMessage
+from .typing import ChainTransferSignal as ChainTransferSignal
+from .typing import ChainProceedingSignal as ChainProceedingSignal
+from .typing import ModelTransferReservation as ModelTransferReservation
+from .typing import ReservationSuccess as ReservationSuccess
+from .typing import ReservationFailure as ReservationFailure
 
 
 GRPC_MAX_MESSAGE_LENGTH: int = 536_870_912  # == 512 * 1024 * 1024
 NUM_ROUNDS = "NUM_ROUNDS"
 CURRENT_ROUND = "CURRENT_ROUND"
 CURRENT_ROUND_MASTER = "CURRENT_ROUND_MASTER"
 CURRENT_ROUND_ZONE = "CURRENT_ROUND_ZONE"
@@ -81,15 +88,14 @@
 EVALUATE_INIT_MODEL_MASTER = "EVALUATE_INIT_MODEL_MASTER"
 MODEL_PATH = "MODEL_PATH"
 REMOVE_OPERATOR = "REMOVE_OPERATOR"
 OPERATORS = "OPERATORS"
 MASTER_SERVER_OPERATOR = "MASTER_SERVER_OPERATOR"
 CLIENT_OPERATOR = "CLIENT_OPERATOR"
 ZONE_SERVER_OPERATOR = "ZONE_SERVER_OPERATOR"
-ZONE_CLIENT_OPERATOR = "ZONE_CLIENT_OPERATOR"
 STRATEGIES = "STRATEGIES"
 MASTER_STRATEGY = "MASTER_STRATEGY"
 ZONE_STRATEGY = "ZONE_STRATEGY"
 ZONE_COMM_FREQUENCY = "ZONE_COMM_FREQUENCY"
 PERIOD = "PERIOD"
 PERIOD_MASTER = "PERIOD_MASTER"
 PERIOD_ZONE = "PERIOD_ZONE"
@@ -107,14 +113,20 @@
 PARTICIPATION = "PARTICIPATION"
 SAVE_MODEL = "SAVE_MODEL"
 ROAMING_TIMEOUT = "ROAMING_TIMEOUT"
 IS_ROAMER = "IS_ROAMER"
 
 
 __all__ = [
+    "ReservationFailure",
+    "ReservationSuccess",
+    "ModelTransferReservation",
+    "ChainProceedingSignal",
+    "ChainTransferSignal",
+    "ModelSyncMessage",
     "SUBTASK_RETURNS_SELECTED",
     "SUBTASK_RETURNS_RESULTS",
     "SUBTASK_RETURNS_FAILURES",
     "SUBTASK_RETURNS_ROAMING",
     "IS_ROAMER",
     "PARTICIPATION",
     "SUBTASK_TIMER",
@@ -155,14 +167,15 @@
     "GetPropertiesIns",
     "GetPropertiesRes",
     "ClientStatus",
     "ServerReceivedSignal",
     "ClientUploadingSignal",
     "ServerStatus",
     "ClientRoamingSignal",
+    "Shutdown",
     "GRPC_MAX_MESSAGE_LENGTH",
     "Metrics",
     "MetricsAggregationFn",
     "ndarray_to_bytes",
     "NDArray",
     "NDArrays",
     "ndarrays_to_parameters",
@@ -176,15 +189,14 @@
     "Report",
     "TID",
     "REMOVE_OPERATOR",
     "OPERATORS",
     "MASTER_SERVER_OPERATOR",
     "CLIENT_OPERATOR",
     "ZONE_SERVER_OPERATOR",
-    "ZONE_CLIENT_OPERATOR",
     "STRATEGIES",
     "MASTER_STRATEGY",
     "ZONE_STRATEGY",
     "PERIOD",
     "PERIOD_MASTER",
     "PERIOD_ZONE",
     "ZONE_COMM_FREQUENCY",
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/common/dp.py` & `daisyfl-0.5.3/src/py/daisyfl/common/dp.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/common/logger.py` & `daisyfl-0.5.3/src/py/daisyfl/common/logger.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/common/metadata.py` & `daisyfl-0.5.3/src/py/daisyfl/common/metadata.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/common/parameter.py` & `daisyfl-0.5.3/src/py/daisyfl/common/parameter.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/common/serde.py` & `daisyfl-0.5.3/src/py/daisyfl/common/serde.py`

 * *Files 11% similar despite different names*

```diff
@@ -278,14 +278,49 @@
     config = None if msg.config is None else inner_map_from_proto(msg.config)
     return typing.EvaluateRes(
         status=status,
         config=config,
     )
 
 
+# === ModelTransferReservation ===
+
+
+def model_transfer_reservation_to_proto(mtr: typing.ModelTransferReservation) -> ClientMessage.ModelTransferReservation:
+    """Serialize ModelTransferReservation to ProtoBuf message."""
+    config_msg = inner_map_to_proto(mtr.config)
+    return ClientMessage.ModelTransferReservation(config=config_msg)
+
+
+def model_transfer_reservation_from_proto(msg: ClientMessage.ModelTransferReservation) -> typing.ModelTransferReservation:
+    """Deserialize ProtoBuf message to ModelTransferReservation."""
+    config = inner_map_from_proto(msg.config)
+    return typing.ModelTransferReservation(config=config)
+
+
+def reservation_success_to_proto(rs: typing.ReservationSuccess) -> ServerMessage.ReservationSuccess:
+    """Serialize ReservationSuccess to ProtoBuf message."""
+    return ServerMessage.ReservationSuccess(status=rs.status)
+
+
+def reservation_success_from_proto(msg: ServerMessage.ReservationSuccess) -> typing.ReservationSuccess:
+    """Deserialize ProtoBuf message to ReservationSuccess."""
+    return typing.ReservationSuccess(status=msg.status)
+
+
+def reservation_failure_to_proto(rf: typing.ReservationFailure) -> ServerMessage.ReservationFailure:
+    """Serialize ReservationFailure to ProtoBuf message."""
+    return ServerMessage.ReservationFailure(status=rf.status)
+
+
+def reservation_failure_from_proto(msg: ServerMessage.ReservationFailure) -> typing.ReservationFailure:
+    """Deserialize ProtoBuf message to ReservationFailure."""
+    return typing.ReservationFailure(status=msg.status)
+
+
 #  === ClientStatus ===
 
 
 def client_status_to_proto(cs: typing.ClientStatus) -> ClientMessage.ClientStatus:
     """Serialize ClientStatus to ProtoBuf message."""
     return ClientMessage.ClientStatus(status=cs.status)
 
@@ -343,14 +378,70 @@
 
 def client_roaming_signal_from_proto(msg: ClientMessage.ClientRoamingSignal) -> typing.ClientRoamingSignal:
     """Deserialize ProtoBuf message to CRS"""
     status = status_from_proto(msg.status)
     return typing.ClientRoamingSignal(status=status)
 
 
+# === Model Sync messages ===
+
+
+def model_sync_request_to_proto(request: typing.ModelSyncMessage) -> ClientMessage.ModelSyncRequest:
+    """Serialize ModelSyncRequest to ProtoBuf message."""
+    parameters_proto = parameters_to_proto(request.parameters)
+    config_msg = inner_map_to_proto(request.config)
+    return ClientMessage.ModelSyncRequest(parameters=parameters_proto, config=config_msg)
+
+
+def model_sync_request_from_proto(msg: ClientMessage.ModelSyncRequest) -> typing.ModelSyncMessage:
+    """Deserialize ModelSyncRequest from ProtoBuf message."""
+    parameters = parameters_from_proto(msg.parameters)
+    config = inner_map_from_proto(msg.config)
+    return typing.ModelSyncMessage(parameters=parameters, config=config)
+
+
+# === Shutdown ===
+
+
+def shutdown_to_proto(shutdown_signal: typing.Shutdown) -> ClientMessage.Shutdown:
+    """Serialize Shutdown to ProtoBuf message."""
+    status_proto = status_to_proto(shutdown_signal.status)
+    return ClientMessage.Shutdown(status=status_proto)
+
+
+# === ChainTransferSignal ===
+
+
+def chain_transfer_signal_to_proto(cts: typing.ChainTransferSignal) -> ClientMessage.ChainTransferSignal:
+    """Serialize ChainTransferSignal to ProtoBuf message."""
+    config_msg = inner_map_to_proto(cts.config)
+    return ClientMessage.ChainTransferSignal(transfer_to=cts.transfer_to, config=config_msg)
+
+
+def chain_transfer_signal_from_proto(msg: ClientMessage.ChainTransferSignal) -> typing.ChainTransferSignal:
+    """Deserialize ProtoBuf message to ChainTransferSignal."""
+    config = inner_map_from_proto(msg.config)
+    return typing.ChainTransferSignal(transfer_to=msg.transfer_to, config=config)
+
+
+# === ChainProceedingSignal ===
+
+
+def chain_proceeding_signal_to_proto(cps: typing.ChainProceedingSignal) -> ServerMessage.ChainProceedingSignal:
+    """Serialize ChainProceedingSignal to ProtoBuf message."""
+    config_msg = inner_map_to_proto(cps.config)
+    return ServerMessage.ChainProceedingSignal(config=config_msg)
+
+
+def chain_proceeding_signal_from_proto(msg: ServerMessage.ChainProceedingSignal) -> typing.ChainProceedingSignal:
+    """Deserialize ProtoBuf message to ChainProceedingSignal."""
+    config = inner_map_from_proto(msg.config)
+    return typing.ChainProceedingSignal(config=config)
+
+
 # === Properties messages ===
 
 
 def properties_to_proto(properties: typing.Properties) -> Any:
     """Serialize... ."""
     proto = {}
     for key in properties:
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/common/typing.py` & `daisyfl-0.5.3/src/py/daisyfl/common/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,30 +142,20 @@
 
     reason: str
 
 @dataclass
 class Task:
     """Input a task when calling server API."""
     config: TypedDict
-    # TID: str
-    # NUM_ROUNDS: int
-    # CURRENT_ROUND: int
-    # EVALUATE: bool
-    # TIMEOUT: int
 
 
 @dataclass
 class Report:
     """After complete a task, return a report."""
     config: TypedDict
-    # CURRENT_ROUND: int
-    # FIT_SAMPLES: int
-    # EVALUATE_SAMPLES: int
-    # LOSS: float
-    # METRICS: Metrics
 
 class Type(Enum):
     """Type of the task manager."""
     
     MASTER = 1
     ZONE = 2
 
@@ -204,7 +194,38 @@
 class ClientUploadingSignal:
     status: Status
 
 
 @dataclass
 class ClientRoamingSignal:
     status: Status
+
+
+@dataclass
+class ModelSyncMessage:
+    parameters: Parameters
+    config: TypedDict
+
+@dataclass
+class Shutdown:
+    status: Status
+
+@dataclass
+class ChainTransferSignal:
+    transfer_to: str
+    config: TypedDict
+
+@dataclass
+class ChainProceedingSignal:
+    config: TypedDict
+
+@dataclass
+class ModelTransferReservation:
+    config: TypedDict
+
+@dataclass
+class ReservationSuccess:
+    status: str
+
+@dataclass
+class ReservationFailure:
+    status: str
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/base/server_logic.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/base/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/base_async/server_logic.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/base_async/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/msg_demo/client_logic.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/msg_demo/client_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from daisyfl.operator.base.client_logic import ClientLogic as BaseClientLogic
 from daisyfl.client import Client
 
 class ClientLogic(BaseClientLogic):
     """Wrapper which adds SecAgg methods."""
     
     def __init__(self, client: Client) -> None:
+        super().__init__(client)
         self.client: Client = client
     
     def fit(
         self, ins: FitIns,
     ) -> FitRes:
         stage = Time(ins.config[TIME])
         if stage == Time.SAY_HI:
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/msg_demo/server_logic.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/msg_demo/server_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     generate_fit_report,
     get_clients_from_list,
     get_configure_evaluate,
     aggregate_evaluate,
     generate_evaluate_report,
     wait_for_results,
 )
-from daisyfl.server import Server
+from daisyfl.utils.server import Server
 
 from daisyfl.operator.base.server_logic import ServerLogic as BaseServerLogic
 
 
 class ServerLogic(BaseServerLogic):
     def __init__(self,
         server: Server,
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/msg_demo/zone_client_logic.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/criterion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-
-
 # Copyright 2020 Adap GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from daisyfl.operator.base.client_logic import ClientLogic as BaseClientLogic
-from daisyfl.client import Client
-class ZoneClientLogic(BaseClientLogic):
-    """Wrapper which adds SecAgg methods."""
-    
-    def __init__(self, client) -> None:
-        self.client: Client = client
-    
+"""Abstract class for criterion sampling."""
+
+
+from abc import ABC, abstractmethod
+
+from .client_proxy import ClientProxy
+
+
+class Criterion(ABC):
+    """Abstract class which allows subclasses to implement criterion sampling."""
+
+    @abstractmethod
+    def select(self, client: ClientProxy) -> bool:
+        """Decide whether a client should be eligible for sampling or not."""
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/msg_demo/zone_server_logic.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/msg_demo/zone_server_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from logging import INFO, WARNING, ERROR
 from typing import Dict, List, Optional, Tuple, TypedDict, Callable
 from threading import Timer, Condition, Event
 from queue import Queue
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.client_proxy import ClientProxy
 from daisyfl.operator.strategy import Strategy
 from daisyfl.common import (
     Parameters,
     Report,
     Task,
     CURRENT_ROUND,
     TIMEOUT,
@@ -41,15 +41,15 @@
     generate_fit_report,
     get_configure_evaluate,
     aggregate_evaluate,
     generate_evaluate_report,
     wait_for_results,
     get_clients_from_list,
 )
-from daisyfl.server import Server
+from daisyfl.utils.server import Server
 from daisyfl.operator.base.server_logic import ServerLogic as BaseServerLogic
 
 
 class ZoneServerLogic(BaseServerLogic):
     def __init__(self,
         server: Server,
         strategy: Strategy,
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/sec_agg/client_logic.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/sec_agg/client_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from daisyfl.operator.base.client_logic import ClientLogic as BaseClientLogic
 from . import primitives
 
 class ClientLogic(BaseClientLogic):
     """Wrapper which adds SecAgg methods."""
     
     def __init__(self, client: Client) -> None:
+        super().__init__(client)
         self.client: Client = client
     
     def fit(
         self, ins: FitIns,
     ) -> FitRes:
         stage = Proto(ins.config[PROTO_KEY])
         if stage == Proto.SETUP:
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/sec_agg/common.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/sec_agg/common.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/sec_agg/primitives.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/sec_agg/primitives.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/sec_agg/server_logic.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/sec_agg/server_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,18 +49,18 @@
     FORWARD_PACKETS,
     ShareRequest,
     SHARE_REQUEST,
     SHARE_RESPONSE,
 )
 from . import primitives
 from daisyfl.operator.base.server_logic import ServerLogic as BaseServerLogic
-from daisyfl.server import Server
+from daisyfl.utils.server import Server
 from threading import Event, Condition, Timer
-from daisyfl.server.server import FitResultsAndFailures
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.server import FitResultsAndFailures
+from daisyfl.utils.client_proxy import ClientProxy
 from daisyfl.operator.utils import (
     get_configure_fit,
     generate_fit_report,
     wait_for_results,
     get_clients_from_list,
 )
 from daisyfl.common.logger import log
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/aggregate.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 import math
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 from daisyfl.common import FitIns, FitRes, Parameters, Scalar
-from daisyfl.server.client_manager import ClientManager
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.client_manager import ClientManager
+from daisyfl.utils.client_proxy import ClientProxy
 from daisyfl.operator.strategy.dpfedavg_fixed import DPFedAvgFixed
 from daisyfl.operator.strategy.strategy import Strategy
 
 
 class DPFedAvgAdaptive(DPFedAvgFixed):
     """Wrapper for configuring a Strategy for DP with Adaptive Clipping."""
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 """
 
 from typing import Dict, List, Optional, Tuple, Union
 
 from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar, CURRENT_ROUND, CurrentReturns, CheckResults
 from daisyfl.common.dp import add_gaussian_noise
 from daisyfl.common.parameter import ndarrays_to_parameters, parameters_to_ndarrays
-from daisyfl.server.server import Server
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.server import Server
+from daisyfl.utils.client_proxy import ClientProxy
 from daisyfl.operator.strategy.strategy import Strategy
 
 
 class DPFedAvgFixed(Strategy):
     """Wrapper for configuring a Strategy for DP with Fixed Clipping."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from daisyfl.common.logger import log
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg
 from .fedavg import FedAvg
 
 
 class FaultTolerantFedAvg(FedAvg):
     """Configurable fault-tolerant FedAvg strategy implementation."""
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedadagrad.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedadagrad.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.client_proxy import ClientProxy
 
 from .fedopt import FedOpt
 
 
 # pylint: disable=too-many-locals
 class FedAdagrad(FedOpt):
     """Adaptive Federated Optimization using Adagrad (FedAdagrad) [Reddi et
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedadam.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedadam.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.client_proxy import ClientProxy
 
 from .fedopt import FedOpt
 
 
 class FedAdam(FedOpt):
     """Adaptive Federated Optimization using Adam (FedAdam) [Reddi et al.,
     2020] strategy.
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedasync.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedasync.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     parameters_to_ndarrays,
     CURRENT_ROUND,
     CurrentReturns,
     CheckResults,
     ACCURACY,
 )
 from daisyfl.common.logger import log
-from daisyfl.server.server import Server
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.server import Server
+from daisyfl.utils.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg, aggregate_fedasync
 from .strategy import Strategy
 
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedavg.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedavg.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     ndarrays_to_parameters,
     parameters_to_ndarrays,
     CheckResults,
     CurrentReturns,
     ACCURACY,
 )
 from daisyfl.common.logger import log
-from daisyfl.server.server import Server
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.server import Server
+from daisyfl.utils.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg
 from .strategy import Strategy
 
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedavg_android.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedavg_android.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     NDArray,
     NDArrays,
     Parameters,
     Scalar,
     CurrentReturns,
     CheckResults,
 )
-from daisyfl.server.server import Server
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.server import Server
+from daisyfl.utils.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg
 from .strategy import Strategy
 
 
 class FedAvgAndroid(Strategy):
     """Configurable FedAvg strategy implementation."""
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedavgm.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedavgm.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from daisyfl.common.logger import log
-from daisyfl.server.server import Server
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.server import Server
+from daisyfl.utils.client_proxy import ClientProxy
 
 from .aggregate import aggregate
 from .fedavg import FedAvg
 
 WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedopt.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/fedyogi.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/fedyogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.client_proxy import ClientProxy
 
 from .fedopt import FedOpt
 
 
 class FedYogi(FedOpt):
     """Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al.,
     2020] strategy.
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/qfedavg.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/qfedavg.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from daisyfl.common.logger import log
-from daisyfl.server.server import Server
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.server import Server
+from daisyfl.utils.client_proxy import ClientProxy
 
 from .aggregate import aggregate_qffl, weighted_loss_avg
 from .fedavg import FedAvg
 
 
 # pylint: disable=too-many-locals
 class QFedAvg(FedAvg):
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/strategy/strategy.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/strategy/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 """Flower server strategy."""
 
 
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional, Tuple, Union
 
 from daisyfl.common import EvaluateIns, EvaluateRes, FitIns, FitRes, Parameters, Scalar, CheckResults, CurrentReturns
-from daisyfl.server.server import Server
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.server import Server
+from daisyfl.utils.client_proxy import ClientProxy
 
 
 class Strategy(ABC):
     """Abstract base class for server strategy implementations."""
 
     @abstractmethod
     def initialize_parameters(
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/utils/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/operator/utils/op_tools.py` & `daisyfl-0.5.3/src/py/daisyfl/operator/utils/op_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     SUBTASK_RETURNS_SELECTED,
     SUBTASK_RETURNS_ROAMING,
     INDIVIDUAL_CLIENT_METRICS,
     CID,
 )
 from daisyfl.common.logger import log
 from daisyfl.common.typing import GetParametersIns
-from daisyfl.server.server import Server
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.server import Server
+from daisyfl.utils.client_proxy import ClientProxy
 from daisyfl.operator.strategy import Strategy
 from threading import Condition
 
 FitResultsAndFailures = Tuple[
     List[Tuple[ClientProxy, FitRes]],
     List[Union[Tuple[ClientProxy, FitRes], BaseException]],
 ]
@@ -61,15 +61,15 @@
     client_instructions = strategy.configure_fit(
         server_round=server_round,
         parameters=parameters,
         server=server,
         credential=credential,
     )
     for i in range(len(client_instructions)):
-        client_instructions[i][1].config = config.copy()
+        client_instructions[i][1].config.update(config)
     return client_instructions
 
 def get_configure_evaluate(
     strategy: Strategy,
     server_round: int,
     parameters: Parameters,
     server: Server,
@@ -79,15 +79,15 @@
     client_instructions = strategy.configure_evaluate(
         server_round=server_round,
         parameters=parameters,
         server=server,
         credential=credential,
     )
     for i in range(len(client_instructions)):
-        client_instructions[i][1].config = config.copy()
+        client_instructions[i][1].config.update(config)
     return client_instructions
 
 def get_clients_from_list(
     server: Server,
     clients: List[Tuple[ClientProxy, Union[FitIns, EvaluateIns]]],
     timeout: float,
     credential: str,
@@ -131,14 +131,16 @@
         if calculate:
             # uploaded by zones
             if res.config[METRICS].__contains__(PARTICIPATION):
                 participation[SUBTASK_RETURNS_SELECTED] += res.config[METRICS][PARTICIPATION][SUBTASK_RETURNS_SELECTED] - 1
                 participation[SUBTASK_RETURNS_RESULTS] += res.config[METRICS][PARTICIPATION][SUBTASK_RETURNS_RESULTS] - 1
                 participation[SUBTASK_RETURNS_FAILURES] += res.config[METRICS][PARTICIPATION][SUBTASK_RETURNS_FAILURES]
                 participation[SUBTASK_RETURNS_ROAMING] += res.config[METRICS][PARTICIPATION][SUBTASK_RETURNS_ROAMING]
+        else:
+            participation = {}
         
     # Aggregate training results
     parameters, metrics = strategy.aggregate_fit(server_round, results_for_aggregate, failures)
     metrics[PARTICIPATION] = participation
     # num_examples
     num_examples = int(sum([res.config[FIT_SAMPLES] for _, res in results]))
     return parameters, num_examples, metrics
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/proto/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/proto/transport_pb2.py` & `daisyfl-0.5.3/src/py/daisyfl/proto/transport_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='daisyfl/proto/transport.proto',
   package='daisyfl.proto',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1d\x64\x61isyfl/proto/transport.proto\x12\rdaisyfl.proto\"<\n\x06Status\x12!\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x13.daisyfl.proto.Code\x12\x0f\n\x07message\x18\x02 \x01(\t\"2\n\nParameters\x12\x0f\n\x07tensors\x18\x01 \x03(\x0c\x12\x13\n\x0btensor_type\x18\x02 \x01(\t\"i\n\x06Scalar\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x42\x08\n\x06scalar\"7\n\tInnerList\x12*\n\ninner_list\x18\x01 \x03(\x0b\x32\x16.daisyfl.proto.Element\"\x8d\x01\n\x08InnerMap\x12\x38\n\tinner_map\x18\x01 \x03(\x0b\x32%.daisyfl.proto.InnerMap.InnerMapEntry\x1aG\n\rInnerMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.daisyfl.proto.Element:\x02\x38\x01\"\x9d\x01\n\x0bInnerMapInt\x12\x42\n\rinner_map_int\x18\x01 \x03(\x0b\x32+.daisyfl.proto.InnerMapInt.InnerMapIntEntry\x1aJ\n\x10InnerMapIntEntry\x12\x0b\n\x03key\x18\x01 \x01(\x03\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.daisyfl.proto.Element:\x02\x38\x01\"\xfe\x01\n\x07\x45lement\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x12,\n\tinner_map\x18\x10 \x01(\x0b\x32\x17.daisyfl.proto.InnerMapH\x00\x12\x33\n\rinner_map_int\x18\x11 \x01(\x0b\x32\x1a.daisyfl.proto.InnerMapIntH\x00\x12.\n\ninner_list\x18\x12 \x01(\x0b\x32\x18.daisyfl.proto.InnerListH\x00\x42\t\n\x07\x65lement\"\x9c\t\n\rServerMessage\x12\x42\n\rreconnect_ins\x18\x01 \x01(\x0b\x32).daisyfl.proto.ServerMessage.ReconnectInsH\x00\x12K\n\x12get_properties_ins\x18\x02 \x01(\x0b\x32-.daisyfl.proto.ServerMessage.GetPropertiesInsH\x00\x12K\n\x12get_parameters_ins\x18\x03 \x01(\x0b\x32-.daisyfl.proto.ServerMessage.GetParametersInsH\x00\x12\x36\n\x07\x66it_ins\x18\x04 \x01(\x0b\x32#.daisyfl.proto.ServerMessage.FitInsH\x00\x12@\n\x0c\x65valuate_ins\x18\x05 \x01(\x0b\x32(.daisyfl.proto.ServerMessage.EvaluateInsH\x00\x12S\n\x16server_received_signal\x18\x06 \x01(\x0b\x32\x31.daisyfl.proto.ServerMessage.ServerReceivedSignalH\x00\x12\x42\n\rserver_status\x18\x07 \x01(\x0b\x32).daisyfl.proto.ServerMessage.ServerStatusH\x00\x1a\x1f\n\x0cReconnectIns\x12\x0f\n\x07seconds\x18\x01 \x01(\x03\x1a\xa3\x01\n\x10GetPropertiesIns\x12I\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x39.daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry\x1a\x44\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1a\xa3\x01\n\x10GetParametersIns\x12I\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x39.daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry\x1a\x44\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1a`\n\x06\x46itIns\x12-\n\nparameters\x18\x01 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x65\n\x0b\x45valuateIns\x12-\n\nparameters\x18\x01 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a=\n\x14ServerReceivedSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x1a\x1e\n\x0cServerStatus\x12\x0e\n\x06status\x18\x01 \x01(\tB\x05\n\x03msg\"\xe0\n\n\rClientMessage\x12\x44\n\x0e\x64isconnect_res\x18\x01 \x01(\x0b\x32*.daisyfl.proto.ClientMessage.DisconnectResH\x00\x12K\n\x12get_properties_res\x18\x02 \x01(\x0b\x32-.daisyfl.proto.ClientMessage.GetPropertiesResH\x00\x12K\n\x12get_parameters_res\x18\x03 \x01(\x0b\x32-.daisyfl.proto.ClientMessage.GetParametersResH\x00\x12\x36\n\x07\x66it_res\x18\x04 \x01(\x0b\x32#.daisyfl.proto.ClientMessage.FitResH\x00\x12@\n\x0c\x65valuate_res\x18\x05 \x01(\x0b\x32(.daisyfl.proto.ClientMessage.EvaluateResH\x00\x12\x42\n\rclient_status\x18\x06 \x01(\x0b\x32).daisyfl.proto.ClientMessage.ClientStatusH\x00\x12U\n\x17\x63lient_uploading_signal\x18\x07 \x01(\x0b\x32\x32.daisyfl.proto.ClientMessage.ClientUploadingSignalH\x00\x12Q\n\x15\x63lient_roaming_signal\x18\x08 \x01(\x0b\x32\x30.daisyfl.proto.ClientMessage.ClientRoamingSignalH\x00\x1a\x36\n\rDisconnectRes\x12%\n\x06reason\x18\x01 \x01(\x0e\x32\x15.daisyfl.proto.Reason\x1a\xd6\x01\n\x10GetPropertiesRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12Q\n\nproperties\x18\x02 \x03(\x0b\x32=.daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry\x1aH\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1ah\n\x10GetParametersRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12-\n\nparameters\x18\x02 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x1a\x87\x01\n\x06\x46itRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12-\n\nparameters\x18\x02 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a]\n\x0b\x45valuateRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x1e\n\x0c\x43lientStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x1a>\n\x15\x43lientUploadingSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x1a<\n\x13\x43lientRoamingSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.StatusB\x05\n\x03msg*\x9f\x01\n\x04\x43ode\x12\x06\n\x02OK\x10\x00\x12\"\n\x1eGET_PROPERTIES_NOT_IMPLEMENTED\x10\x01\x12\"\n\x1eGET_PARAMETERS_NOT_IMPLEMENTED\x10\x02\x12\x17\n\x13\x46IT_NOT_IMPLEMENTED\x10\x03\x12\x1c\n\x18\x45VALUATE_NOT_IMPLEMENTED\x10\x04\x12\x10\n\x0cMESSAGE_LOST\x10\x05*[\n\x06Reason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tRECONNECT\x10\x01\x12\x16\n\x12POWER_DISCONNECTED\x10\x02\x12\x14\n\x10WIFI_UNAVAILABLE\x10\x03\x12\x07\n\x03\x41\x43K\x10\x04\x32Y\n\rFlowerService\x12H\n\x04Join\x12\x1c.daisyfl.proto.ClientMessage\x1a\x1c.daisyfl.proto.ServerMessage\"\x00(\x01\x30\x01\x62\x06proto3'
+  serialized_pb=b'\n\x1d\x64\x61isyfl/proto/transport.proto\x12\rdaisyfl.proto\"<\n\x06Status\x12!\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x13.daisyfl.proto.Code\x12\x0f\n\x07message\x18\x02 \x01(\t\"2\n\nParameters\x12\x0f\n\x07tensors\x18\x01 \x03(\x0c\x12\x13\n\x0btensor_type\x18\x02 \x01(\t\"i\n\x06Scalar\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x42\x08\n\x06scalar\"7\n\tInnerList\x12*\n\ninner_list\x18\x01 \x03(\x0b\x32\x16.daisyfl.proto.Element\"\x8d\x01\n\x08InnerMap\x12\x38\n\tinner_map\x18\x01 \x03(\x0b\x32%.daisyfl.proto.InnerMap.InnerMapEntry\x1aG\n\rInnerMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.daisyfl.proto.Element:\x02\x38\x01\"\x9d\x01\n\x0bInnerMapInt\x12\x42\n\rinner_map_int\x18\x01 \x03(\x0b\x32+.daisyfl.proto.InnerMapInt.InnerMapIntEntry\x1aJ\n\x10InnerMapIntEntry\x12\x0b\n\x03key\x18\x01 \x01(\x03\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.daisyfl.proto.Element:\x02\x38\x01\"\xfe\x01\n\x07\x45lement\x12\x10\n\x06\x64ouble\x18\x01 \x01(\x01H\x00\x12\x10\n\x06sint64\x18\x08 \x01(\x12H\x00\x12\x0e\n\x04\x62ool\x18\r \x01(\x08H\x00\x12\x10\n\x06string\x18\x0e \x01(\tH\x00\x12\x0f\n\x05\x62ytes\x18\x0f \x01(\x0cH\x00\x12,\n\tinner_map\x18\x10 \x01(\x0b\x32\x17.daisyfl.proto.InnerMapH\x00\x12\x33\n\rinner_map_int\x18\x11 \x01(\x0b\x32\x1a.daisyfl.proto.InnerMapIntH\x00\x12.\n\ninner_list\x18\x12 \x01(\x0b\x32\x18.daisyfl.proto.InnerListH\x00\x42\t\n\x07\x65lement\"\xa1\x0c\n\rServerMessage\x12\x42\n\rreconnect_ins\x18\x01 \x01(\x0b\x32).daisyfl.proto.ServerMessage.ReconnectInsH\x00\x12K\n\x12get_properties_ins\x18\x02 \x01(\x0b\x32-.daisyfl.proto.ServerMessage.GetPropertiesInsH\x00\x12K\n\x12get_parameters_ins\x18\x03 \x01(\x0b\x32-.daisyfl.proto.ServerMessage.GetParametersInsH\x00\x12\x36\n\x07\x66it_ins\x18\x04 \x01(\x0b\x32#.daisyfl.proto.ServerMessage.FitInsH\x00\x12@\n\x0c\x65valuate_ins\x18\x05 \x01(\x0b\x32(.daisyfl.proto.ServerMessage.EvaluateInsH\x00\x12S\n\x16server_received_signal\x18\x06 \x01(\x0b\x32\x31.daisyfl.proto.ServerMessage.ServerReceivedSignalH\x00\x12\x42\n\rserver_status\x18\x07 \x01(\x0b\x32).daisyfl.proto.ServerMessage.ServerStatusH\x00\x12U\n\x17\x63hain_proceeding_signal\x18\x08 \x01(\x0b\x32\x32.daisyfl.proto.ServerMessage.ChainProceedingSignalH\x00\x12N\n\x13reservation_success\x18\t \x01(\x0b\x32/.daisyfl.proto.ServerMessage.ReservationSuccessH\x00\x12N\n\x13reservation_failure\x18\n \x01(\x0b\x32/.daisyfl.proto.ServerMessage.ReservationFailureH\x00\x1a\x1f\n\x0cReconnectIns\x12\x0f\n\x07seconds\x18\x01 \x01(\x03\x1a\xa3\x01\n\x10GetPropertiesIns\x12I\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x39.daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry\x1a\x44\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1a\xa3\x01\n\x10GetParametersIns\x12I\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\x39.daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry\x1a\x44\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1a`\n\x06\x46itIns\x12-\n\nparameters\x18\x01 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x65\n\x0b\x45valuateIns\x12-\n\nparameters\x18\x01 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a=\n\x14ServerReceivedSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x1a\x1e\n\x0cServerStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x1a@\n\x15\x43hainProceedingSignal\x12\'\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a$\n\x12ReservationSuccess\x12\x0e\n\x06status\x18\x01 \x01(\t\x1a$\n\x12ReservationFailure\x12\x0e\n\x06status\x18\x01 \x01(\tB\x05\n\x03msg\"\xd1\x0f\n\rClientMessage\x12\x44\n\x0e\x64isconnect_res\x18\x01 \x01(\x0b\x32*.daisyfl.proto.ClientMessage.DisconnectResH\x00\x12K\n\x12get_properties_res\x18\x02 \x01(\x0b\x32-.daisyfl.proto.ClientMessage.GetPropertiesResH\x00\x12K\n\x12get_parameters_res\x18\x03 \x01(\x0b\x32-.daisyfl.proto.ClientMessage.GetParametersResH\x00\x12\x36\n\x07\x66it_res\x18\x04 \x01(\x0b\x32#.daisyfl.proto.ClientMessage.FitResH\x00\x12@\n\x0c\x65valuate_res\x18\x05 \x01(\x0b\x32(.daisyfl.proto.ClientMessage.EvaluateResH\x00\x12\x42\n\rclient_status\x18\x06 \x01(\x0b\x32).daisyfl.proto.ClientMessage.ClientStatusH\x00\x12U\n\x17\x63lient_uploading_signal\x18\x07 \x01(\x0b\x32\x32.daisyfl.proto.ClientMessage.ClientUploadingSignalH\x00\x12Q\n\x15\x63lient_roaming_signal\x18\x08 \x01(\x0b\x32\x30.daisyfl.proto.ClientMessage.ClientRoamingSignalH\x00\x12K\n\x12model_sync_request\x18\t \x01(\x0b\x32-.daisyfl.proto.ClientMessage.ModelSyncRequestH\x00\x12\x39\n\x08shutdown\x18\n \x01(\x0b\x32%.daisyfl.proto.ClientMessage.ShutdownH\x00\x12Q\n\x15\x63hain_transfer_signal\x18\x0b \x01(\x0b\x32\x30.daisyfl.proto.ClientMessage.ChainTransferSignalH\x00\x12[\n\x1amodel_transfer_reservation\x18\x0c \x01(\x0b\x32\x35.daisyfl.proto.ClientMessage.ModelTransferReservationH\x00\x1a\x36\n\rDisconnectRes\x12%\n\x06reason\x18\x01 \x01(\x0e\x32\x15.daisyfl.proto.Reason\x1a\xd6\x01\n\x10GetPropertiesRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12Q\n\nproperties\x18\x02 \x03(\x0b\x32=.daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry\x1aH\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.daisyfl.proto.Scalar:\x02\x38\x01\x1ah\n\x10GetParametersRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12-\n\nparameters\x18\x02 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x1a\x87\x01\n\x06\x46itRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12-\n\nparameters\x18\x02 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a]\n\x0b\x45valuateRes\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x1e\n\x0c\x43lientStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x1a>\n\x15\x43lientUploadingSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x1a<\n\x13\x43lientRoamingSignal\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x1aj\n\x10ModelSyncRequest\x12-\n\nparameters\x18\x01 \x01(\x0b\x32\x19.daisyfl.proto.Parameters\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x31\n\x08Shutdown\x12%\n\x06status\x18\x01 \x01(\x0b\x32\x15.daisyfl.proto.Status\x1aS\n\x13\x43hainTransferSignal\x12\x13\n\x0btransfer_to\x18\x01 \x01(\t\x12\'\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x17.daisyfl.proto.InnerMap\x1a\x43\n\x18ModelTransferReservation\x12\'\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x17.daisyfl.proto.InnerMapB\x05\n\x03msg*\x9f\x01\n\x04\x43ode\x12\x06\n\x02OK\x10\x00\x12\"\n\x1eGET_PROPERTIES_NOT_IMPLEMENTED\x10\x01\x12\"\n\x1eGET_PARAMETERS_NOT_IMPLEMENTED\x10\x02\x12\x17\n\x13\x46IT_NOT_IMPLEMENTED\x10\x03\x12\x1c\n\x18\x45VALUATE_NOT_IMPLEMENTED\x10\x04\x12\x10\n\x0cMESSAGE_LOST\x10\x05*[\n\x06Reason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\r\n\tRECONNECT\x10\x01\x12\x16\n\x12POWER_DISCONNECTED\x10\x02\x12\x14\n\x10WIFI_UNAVAILABLE\x10\x03\x12\x07\n\x03\x41\x43K\x10\x04\x32Y\n\rFlowerService\x12H\n\x04Join\x12\x1c.daisyfl.proto.ClientMessage\x1a\x1c.daisyfl.proto.ServerMessage\"\x00(\x01\x30\x01\x62\x06proto3'
 )
 
 _CODE = _descriptor.EnumDescriptor(
   name='Code',
   full_name='daisyfl.proto.Code',
   filename=None,
   file=DESCRIPTOR,
@@ -59,16 +59,16 @@
       name='MESSAGE_LOST', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3450,
-  serialized_end=3609,
+  serialized_start=4464,
+  serialized_end=4623,
 )
 _sym_db.RegisterEnumDescriptor(_CODE)
 
 Code = enum_type_wrapper.EnumTypeWrapper(_CODE)
 _REASON = _descriptor.EnumDescriptor(
   name='Reason',
   full_name='daisyfl.proto.Reason',
@@ -100,16 +100,16 @@
       name='ACK', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3611,
-  serialized_end=3702,
+  serialized_start=4625,
+  serialized_end=4716,
 )
 _sym_db.RegisterEnumDescriptor(_REASON)
 
 Reason = enum_type_wrapper.EnumTypeWrapper(_REASON)
 OK = 0
 GET_PROPERTIES_NOT_IMPLEMENTED = 1
 GET_PARAMETERS_NOT_IMPLEMENTED = 2
@@ -548,16 +548,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1402,
-  serialized_end=1433,
+  serialized_start=1649,
+  serialized_end=1680,
 )
 
 _SERVERMESSAGE_GETPROPERTIESINS_CONFIGENTRY = _descriptor.Descriptor(
   name='ConfigEntry',
   full_name='daisyfl.proto.ServerMessage.GetPropertiesIns.ConfigEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -586,16 +586,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1531,
-  serialized_end=1599,
+  serialized_start=1778,
+  serialized_end=1846,
 )
 
 _SERVERMESSAGE_GETPROPERTIESINS = _descriptor.Descriptor(
   name='GetPropertiesIns',
   full_name='daisyfl.proto.ServerMessage.GetPropertiesIns',
   filename=None,
   file=DESCRIPTOR,
@@ -617,16 +617,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1436,
-  serialized_end=1599,
+  serialized_start=1683,
+  serialized_end=1846,
 )
 
 _SERVERMESSAGE_GETPARAMETERSINS_CONFIGENTRY = _descriptor.Descriptor(
   name='ConfigEntry',
   full_name='daisyfl.proto.ServerMessage.GetParametersIns.ConfigEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -655,16 +655,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1531,
-  serialized_end=1599,
+  serialized_start=1778,
+  serialized_end=1846,
 )
 
 _SERVERMESSAGE_GETPARAMETERSINS = _descriptor.Descriptor(
   name='GetParametersIns',
   full_name='daisyfl.proto.ServerMessage.GetParametersIns',
   filename=None,
   file=DESCRIPTOR,
@@ -686,16 +686,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1602,
-  serialized_end=1765,
+  serialized_start=1849,
+  serialized_end=2012,
 )
 
 _SERVERMESSAGE_FITINS = _descriptor.Descriptor(
   name='FitIns',
   full_name='daisyfl.proto.ServerMessage.FitIns',
   filename=None,
   file=DESCRIPTOR,
@@ -724,16 +724,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1767,
-  serialized_end=1863,
+  serialized_start=2014,
+  serialized_end=2110,
 )
 
 _SERVERMESSAGE_EVALUATEINS = _descriptor.Descriptor(
   name='EvaluateIns',
   full_name='daisyfl.proto.ServerMessage.EvaluateIns',
   filename=None,
   file=DESCRIPTOR,
@@ -762,16 +762,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1865,
-  serialized_end=1966,
+  serialized_start=2112,
+  serialized_end=2213,
 )
 
 _SERVERMESSAGE_SERVERRECEIVEDSIGNAL = _descriptor.Descriptor(
   name='ServerReceivedSignal',
   full_name='daisyfl.proto.ServerMessage.ServerReceivedSignal',
   filename=None,
   file=DESCRIPTOR,
@@ -793,16 +793,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1968,
-  serialized_end=2029,
+  serialized_start=2215,
+  serialized_end=2276,
 )
 
 _SERVERMESSAGE_SERVERSTATUS = _descriptor.Descriptor(
   name='ServerStatus',
   full_name='daisyfl.proto.ServerMessage.ServerStatus',
   filename=None,
   file=DESCRIPTOR,
@@ -824,16 +824,109 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2031,
-  serialized_end=2061,
+  serialized_start=2278,
+  serialized_end=2308,
+)
+
+_SERVERMESSAGE_CHAINPROCEEDINGSIGNAL = _descriptor.Descriptor(
+  name='ChainProceedingSignal',
+  full_name='daisyfl.proto.ServerMessage.ChainProceedingSignal',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='config', full_name='daisyfl.proto.ServerMessage.ChainProceedingSignal.config', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2310,
+  serialized_end=2374,
+)
+
+_SERVERMESSAGE_RESERVATIONSUCCESS = _descriptor.Descriptor(
+  name='ReservationSuccess',
+  full_name='daisyfl.proto.ServerMessage.ReservationSuccess',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='daisyfl.proto.ServerMessage.ReservationSuccess.status', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2376,
+  serialized_end=2412,
+)
+
+_SERVERMESSAGE_RESERVATIONFAILURE = _descriptor.Descriptor(
+  name='ReservationFailure',
+  full_name='daisyfl.proto.ServerMessage.ReservationFailure',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='daisyfl.proto.ServerMessage.ReservationFailure.status', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2414,
+  serialized_end=2450,
 )
 
 _SERVERMESSAGE = _descriptor.Descriptor(
   name='ServerMessage',
   full_name='daisyfl.proto.ServerMessage',
   filename=None,
   file=DESCRIPTOR,
@@ -885,33 +978,54 @@
     _descriptor.FieldDescriptor(
       name='server_status', full_name='daisyfl.proto.ServerMessage.server_status', index=6,
       number=7, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='chain_proceeding_signal', full_name='daisyfl.proto.ServerMessage.chain_proceeding_signal', index=7,
+      number=8, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='reservation_success', full_name='daisyfl.proto.ServerMessage.reservation_success', index=8,
+      number=9, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='reservation_failure', full_name='daisyfl.proto.ServerMessage.reservation_failure', index=9,
+      number=10, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_SERVERMESSAGE_RECONNECTINS, _SERVERMESSAGE_GETPROPERTIESINS, _SERVERMESSAGE_GETPARAMETERSINS, _SERVERMESSAGE_FITINS, _SERVERMESSAGE_EVALUATEINS, _SERVERMESSAGE_SERVERRECEIVEDSIGNAL, _SERVERMESSAGE_SERVERSTATUS, ],
+  nested_types=[_SERVERMESSAGE_RECONNECTINS, _SERVERMESSAGE_GETPROPERTIESINS, _SERVERMESSAGE_GETPARAMETERSINS, _SERVERMESSAGE_FITINS, _SERVERMESSAGE_EVALUATEINS, _SERVERMESSAGE_SERVERRECEIVEDSIGNAL, _SERVERMESSAGE_SERVERSTATUS, _SERVERMESSAGE_CHAINPROCEEDINGSIGNAL, _SERVERMESSAGE_RESERVATIONSUCCESS, _SERVERMESSAGE_RESERVATIONFAILURE, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='msg', full_name='daisyfl.proto.ServerMessage.msg',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
   serialized_start=888,
-  serialized_end=2068,
+  serialized_end=2457,
 )
 
 
 _CLIENTMESSAGE_DISCONNECTRES = _descriptor.Descriptor(
   name='DisconnectRes',
   full_name='daisyfl.proto.ClientMessage.DisconnectRes',
   filename=None,
@@ -934,16 +1048,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2672,
-  serialized_end=2726,
+  serialized_start=3373,
+  serialized_end=3427,
 )
 
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY = _descriptor.Descriptor(
   name='PropertiesEntry',
   full_name='daisyfl.proto.ClientMessage.GetPropertiesRes.PropertiesEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -972,16 +1086,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2871,
-  serialized_end=2943,
+  serialized_start=3572,
+  serialized_end=3644,
 )
 
 _CLIENTMESSAGE_GETPROPERTIESRES = _descriptor.Descriptor(
   name='GetPropertiesRes',
   full_name='daisyfl.proto.ClientMessage.GetPropertiesRes',
   filename=None,
   file=DESCRIPTOR,
@@ -1010,16 +1124,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2729,
-  serialized_end=2943,
+  serialized_start=3430,
+  serialized_end=3644,
 )
 
 _CLIENTMESSAGE_GETPARAMETERSRES = _descriptor.Descriptor(
   name='GetParametersRes',
   full_name='daisyfl.proto.ClientMessage.GetParametersRes',
   filename=None,
   file=DESCRIPTOR,
@@ -1048,16 +1162,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2945,
-  serialized_end=3049,
+  serialized_start=3646,
+  serialized_end=3750,
 )
 
 _CLIENTMESSAGE_FITRES = _descriptor.Descriptor(
   name='FitRes',
   full_name='daisyfl.proto.ClientMessage.FitRes',
   filename=None,
   file=DESCRIPTOR,
@@ -1093,16 +1207,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3052,
-  serialized_end=3187,
+  serialized_start=3753,
+  serialized_end=3888,
 )
 
 _CLIENTMESSAGE_EVALUATERES = _descriptor.Descriptor(
   name='EvaluateRes',
   full_name='daisyfl.proto.ClientMessage.EvaluateRes',
   filename=None,
   file=DESCRIPTOR,
@@ -1131,16 +1245,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3189,
-  serialized_end=3282,
+  serialized_start=3890,
+  serialized_end=3983,
 )
 
 _CLIENTMESSAGE_CLIENTSTATUS = _descriptor.Descriptor(
   name='ClientStatus',
   full_name='daisyfl.proto.ClientMessage.ClientStatus',
   filename=None,
   file=DESCRIPTOR,
@@ -1162,16 +1276,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3284,
-  serialized_end=3314,
+  serialized_start=3985,
+  serialized_end=4015,
 )
 
 _CLIENTMESSAGE_CLIENTUPLOADINGSIGNAL = _descriptor.Descriptor(
   name='ClientUploadingSignal',
   full_name='daisyfl.proto.ClientMessage.ClientUploadingSignal',
   filename=None,
   file=DESCRIPTOR,
@@ -1193,16 +1307,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3316,
-  serialized_end=3378,
+  serialized_start=4017,
+  serialized_end=4079,
 )
 
 _CLIENTMESSAGE_CLIENTROAMINGSIGNAL = _descriptor.Descriptor(
   name='ClientRoamingSignal',
   full_name='daisyfl.proto.ClientMessage.ClientRoamingSignal',
   filename=None,
   file=DESCRIPTOR,
@@ -1224,16 +1338,154 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3380,
-  serialized_end=3440,
+  serialized_start=4081,
+  serialized_end=4141,
+)
+
+_CLIENTMESSAGE_MODELSYNCREQUEST = _descriptor.Descriptor(
+  name='ModelSyncRequest',
+  full_name='daisyfl.proto.ClientMessage.ModelSyncRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='parameters', full_name='daisyfl.proto.ClientMessage.ModelSyncRequest.parameters', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='config', full_name='daisyfl.proto.ClientMessage.ModelSyncRequest.config', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4143,
+  serialized_end=4249,
+)
+
+_CLIENTMESSAGE_SHUTDOWN = _descriptor.Descriptor(
+  name='Shutdown',
+  full_name='daisyfl.proto.ClientMessage.Shutdown',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='daisyfl.proto.ClientMessage.Shutdown.status', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4251,
+  serialized_end=4300,
+)
+
+_CLIENTMESSAGE_CHAINTRANSFERSIGNAL = _descriptor.Descriptor(
+  name='ChainTransferSignal',
+  full_name='daisyfl.proto.ClientMessage.ChainTransferSignal',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='transfer_to', full_name='daisyfl.proto.ClientMessage.ChainTransferSignal.transfer_to', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='config', full_name='daisyfl.proto.ClientMessage.ChainTransferSignal.config', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4302,
+  serialized_end=4385,
+)
+
+_CLIENTMESSAGE_MODELTRANSFERRESERVATION = _descriptor.Descriptor(
+  name='ModelTransferReservation',
+  full_name='daisyfl.proto.ClientMessage.ModelTransferReservation',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='config', full_name='daisyfl.proto.ClientMessage.ModelTransferReservation.config', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4387,
+  serialized_end=4454,
 )
 
 _CLIENTMESSAGE = _descriptor.Descriptor(
   name='ClientMessage',
   full_name='daisyfl.proto.ClientMessage',
   filename=None,
   file=DESCRIPTOR,
@@ -1292,33 +1544,61 @@
     _descriptor.FieldDescriptor(
       name='client_roaming_signal', full_name='daisyfl.proto.ClientMessage.client_roaming_signal', index=7,
       number=8, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='model_sync_request', full_name='daisyfl.proto.ClientMessage.model_sync_request', index=8,
+      number=9, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='shutdown', full_name='daisyfl.proto.ClientMessage.shutdown', index=9,
+      number=10, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='chain_transfer_signal', full_name='daisyfl.proto.ClientMessage.chain_transfer_signal', index=10,
+      number=11, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='model_transfer_reservation', full_name='daisyfl.proto.ClientMessage.model_transfer_reservation', index=11,
+      number=12, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_CLIENTMESSAGE_DISCONNECTRES, _CLIENTMESSAGE_GETPROPERTIESRES, _CLIENTMESSAGE_GETPARAMETERSRES, _CLIENTMESSAGE_FITRES, _CLIENTMESSAGE_EVALUATERES, _CLIENTMESSAGE_CLIENTSTATUS, _CLIENTMESSAGE_CLIENTUPLOADINGSIGNAL, _CLIENTMESSAGE_CLIENTROAMINGSIGNAL, ],
+  nested_types=[_CLIENTMESSAGE_DISCONNECTRES, _CLIENTMESSAGE_GETPROPERTIESRES, _CLIENTMESSAGE_GETPARAMETERSRES, _CLIENTMESSAGE_FITRES, _CLIENTMESSAGE_EVALUATERES, _CLIENTMESSAGE_CLIENTSTATUS, _CLIENTMESSAGE_CLIENTUPLOADINGSIGNAL, _CLIENTMESSAGE_CLIENTROAMINGSIGNAL, _CLIENTMESSAGE_MODELSYNCREQUEST, _CLIENTMESSAGE_SHUTDOWN, _CLIENTMESSAGE_CHAINTRANSFERSIGNAL, _CLIENTMESSAGE_MODELTRANSFERRESERVATION, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='msg', full_name='daisyfl.proto.ClientMessage.msg',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2071,
-  serialized_end=3447,
+  serialized_start=2460,
+  serialized_end=4461,
 )
 
 _STATUS.fields_by_name['code'].enum_type = _CODE
 _SCALAR.oneofs_by_name['scalar'].fields.append(
   _SCALAR.fields_by_name['double'])
 _SCALAR.fields_by_name['double'].containing_oneof = _SCALAR.oneofs_by_name['scalar']
 _SCALAR.oneofs_by_name['scalar'].fields.append(
@@ -1381,21 +1661,28 @@
 _SERVERMESSAGE_FITINS.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE_EVALUATEINS.fields_by_name['parameters'].message_type = _PARAMETERS
 _SERVERMESSAGE_EVALUATEINS.fields_by_name['config'].message_type = _INNERMAP
 _SERVERMESSAGE_EVALUATEINS.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE_SERVERRECEIVEDSIGNAL.fields_by_name['status'].message_type = _STATUS
 _SERVERMESSAGE_SERVERRECEIVEDSIGNAL.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE_SERVERSTATUS.containing_type = _SERVERMESSAGE
+_SERVERMESSAGE_CHAINPROCEEDINGSIGNAL.fields_by_name['config'].message_type = _INNERMAP
+_SERVERMESSAGE_CHAINPROCEEDINGSIGNAL.containing_type = _SERVERMESSAGE
+_SERVERMESSAGE_RESERVATIONSUCCESS.containing_type = _SERVERMESSAGE
+_SERVERMESSAGE_RESERVATIONFAILURE.containing_type = _SERVERMESSAGE
 _SERVERMESSAGE.fields_by_name['reconnect_ins'].message_type = _SERVERMESSAGE_RECONNECTINS
 _SERVERMESSAGE.fields_by_name['get_properties_ins'].message_type = _SERVERMESSAGE_GETPROPERTIESINS
 _SERVERMESSAGE.fields_by_name['get_parameters_ins'].message_type = _SERVERMESSAGE_GETPARAMETERSINS
 _SERVERMESSAGE.fields_by_name['fit_ins'].message_type = _SERVERMESSAGE_FITINS
 _SERVERMESSAGE.fields_by_name['evaluate_ins'].message_type = _SERVERMESSAGE_EVALUATEINS
 _SERVERMESSAGE.fields_by_name['server_received_signal'].message_type = _SERVERMESSAGE_SERVERRECEIVEDSIGNAL
 _SERVERMESSAGE.fields_by_name['server_status'].message_type = _SERVERMESSAGE_SERVERSTATUS
+_SERVERMESSAGE.fields_by_name['chain_proceeding_signal'].message_type = _SERVERMESSAGE_CHAINPROCEEDINGSIGNAL
+_SERVERMESSAGE.fields_by_name['reservation_success'].message_type = _SERVERMESSAGE_RESERVATIONSUCCESS
+_SERVERMESSAGE.fields_by_name['reservation_failure'].message_type = _SERVERMESSAGE_RESERVATIONFAILURE
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['reconnect_ins'])
 _SERVERMESSAGE.fields_by_name['reconnect_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['get_properties_ins'])
 _SERVERMESSAGE.fields_by_name['get_properties_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
@@ -1409,14 +1696,23 @@
 _SERVERMESSAGE.fields_by_name['evaluate_ins'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['server_received_signal'])
 _SERVERMESSAGE.fields_by_name['server_received_signal'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
   _SERVERMESSAGE.fields_by_name['server_status'])
 _SERVERMESSAGE.fields_by_name['server_status'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
+_SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
+  _SERVERMESSAGE.fields_by_name['chain_proceeding_signal'])
+_SERVERMESSAGE.fields_by_name['chain_proceeding_signal'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
+_SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
+  _SERVERMESSAGE.fields_by_name['reservation_success'])
+_SERVERMESSAGE.fields_by_name['reservation_success'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
+_SERVERMESSAGE.oneofs_by_name['msg'].fields.append(
+  _SERVERMESSAGE.fields_by_name['reservation_failure'])
+_SERVERMESSAGE.fields_by_name['reservation_failure'].containing_oneof = _SERVERMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE_DISCONNECTRES.fields_by_name['reason'].enum_type = _REASON
 _CLIENTMESSAGE_DISCONNECTRES.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY.fields_by_name['value'].message_type = _SCALAR
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY.containing_type = _CLIENTMESSAGE_GETPROPERTIESRES
 _CLIENTMESSAGE_GETPROPERTIESRES.fields_by_name['status'].message_type = _STATUS
 _CLIENTMESSAGE_GETPROPERTIESRES.fields_by_name['properties'].message_type = _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY
 _CLIENTMESSAGE_GETPROPERTIESRES.containing_type = _CLIENTMESSAGE
@@ -1431,22 +1727,35 @@
 _CLIENTMESSAGE_EVALUATERES.fields_by_name['config'].message_type = _INNERMAP
 _CLIENTMESSAGE_EVALUATERES.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE_CLIENTSTATUS.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE_CLIENTUPLOADINGSIGNAL.fields_by_name['status'].message_type = _STATUS
 _CLIENTMESSAGE_CLIENTUPLOADINGSIGNAL.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE_CLIENTROAMINGSIGNAL.fields_by_name['status'].message_type = _STATUS
 _CLIENTMESSAGE_CLIENTROAMINGSIGNAL.containing_type = _CLIENTMESSAGE
+_CLIENTMESSAGE_MODELSYNCREQUEST.fields_by_name['parameters'].message_type = _PARAMETERS
+_CLIENTMESSAGE_MODELSYNCREQUEST.fields_by_name['config'].message_type = _INNERMAP
+_CLIENTMESSAGE_MODELSYNCREQUEST.containing_type = _CLIENTMESSAGE
+_CLIENTMESSAGE_SHUTDOWN.fields_by_name['status'].message_type = _STATUS
+_CLIENTMESSAGE_SHUTDOWN.containing_type = _CLIENTMESSAGE
+_CLIENTMESSAGE_CHAINTRANSFERSIGNAL.fields_by_name['config'].message_type = _INNERMAP
+_CLIENTMESSAGE_CHAINTRANSFERSIGNAL.containing_type = _CLIENTMESSAGE
+_CLIENTMESSAGE_MODELTRANSFERRESERVATION.fields_by_name['config'].message_type = _INNERMAP
+_CLIENTMESSAGE_MODELTRANSFERRESERVATION.containing_type = _CLIENTMESSAGE
 _CLIENTMESSAGE.fields_by_name['disconnect_res'].message_type = _CLIENTMESSAGE_DISCONNECTRES
 _CLIENTMESSAGE.fields_by_name['get_properties_res'].message_type = _CLIENTMESSAGE_GETPROPERTIESRES
 _CLIENTMESSAGE.fields_by_name['get_parameters_res'].message_type = _CLIENTMESSAGE_GETPARAMETERSRES
 _CLIENTMESSAGE.fields_by_name['fit_res'].message_type = _CLIENTMESSAGE_FITRES
 _CLIENTMESSAGE.fields_by_name['evaluate_res'].message_type = _CLIENTMESSAGE_EVALUATERES
 _CLIENTMESSAGE.fields_by_name['client_status'].message_type = _CLIENTMESSAGE_CLIENTSTATUS
 _CLIENTMESSAGE.fields_by_name['client_uploading_signal'].message_type = _CLIENTMESSAGE_CLIENTUPLOADINGSIGNAL
 _CLIENTMESSAGE.fields_by_name['client_roaming_signal'].message_type = _CLIENTMESSAGE_CLIENTROAMINGSIGNAL
+_CLIENTMESSAGE.fields_by_name['model_sync_request'].message_type = _CLIENTMESSAGE_MODELSYNCREQUEST
+_CLIENTMESSAGE.fields_by_name['shutdown'].message_type = _CLIENTMESSAGE_SHUTDOWN
+_CLIENTMESSAGE.fields_by_name['chain_transfer_signal'].message_type = _CLIENTMESSAGE_CHAINTRANSFERSIGNAL
+_CLIENTMESSAGE.fields_by_name['model_transfer_reservation'].message_type = _CLIENTMESSAGE_MODELTRANSFERRESERVATION
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['disconnect_res'])
 _CLIENTMESSAGE.fields_by_name['disconnect_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['get_properties_res'])
 _CLIENTMESSAGE.fields_by_name['get_properties_res'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
@@ -1463,14 +1772,26 @@
 _CLIENTMESSAGE.fields_by_name['client_status'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['client_uploading_signal'])
 _CLIENTMESSAGE.fields_by_name['client_uploading_signal'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 _CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
   _CLIENTMESSAGE.fields_by_name['client_roaming_signal'])
 _CLIENTMESSAGE.fields_by_name['client_roaming_signal'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
+_CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
+  _CLIENTMESSAGE.fields_by_name['model_sync_request'])
+_CLIENTMESSAGE.fields_by_name['model_sync_request'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
+_CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
+  _CLIENTMESSAGE.fields_by_name['shutdown'])
+_CLIENTMESSAGE.fields_by_name['shutdown'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
+_CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
+  _CLIENTMESSAGE.fields_by_name['chain_transfer_signal'])
+_CLIENTMESSAGE.fields_by_name['chain_transfer_signal'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
+_CLIENTMESSAGE.oneofs_by_name['msg'].fields.append(
+  _CLIENTMESSAGE.fields_by_name['model_transfer_reservation'])
+_CLIENTMESSAGE.fields_by_name['model_transfer_reservation'].containing_oneof = _CLIENTMESSAGE.oneofs_by_name['msg']
 DESCRIPTOR.message_types_by_name['Status'] = _STATUS
 DESCRIPTOR.message_types_by_name['Parameters'] = _PARAMETERS
 DESCRIPTOR.message_types_by_name['Scalar'] = _SCALAR
 DESCRIPTOR.message_types_by_name['InnerList'] = _INNERLIST
 DESCRIPTOR.message_types_by_name['InnerMap'] = _INNERMAP
 DESCRIPTOR.message_types_by_name['InnerMapInt'] = _INNERMAPINT
 DESCRIPTOR.message_types_by_name['Element'] = _ELEMENT
@@ -1605,28 +1926,52 @@
 
   'ServerStatus' : _reflection.GeneratedProtocolMessageType('ServerStatus', (_message.Message,), {
     'DESCRIPTOR' : _SERVERMESSAGE_SERVERSTATUS,
     '__module__' : 'daisyfl.proto.transport_pb2'
     # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.ServerStatus)
     })
   ,
+
+  'ChainProceedingSignal' : _reflection.GeneratedProtocolMessageType('ChainProceedingSignal', (_message.Message,), {
+    'DESCRIPTOR' : _SERVERMESSAGE_CHAINPROCEEDINGSIGNAL,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.ChainProceedingSignal)
+    })
+  ,
+
+  'ReservationSuccess' : _reflection.GeneratedProtocolMessageType('ReservationSuccess', (_message.Message,), {
+    'DESCRIPTOR' : _SERVERMESSAGE_RESERVATIONSUCCESS,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.ReservationSuccess)
+    })
+  ,
+
+  'ReservationFailure' : _reflection.GeneratedProtocolMessageType('ReservationFailure', (_message.Message,), {
+    'DESCRIPTOR' : _SERVERMESSAGE_RESERVATIONFAILURE,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage.ReservationFailure)
+    })
+  ,
   'DESCRIPTOR' : _SERVERMESSAGE,
   '__module__' : 'daisyfl.proto.transport_pb2'
   # @@protoc_insertion_point(class_scope:daisyfl.proto.ServerMessage)
   })
 _sym_db.RegisterMessage(ServerMessage)
 _sym_db.RegisterMessage(ServerMessage.ReconnectIns)
 _sym_db.RegisterMessage(ServerMessage.GetPropertiesIns)
 _sym_db.RegisterMessage(ServerMessage.GetPropertiesIns.ConfigEntry)
 _sym_db.RegisterMessage(ServerMessage.GetParametersIns)
 _sym_db.RegisterMessage(ServerMessage.GetParametersIns.ConfigEntry)
 _sym_db.RegisterMessage(ServerMessage.FitIns)
 _sym_db.RegisterMessage(ServerMessage.EvaluateIns)
 _sym_db.RegisterMessage(ServerMessage.ServerReceivedSignal)
 _sym_db.RegisterMessage(ServerMessage.ServerStatus)
+_sym_db.RegisterMessage(ServerMessage.ChainProceedingSignal)
+_sym_db.RegisterMessage(ServerMessage.ReservationSuccess)
+_sym_db.RegisterMessage(ServerMessage.ReservationFailure)
 
 ClientMessage = _reflection.GeneratedProtocolMessageType('ClientMessage', (_message.Message,), {
 
   'DisconnectRes' : _reflection.GeneratedProtocolMessageType('DisconnectRes', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_DISCONNECTRES,
     '__module__' : 'daisyfl.proto.transport_pb2'
     # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.DisconnectRes)
@@ -1684,28 +2029,60 @@
 
   'ClientRoamingSignal' : _reflection.GeneratedProtocolMessageType('ClientRoamingSignal', (_message.Message,), {
     'DESCRIPTOR' : _CLIENTMESSAGE_CLIENTROAMINGSIGNAL,
     '__module__' : 'daisyfl.proto.transport_pb2'
     # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.ClientRoamingSignal)
     })
   ,
+
+  'ModelSyncRequest' : _reflection.GeneratedProtocolMessageType('ModelSyncRequest', (_message.Message,), {
+    'DESCRIPTOR' : _CLIENTMESSAGE_MODELSYNCREQUEST,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.ModelSyncRequest)
+    })
+  ,
+
+  'Shutdown' : _reflection.GeneratedProtocolMessageType('Shutdown', (_message.Message,), {
+    'DESCRIPTOR' : _CLIENTMESSAGE_SHUTDOWN,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.Shutdown)
+    })
+  ,
+
+  'ChainTransferSignal' : _reflection.GeneratedProtocolMessageType('ChainTransferSignal', (_message.Message,), {
+    'DESCRIPTOR' : _CLIENTMESSAGE_CHAINTRANSFERSIGNAL,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.ChainTransferSignal)
+    })
+  ,
+
+  'ModelTransferReservation' : _reflection.GeneratedProtocolMessageType('ModelTransferReservation', (_message.Message,), {
+    'DESCRIPTOR' : _CLIENTMESSAGE_MODELTRANSFERRESERVATION,
+    '__module__' : 'daisyfl.proto.transport_pb2'
+    # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage.ModelTransferReservation)
+    })
+  ,
   'DESCRIPTOR' : _CLIENTMESSAGE,
   '__module__' : 'daisyfl.proto.transport_pb2'
   # @@protoc_insertion_point(class_scope:daisyfl.proto.ClientMessage)
   })
 _sym_db.RegisterMessage(ClientMessage)
 _sym_db.RegisterMessage(ClientMessage.DisconnectRes)
 _sym_db.RegisterMessage(ClientMessage.GetPropertiesRes)
 _sym_db.RegisterMessage(ClientMessage.GetPropertiesRes.PropertiesEntry)
 _sym_db.RegisterMessage(ClientMessage.GetParametersRes)
 _sym_db.RegisterMessage(ClientMessage.FitRes)
 _sym_db.RegisterMessage(ClientMessage.EvaluateRes)
 _sym_db.RegisterMessage(ClientMessage.ClientStatus)
 _sym_db.RegisterMessage(ClientMessage.ClientUploadingSignal)
 _sym_db.RegisterMessage(ClientMessage.ClientRoamingSignal)
+_sym_db.RegisterMessage(ClientMessage.ModelSyncRequest)
+_sym_db.RegisterMessage(ClientMessage.Shutdown)
+_sym_db.RegisterMessage(ClientMessage.ChainTransferSignal)
+_sym_db.RegisterMessage(ClientMessage.ModelTransferReservation)
 
 
 _INNERMAP_INNERMAPENTRY._options = None
 _INNERMAPINT_INNERMAPINTENTRY._options = None
 _SERVERMESSAGE_GETPROPERTIESINS_CONFIGENTRY._options = None
 _SERVERMESSAGE_GETPARAMETERSINS_CONFIGENTRY._options = None
 _CLIENTMESSAGE_GETPROPERTIESRES_PROPERTIESENTRY._options = None
@@ -1713,16 +2090,16 @@
 _FLOWERSERVICE = _descriptor.ServiceDescriptor(
   name='FlowerService',
   full_name='daisyfl.proto.FlowerService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=3704,
-  serialized_end=3793,
+  serialized_start=4718,
+  serialized_end=4807,
   methods=[
   _descriptor.MethodDescriptor(
     name='Join',
     full_name='daisyfl.proto.FlowerService.Join',
     index=0,
     containing_service=None,
     input_type=_CLIENTMESSAGE,
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/proto/transport_pb2.pyi` & `daisyfl-0.5.3/src/py/daisyfl/proto/transport_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -355,48 +355,92 @@
         status: typing.Text
         def __init__(self,
             *,
             status: typing.Text = ...,
             ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
 
+    class ChainProceedingSignal(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        CONFIG_FIELD_NUMBER: builtins.int
+        @property
+        def config(self) -> global___InnerMap: ...
+        def __init__(self,
+            *,
+            config: typing.Optional[global___InnerMap] = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["config",b"config"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["config",b"config"]) -> None: ...
+
+    class ReservationSuccess(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        STATUS_FIELD_NUMBER: builtins.int
+        status: typing.Text
+        def __init__(self,
+            *,
+            status: typing.Text = ...,
+            ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
+
+    class ReservationFailure(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        STATUS_FIELD_NUMBER: builtins.int
+        status: typing.Text
+        def __init__(self,
+            *,
+            status: typing.Text = ...,
+            ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
+
     RECONNECT_INS_FIELD_NUMBER: builtins.int
     GET_PROPERTIES_INS_FIELD_NUMBER: builtins.int
     GET_PARAMETERS_INS_FIELD_NUMBER: builtins.int
     FIT_INS_FIELD_NUMBER: builtins.int
     EVALUATE_INS_FIELD_NUMBER: builtins.int
     SERVER_RECEIVED_SIGNAL_FIELD_NUMBER: builtins.int
     SERVER_STATUS_FIELD_NUMBER: builtins.int
+    CHAIN_PROCEEDING_SIGNAL_FIELD_NUMBER: builtins.int
+    RESERVATION_SUCCESS_FIELD_NUMBER: builtins.int
+    RESERVATION_FAILURE_FIELD_NUMBER: builtins.int
     @property
     def reconnect_ins(self) -> global___ServerMessage.ReconnectIns: ...
     @property
     def get_properties_ins(self) -> global___ServerMessage.GetPropertiesIns: ...
     @property
     def get_parameters_ins(self) -> global___ServerMessage.GetParametersIns: ...
     @property
     def fit_ins(self) -> global___ServerMessage.FitIns: ...
     @property
     def evaluate_ins(self) -> global___ServerMessage.EvaluateIns: ...
     @property
     def server_received_signal(self) -> global___ServerMessage.ServerReceivedSignal: ...
     @property
     def server_status(self) -> global___ServerMessage.ServerStatus: ...
+    @property
+    def chain_proceeding_signal(self) -> global___ServerMessage.ChainProceedingSignal: ...
+    @property
+    def reservation_success(self) -> global___ServerMessage.ReservationSuccess: ...
+    @property
+    def reservation_failure(self) -> global___ServerMessage.ReservationFailure: ...
     def __init__(self,
         *,
         reconnect_ins: typing.Optional[global___ServerMessage.ReconnectIns] = ...,
         get_properties_ins: typing.Optional[global___ServerMessage.GetPropertiesIns] = ...,
         get_parameters_ins: typing.Optional[global___ServerMessage.GetParametersIns] = ...,
         fit_ins: typing.Optional[global___ServerMessage.FitIns] = ...,
         evaluate_ins: typing.Optional[global___ServerMessage.EvaluateIns] = ...,
         server_received_signal: typing.Optional[global___ServerMessage.ServerReceivedSignal] = ...,
         server_status: typing.Optional[global___ServerMessage.ServerStatus] = ...,
+        chain_proceeding_signal: typing.Optional[global___ServerMessage.ChainProceedingSignal] = ...,
+        reservation_success: typing.Optional[global___ServerMessage.ReservationSuccess] = ...,
+        reservation_failure: typing.Optional[global___ServerMessage.ReservationFailure] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins","server_received_signal",b"server_received_signal","server_status",b"server_status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins","server_received_signal",b"server_received_signal","server_status",b"server_status"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["reconnect_ins","get_properties_ins","get_parameters_ins","fit_ins","evaluate_ins","server_received_signal","server_status"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["chain_proceeding_signal",b"chain_proceeding_signal","evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins","reservation_failure",b"reservation_failure","reservation_success",b"reservation_success","server_received_signal",b"server_received_signal","server_status",b"server_status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["chain_proceeding_signal",b"chain_proceeding_signal","evaluate_ins",b"evaluate_ins","fit_ins",b"fit_ins","get_parameters_ins",b"get_parameters_ins","get_properties_ins",b"get_properties_ins","msg",b"msg","reconnect_ins",b"reconnect_ins","reservation_failure",b"reservation_failure","reservation_success",b"reservation_success","server_received_signal",b"server_received_signal","server_status",b"server_status"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["reconnect_ins","get_properties_ins","get_parameters_ins","fit_ins","evaluate_ins","server_received_signal","server_status","chain_proceeding_signal","reservation_success","reservation_failure"]]: ...
 global___ServerMessage = ServerMessage
 
 class ClientMessage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     class DisconnectRes(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
         REASON_FIELD_NUMBER: builtins.int
@@ -520,22 +564,81 @@
         def __init__(self,
             *,
             status: typing.Optional[global___Status] = ...,
             ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["status",b"status"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
 
+    class ModelSyncRequest(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        PARAMETERS_FIELD_NUMBER: builtins.int
+        CONFIG_FIELD_NUMBER: builtins.int
+        @property
+        def parameters(self) -> global___Parameters: ...
+        @property
+        def config(self) -> global___InnerMap: ...
+        def __init__(self,
+            *,
+            parameters: typing.Optional[global___Parameters] = ...,
+            config: typing.Optional[global___InnerMap] = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["config",b"config","parameters",b"parameters"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["config",b"config","parameters",b"parameters"]) -> None: ...
+
+    class Shutdown(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        STATUS_FIELD_NUMBER: builtins.int
+        @property
+        def status(self) -> global___Status: ...
+        def __init__(self,
+            *,
+            status: typing.Optional[global___Status] = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["status",b"status"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["status",b"status"]) -> None: ...
+
+    class ChainTransferSignal(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        TRANSFER_TO_FIELD_NUMBER: builtins.int
+        CONFIG_FIELD_NUMBER: builtins.int
+        transfer_to: typing.Text
+        @property
+        def config(self) -> global___InnerMap: ...
+        def __init__(self,
+            *,
+            transfer_to: typing.Text = ...,
+            config: typing.Optional[global___InnerMap] = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["config",b"config"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["config",b"config","transfer_to",b"transfer_to"]) -> None: ...
+
+    class ModelTransferReservation(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        CONFIG_FIELD_NUMBER: builtins.int
+        @property
+        def config(self) -> global___InnerMap: ...
+        def __init__(self,
+            *,
+            config: typing.Optional[global___InnerMap] = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["config",b"config"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["config",b"config"]) -> None: ...
+
     DISCONNECT_RES_FIELD_NUMBER: builtins.int
     GET_PROPERTIES_RES_FIELD_NUMBER: builtins.int
     GET_PARAMETERS_RES_FIELD_NUMBER: builtins.int
     FIT_RES_FIELD_NUMBER: builtins.int
     EVALUATE_RES_FIELD_NUMBER: builtins.int
     CLIENT_STATUS_FIELD_NUMBER: builtins.int
     CLIENT_UPLOADING_SIGNAL_FIELD_NUMBER: builtins.int
     CLIENT_ROAMING_SIGNAL_FIELD_NUMBER: builtins.int
+    MODEL_SYNC_REQUEST_FIELD_NUMBER: builtins.int
+    SHUTDOWN_FIELD_NUMBER: builtins.int
+    CHAIN_TRANSFER_SIGNAL_FIELD_NUMBER: builtins.int
+    MODEL_TRANSFER_RESERVATION_FIELD_NUMBER: builtins.int
     @property
     def disconnect_res(self) -> global___ClientMessage.DisconnectRes: ...
     @property
     def get_properties_res(self) -> global___ClientMessage.GetPropertiesRes: ...
     @property
     def get_parameters_res(self) -> global___ClientMessage.GetParametersRes: ...
     @property
@@ -544,22 +647,34 @@
     def evaluate_res(self) -> global___ClientMessage.EvaluateRes: ...
     @property
     def client_status(self) -> global___ClientMessage.ClientStatus: ...
     @property
     def client_uploading_signal(self) -> global___ClientMessage.ClientUploadingSignal: ...
     @property
     def client_roaming_signal(self) -> global___ClientMessage.ClientRoamingSignal: ...
+    @property
+    def model_sync_request(self) -> global___ClientMessage.ModelSyncRequest: ...
+    @property
+    def shutdown(self) -> global___ClientMessage.Shutdown: ...
+    @property
+    def chain_transfer_signal(self) -> global___ClientMessage.ChainTransferSignal: ...
+    @property
+    def model_transfer_reservation(self) -> global___ClientMessage.ModelTransferReservation: ...
     def __init__(self,
         *,
         disconnect_res: typing.Optional[global___ClientMessage.DisconnectRes] = ...,
         get_properties_res: typing.Optional[global___ClientMessage.GetPropertiesRes] = ...,
         get_parameters_res: typing.Optional[global___ClientMessage.GetParametersRes] = ...,
         fit_res: typing.Optional[global___ClientMessage.FitRes] = ...,
         evaluate_res: typing.Optional[global___ClientMessage.EvaluateRes] = ...,
         client_status: typing.Optional[global___ClientMessage.ClientStatus] = ...,
         client_uploading_signal: typing.Optional[global___ClientMessage.ClientUploadingSignal] = ...,
         client_roaming_signal: typing.Optional[global___ClientMessage.ClientRoamingSignal] = ...,
+        model_sync_request: typing.Optional[global___ClientMessage.ModelSyncRequest] = ...,
+        shutdown: typing.Optional[global___ClientMessage.Shutdown] = ...,
+        chain_transfer_signal: typing.Optional[global___ClientMessage.ChainTransferSignal] = ...,
+        model_transfer_reservation: typing.Optional[global___ClientMessage.ModelTransferReservation] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["client_roaming_signal",b"client_roaming_signal","client_status",b"client_status","client_uploading_signal",b"client_uploading_signal","disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_roaming_signal",b"client_roaming_signal","client_status",b"client_status","client_uploading_signal",b"client_uploading_signal","disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","msg",b"msg"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["disconnect_res","get_properties_res","get_parameters_res","fit_res","evaluate_res","client_status","client_uploading_signal","client_roaming_signal"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["chain_transfer_signal",b"chain_transfer_signal","client_roaming_signal",b"client_roaming_signal","client_status",b"client_status","client_uploading_signal",b"client_uploading_signal","disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","model_sync_request",b"model_sync_request","model_transfer_reservation",b"model_transfer_reservation","msg",b"msg","shutdown",b"shutdown"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["chain_transfer_signal",b"chain_transfer_signal","client_roaming_signal",b"client_roaming_signal","client_status",b"client_status","client_uploading_signal",b"client_uploading_signal","disconnect_res",b"disconnect_res","evaluate_res",b"evaluate_res","fit_res",b"fit_res","get_parameters_res",b"get_parameters_res","get_properties_res",b"get_properties_res","model_sync_request",b"model_sync_request","model_transfer_reservation",b"model_transfer_reservation","msg",b"msg","shutdown",b"shutdown"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["msg",b"msg"]) -> typing.Optional[typing_extensions.Literal["disconnect_res","get_properties_res","get_parameters_res","fit_res","evaluate_res","client_status","client_uploading_signal","client_roaming_signal","model_sync_request","shutdown","chain_transfer_signal","model_transfer_reservation"]]: ...
 global___ClientMessage = ClientMessage
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/proto/transport_pb2_grpc.py` & `daisyfl-0.5.3/src/py/daisyfl/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/proto/transport_pb2_grpc.pyi` & `daisyfl-0.5.3/src/py/daisyfl/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/simulation/ray_transport/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,23 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower server."""
-
-
-from .app import start_server as start_server
-from .client_manager import ClientManager as ClientManager
-from .client_manager import SimpleClientManager as SimpleClientManager
-from .history import History as History
-from .server import Server as Server
-
-__all__ = [
-    "ClientManager",
-    "History",
-    "Server",
-    "SimpleClientManager",
-    "start_server",
-]
+"""Ray-based Flower ClientProxy implementation."""
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/app.py` & `daisyfl-0.5.3/src/py/daisyfl/master/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,131 +18,110 @@
 
 from daisyfl.common.logger import log
 from daisyfl.common import (
     Type,
     GRPC_MAX_MESSAGE_LENGTH,
 )
 from daisyfl.proto.transport_pb2_grpc import add_FlowerServiceServicer_to_server
-from daisyfl.server.client_manager import ClientManager, SimpleClientManager
-from daisyfl.server.grpc_server.flower_service_servicer import FlowerServiceServicer
-from daisyfl.server.grpc_server.grpc_server import (
+from daisyfl.utils.client_manager import SimpleClientManager
+from daisyfl.master.grpc_server.grpc_server import (
     generic_create_grpc_server,
     start_grpc_server,
 )
-from daisyfl.server.history import History
-from daisyfl.server.server import Server
-from daisyfl.server.server_operator_manager import ServerOperatorManager
-from daisyfl.server.task_manager import TaskManager
-from daisyfl.server.server_api_handler import ServerListener
-from daisyfl.client.zone_client import ZoneClient
+from daisyfl.utils.server import Server
+from daisyfl.utils.server_operator_manager import ServerOperatorManager
+from daisyfl.utils.task_manager import TaskManager
+from daisyfl.master.server_api_handler import ServerListener
 
 import threading
 import time
 
 DEFAULT_SERVER_ADDRESS = "[::]:8887"
 _cnd_stop: threading.Condition = threading.Condition()
+def shutdown():
+    with _cnd_stop:
+        _cnd_stop.notify()
 
-def start_server(  # pylint: disable=too-many-arguments
+def start_master(  # pylint: disable=too-many-arguments
     *,
-    # task manager
-    zone: bool = False,
-    parent_address: str = "",
     # server
     server_address: str = DEFAULT_SERVER_ADDRESS,
     # api_handler
     api_ip: str = None,
     api_port: int = None,
     # grpc
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     certificates: Optional[Tuple[bytes, bytes, bytes]] = None,
 ) -> None:
     # Initialize server and task manager
     initialized_server: Server = _init_defaults(
-        zone=zone,
-        parent_address=parent_address,
+        server_address=server_address,
         api_ip=api_ip,
         api_port=api_port,
     )
-    log(INFO, "Starting Flower server",)
+    log(INFO, "Starting Master server",)
 
     # Start gRPC server
     grpc_server = start_grpc_server(
         client_manager=initialized_server.get_client_manager(),
         server_address=server_address,
         max_message_length=grpc_max_message_length,
         certificates=certificates,
+        chain_transfer_fn=initialized_server.chain_transfer_fn,
+        model_sync_fn=initialized_server.server_sync_fn,
+        shutdown_fn=shutdown,
     )
     log(
         INFO,
-        "Flower ECE: gRPC server running , SSL is %s",
+        "Master gRPC server running , SSL is %s",
         "enabled" if certificates is not None else "disabled",
     )
 
     # Wait until shutdown
     with _cnd_stop:
         _cnd_stop.wait()
     # Stop the gRPC server
     grpc_server.stop(grace=1)
     initialized_server.get_client_manager().unregister_all()
-    log(INFO, "Daisy server shutdown")
+    log(INFO, "Master server shutdown")
     exit(0)
 
 
 def _init_defaults(
-    zone: bool,
-    parent_address: Optional[str],
+    server_address: str,
     api_ip: str = None,
     api_port: int = None,
-) -> Tuple[Server, TaskManager]:
+) -> Server:
     # client_manager
     client_manager = SimpleClientManager()       
     # server
-    server = Server(client_manager=client_manager)
+    server = Server(client_manager=client_manager, server_address=server_address,)
     # server_operator_manager
     server_operator_manager = ServerOperatorManager(server=server)
-    # zone or master
-    manager_type = Type.ZONE if zone else Type.MASTER
     # task_manager
     task_manager = TaskManager(
         server_operator_manager=server_operator_manager,
-        manager_type=manager_type,
+        manager_type=Type.MASTER,
     )
-    # for master: start ServerListener
-    if manager_type == Type.MASTER:
-        start_server_listener(api_ip=api_ip, api_port=api_port, task_manager=task_manager)
-    # for zone: start ZoneClient
-    elif manager_type == Type.ZONE:
-        start_zone_client(parent_address, api_ip, api_port, task_manager)
-    else:
-        log(ERROR, "Use undefined node type.")
-        exit(1)
+    # start ServerListener
+    start_server_listener(api_ip=api_ip, api_port=api_port, task_manager=task_manager)
     
     return server
 
 # server_listener
 def start_server_listener(api_ip: str, api_port: int, task_manager: TaskManager) -> bool:
     if isinstance(api_ip, str) and isinstance(api_port, int):
-        listener = ServerListener(api_ip, api_port, task_manager, _cnd_stop)
+        listener = ServerListener(api_ip, api_port, task_manager,)
         listener_thread = threading.Thread(target=listener.run, args=())
         listener_thread.setDaemon(True)
         listener_thread.start()
         time.sleep(1)
         if not listener_thread.is_alive():
             log(ERROR, "ServerListner failed")
             exit(1)
     else:
         log(
             ERROR,
             "Please check api_ip is string and api_port is integer.",
         )
         exit(1)
     return True
-
-# zone_client
-def start_zone_client(parent_address: str,  api_ip: str, api_port: int, task_manager: TaskManager):
-    zc = threading.Thread(target=ZoneClient, args=(parent_address, api_ip, api_port, task_manager, _cnd_stop))
-    zc.setDaemon(True)
-    zc.start()
-    threading.Event().wait(timeout=1)
-    if not zc.is_alive():
-        log(ERROR, "ZoneClient failed")
-        exit(1)
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/client_manager.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/client_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from abc import ABC, abstractmethod
 from logging import INFO
 from typing import Dict, List, Optional, Callable
 
 from daisyfl.common.logger import log
 from daisyfl.common import CREDENTIAL, IS_ZONE
 
-from .client_proxy import ClientProxy
-from .criterion import Criterion
+from daisyfl.utils.client_proxy import ClientProxy
+from daisyfl.utils.criterion import Criterion
 import time
 
 class ClientManager(ABC):
     """Abstract base class for managing Flower clients."""
 
     @abstractmethod
     def num_available(self) -> int:
@@ -167,19 +167,20 @@
         client.set_check_waiting_fn(self.check_waiting)
         client.set_client_fail_fn(self.client_fail)
         client.set_client_roam_fn(self.client_roam)
         # register a zone
         if is_zone:
             self.zones[client.cid] = client
         else:
+            # TODO: record credential at client_proxy
             credential = client.metadata_dict[CREDENTIAL]
             if not self.clients.__contains__(credential):
                 self.clients[credential] = {}
             self.clients[credential][client.cid] = client
-        
+            client.credential = credential
         with self._cv:
             self._cv.notify_all()
 
         return True
 
     def unregister(self, client: ClientProxy) -> None:
         """Unregister Flower ClientProxy instance.
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/client_proxy.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/client_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import Optional, Union, Callable
 
 from daisyfl.common import (
     DisconnectRes,
     EvaluateIns,
     EvaluateRes,
     FitIns,
+    ChainProceedingSignal,
     FitRes,
     GetParametersIns,
     GetParametersRes,
     GetPropertiesIns,
     GetPropertiesRes,
     Properties,
     ReconnectIns,
@@ -54,15 +55,15 @@
         ins: GetParametersIns,
     ) -> None:
         """Return the current local model parameters."""
 
     @abstractmethod
     def fit(
         self,
-        ins: FitIns,
+        ins: Union[FitIns, ChainProceedingSignal],
     ) -> None:
         """Refine the provided parameters using the locally held dataset."""
 
     @abstractmethod
     def evaluate(
         self,
         ins: EvaluateIns,
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/criterion.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,21 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Abstract class for criterion sampling."""
+"""Contains server side utilities to be used in combination with various
+components."""
 
 
-from abc import ABC, abstractmethod
+from .dynamic_loader import dynamic_load as dynamic_load
 
-from .client_proxy import ClientProxy
 
-
-class Criterion(ABC):
-    """Abstract class which allows subclasses to implement criterion sampling."""
-
-    @abstractmethod
-    def select(self, client: ClientProxy) -> bool:
-        """Decide whether a client should be eligible for sampling or not."""
+__all__ = [
+    "dynamic_load",
+]
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/client/grpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/flower_service_servicer.py` & `daisyfl-0.5.3/src/py/daisyfl/zone/grpc_server/zone_service_servicer.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 from typing import Callable, Iterator, Any, Dict, Tuple, Optional
 import timeit
 import grpc
 from iterators import TimeoutIterator
 
 from daisyfl.proto import transport_pb2_grpc
 from daisyfl.proto.transport_pb2 import ClientMessage, ServerMessage
-from daisyfl.server.client_manager import ClientManager
-from daisyfl.server.grpc_server.grpc_bridge import GRPCBridge
-from daisyfl.server.grpc_server.grpc_client_proxy import GrpcClientProxy
+from daisyfl.utils.client_manager import ClientManager
+from daisyfl.utils.grpc_bridge import GRPCBridge
+from daisyfl.utils.connection import grpc_connection
+from daisyfl.utils.grpc_client_proxy import GrpcClientProxy
 from daisyfl.common.logger import log
 from logging import INFO, WARNING, DEBUG, ERROR
 from daisyfl.common import (
     HANDOVER,
     ROOT_CERTIFICATES,
     ANCHOR,
     GRPC_MAX_MESSAGE_LENGTH,
@@ -49,19 +50,20 @@
     CID,
     Code,
     ServerReceivedSignal,
     ClientRoamingSignal,
     Status,
     FitRes,
     Parameters,
+    ModelSyncMessage,
+    ChainTransferSignal,
 )
 from daisyfl.proto.transport_pb2_grpc import FlowerServiceStub
 from threading import Condition, Event
-from enum import Enum
-from queue import Queue
+
 
 def default_bridge_factory(client_idling: bool) -> GRPCBridge:
     """Return GRPCBridge instance."""
     return GRPCBridge(client_idling)
 
 
 def default_grpc_client_factory(bridge: GRPCBridge, metadata_dict: Dict) -> GrpcClientProxy:
@@ -84,41 +86,30 @@
             client.bridge.close()
             client_manager.unregister(client)
 
         context.add_callback(rpc_termination_callback)
 
     return is_success
 
-
-def on_channel_state_change(channel_connectivity: str) -> None:
-    """Log channel connectivity."""
-    log(DEBUG, channel_connectivity)
-
-class FlowerServiceServicer(transport_pb2_grpc.FlowerServiceServicer):
-    """FlowerServiceServicer for bi-directional gRPC message stream."""
+class ZoneServiceServicer(transport_pb2_grpc.FlowerServiceServicer):
+    """ZoneServiceServicer for bi-directional gRPC message stream."""
 
     def __init__(
         self,
         client_manager: ClientManager,
         server_address: str,
         grpc_bridge_factory: Callable[[bool], GRPCBridge] = default_bridge_factory,
         grpc_client_factory: Callable[
             [GRPCBridge, Dict], GrpcClientProxy
         ] = default_grpc_client_factory,
     ) -> None:
         self.client_manager: ClientManager = client_manager
         self.server_address: str = server_address
         self.grpc_bridge_factory = grpc_bridge_factory
         self.client_factory = grpc_client_factory
-        # sentinel
-        self.sentinel = ClientMessage(fit_res=serde.fit_res_to_proto(FitRes(
-            status=Status(code=Code.OK, message="Success"),
-            parameters=Parameters(tensors=[], tensor_type=""),
-            config={},
-        )))
 
     def Join(  # pylint: disable=invalid-name
         self,
         request_iterator: Iterator[ClientMessage],
         context: grpc.ServicerContext,
     ) -> Iterator[ServerMessage]:
         """Method will be invoked by each GrpcClientProxy which participates in
@@ -138,74 +129,42 @@
             # check handover
             metadata_dict = metadata_to_dict(context.invocation_metadata(), _check_reserved=False)
             if metadata_dict.__contains__(HANDOVER):
                 yield from self.roaming_request(client_timeout_iterator=client_timeout_iterator, context=context)
             else:
                 client_status: ClientStatus = serde.client_status_from_proto(client_message.client_status)
                 yield from self.serve(client_timeout_iterator=client_timeout_iterator, context=context, client_status=client_status)
+        elif field == "model_sync_request":
+                model_sync_message: ModelSyncMessage = serde.model_sync_request_from_proto(client_message.model_sync_request)
+                yield from self.model_sync(model_sync_message=model_sync_message)
         elif field == "client_roaming_signal":
             # get roaming information from Anchor
             log(INFO, "Receive CRS")
             yield from self.roaming_info_request(client_timeout_iterator=client_timeout_iterator, context=context,)
+        elif field == "shutdown":
+            self.shutdown()
+            return
         else:
             log(ERROR, "Receive unexpected message type.")
             return
-
-    @contextmanager
-    def grpc_connection(
-        self,
-        parent_address: str,
-        metadata: Tuple,
-        root_certificates: Optional[bytes] = None,
-    ) -> Iterator[Tuple[Callable[[], ServerMessage], Callable[[ClientMessage], None]]]:
-        # Possible options:
-        # https://github.com/grpc/grpc/blob/v1.43.x/include/grpc/impl/codegen/grpc_types.h
-        channel_options = [
-            ("grpc.max_send_message_length", GRPC_MAX_MESSAGE_LENGTH),
-            ("grpc.max_receive_message_length", GRPC_MAX_MESSAGE_LENGTH),
-        ]
-
-        if root_certificates is not None:
-            ssl_channel_credentials = grpc.ssl_channel_credentials(root_certificates)
-            channel = grpc.secure_channel(
-                parent_address, ssl_channel_credentials, options=channel_options
-            )
-            log(INFO, "Opened secure gRPC connection using certificates")
-        else:
-            channel = grpc.insecure_channel(parent_address, options=channel_options)
-            log(INFO, "Opened insecure gRPC connection (no certificates were passed)")
-
-        channel.subscribe(on_channel_state_change)
-        
-        stub = FlowerServiceStub(channel)
-        queue: Queue[ClientMessage] = Queue(maxsize=1)
-        time_iterator = TimeoutIterator(iterator=iter(queue.get, None), reset_on_next=True)
-
-        server_message_iterator: Iterator[ServerMessage] = stub.Join(time_iterator, metadata=metadata)
-        timeout_iterator = TimeoutIterator(iterator=server_message_iterator, reset_on_next=True)
-
-        def receive_fn(timeout: Optional[int] = None) -> Tuple[ServerMessage, bool]:
-            if timeout is not None:
-                timeout_iterator.set_timeout(float(timeout))
-            server_message = next(timeout_iterator)
-            if server_message is timeout_iterator.get_sentinel():
-                return server_message, False
-            return server_message, True
-        receive: Callable[[Optional[int]], Tuple[ServerMessage, bool]] = receive_fn
-        send: Callable[[ClientMessage], None] = lambda msg: queue.put(msg, block=False)
-
+    
+    # process different message types
+    def model_sync(self, model_sync_message: ModelSyncMessage):
         try:
-            yield send, receive
-        finally:
-            # Release Iterator to avoid leaking memory
-            time_iterator.interrupt()
-            send(self.sentinel)
-            # Make sure to have a final
-            channel.close()
-            log(DEBUG, "gRPC channel closed")
+            # set edge model
+            self.model_sync_fn(model_sync_message)
+            log(DEBUG, "set ModelSyncMessage")
+            # send SRS
+            srs = ServerReceivedSignal(status=Status(code=Code.OK, message=""))
+            server_message = ServerMessage(server_received_signal=serde.server_received_signal_to_proto(srs))
+            yield server_message
+            log(DEBUG, "Send SRS")
+            return
+        except StopIteration:
+            return
 
     def roaming_request(
         self,
         client_timeout_iterator: Iterator[ClientMessage],
         context: grpc.ServicerContext,
     ) -> Iterator[ServerMessage]:
         """Get roaming information from anchor."""
@@ -235,15 +194,15 @@
                 return
             field = client_message.WhichOneof("msg")
             if field != "client_uploading_signal":
                 return
             log(DEBUG, "Receive CUS")
             
             # connect to anchor
-            with self.grpc_connection(
+            with grpc_connection(
                 parent_address=parent_address,
                 metadata=dict_to_metadata(metadata_dict),
                 root_certificates=root_certificates
             ) as conn:
                 send, receive = conn
                 ## send CRS to anchor
                 crs = ClientRoamingSignal(status=Status(code=Code.OK, message=""))
@@ -376,27 +335,32 @@
                     server_status = serde.server_status_to_proto(ServerStatus(status=SERVER_WAITING))
                 server_status_msg = ServerMessage(server_status=server_status)
                 yield server_status_msg
                 log(DEBUG, "Send ServerStatus")
                 # get the result
                 client_message, success = self.get_client_message(client_message_iterator=client_timeout_iterator, context=context, timeout=None)
                 if success:
-                    if server_waiting:
+                    if client_message.WhichOneof("msg") == "chain_transfer_signal":
+                        cts: ChainTransferSignal = serde.chain_transfer_signal_from_proto(client_message.chain_transfer_signal)
+                        self.chain_transfer_fn(client_proxy.cid, client_proxy.credential, cts)
+                        log(DEBUG, "set CTS")
+                    elif server_waiting:
                         client_proxy.bridge.set_client_message(client_message=client_message)
                         log(DEBUG, "Set ClientMessage")
                     srs = ServerReceivedSignal(status=Status(code=Code.OK, message=""))
                     server_message = ServerMessage(server_received_signal=serde.server_received_signal_to_proto(srs))
                     yield server_message
                     log(DEBUG, "Send SRS")
                     client_idling = True
-                    Event.wait(timeout=5)
+                    Event().wait(timeout=5)
             except StopIteration:
                 return
         # return
 
+    # communication
     def get_server_message(self, client_proxy: GrpcClientProxy,) -> Iterator[ServerMessage]:
         log(DEBUG, "Try sending ServerMessage")
         _server_message_iterator = client_proxy.bridge.server_message_iterator()
         # Get server_message from bridge
         server_message: ServerMessage = next(_server_message_iterator)
         yield server_message
 
@@ -421,9 +385,23 @@
             # that client_message in subsequent lines is not None
             # It does not understand that `context.abort` will terminate
             # this execution context by raising an exception.
             return client_message, False
 
         return client_message, True
 
-
-# TODO: FlowerService -> DaisyService
+    # shutdown
+    def set_shutdown_fn(self, shutdown_fn: Callable):
+        self.shutdown_fn: Callable = shutdown_fn
+
+    def shutdown(self,):
+        self.shutdown_fn()
+        return
+
+    # model synchronization
+    def set_model_sync_fn(self, model_sync_fn: Callable):
+        self.model_sync_fn: Callable = model_sync_fn
+
+    # chain transfer
+    def set_chain_transfer_fn(self, chain_transfer_fn: Callable):
+        self.chain_transfer_fn: Callable = chain_transfer_fn
+
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/grpc_bridge.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/grpc_client_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 """gRPC-based Flower ClientProxy implementation."""
 
 from typing import Optional, Dict, Union, Callable
 
 from daisyfl import common
 from daisyfl.common import serde
 from daisyfl.proto.transport_pb2 import ClientMessage, ServerMessage
-from daisyfl.server.client_proxy import ClientProxy
-from daisyfl.server.grpc_server.grpc_bridge import GRPCBridge
+from daisyfl.utils.client_proxy import ClientProxy
+from daisyfl.utils.grpc_bridge import GRPCBridge
 from daisyfl.common.logger import log
 from logging import WARNING, INFO, ERROR
 
 class GrpcClientProxy(ClientProxy):
     """Flower client proxy which delegates over the network using gRPC."""
 
     def __init__(
@@ -57,21 +57,24 @@
         get_parameters_msg = serde.get_parameters_ins_to_proto(ins)
         self.bridge.request(
             ServerMessage(get_parameters_ins=get_parameters_msg),
         )
 
     def fit(
         self,
-        ins: common.FitIns,
+        ins: Union[common.FitIns, common.ChainProceedingSignal],
     ) -> None:
         """Refine the provided parameters using the locally held dataset."""
-        fit_ins_msg = serde.fit_ins_to_proto(ins)
-        self.bridge.request(
-            ServerMessage(fit_ins=fit_ins_msg),
-        )
+        if isinstance(ins, common.FitIns):
+            ins_msg = serde.fit_ins_to_proto(ins)
+            sm = ServerMessage(fit_ins=ins_msg)
+        elif isinstance(ins, common.ChainProceedingSignal):
+            ins_msg = serde.chain_proceeding_signal_to_proto(ins)
+            sm = ServerMessage(chain_proceeding_signal=ins_msg)
+        self.bridge.request(sm)
 
     def evaluate(
         self,
         ins: common.EvaluateIns,
     ) -> None:
         """Evaluate the provided parameters using the locally held dataset."""
         evaluate_msg = serde.evaluate_ins_to_proto(ins)
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/grpc_server/grpc_server.py` & `daisyfl-0.5.3/src/py/daisyfl/master/grpc_server/grpc_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 from typing import Any, Callable, Optional, Tuple, Union
 
 import grpc
 
 from daisyfl.common import GRPC_MAX_MESSAGE_LENGTH
 from daisyfl.common.logger import log
 from daisyfl.proto.transport_pb2_grpc import add_FlowerServiceServicer_to_server
-from daisyfl.server.client_manager import ClientManager
-from daisyfl.server.grpc_server.flower_service_servicer import FlowerServiceServicer
+from daisyfl.utils.client_manager import ClientManager
+from daisyfl.master.grpc_server.master_service_servicer import MasterServiceServicer
 
 INVALID_CERTIFICATES_ERR_MSG = """
     When setting any of root_certificate, certificate, or private_key,
     all of them need to be set.
 """
 
 AddServicerToServerFn = Callable[..., Any]
@@ -52,14 +52,17 @@
 def start_grpc_server(  # pylint: disable=too-many-arguments
     client_manager: ClientManager,
     server_address: str,
     max_concurrent_workers: int = 1000,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     keepalive_time_ms: int = 210000,
     certificates: Optional[Tuple[bytes, bytes, bytes]] = None,
+    chain_transfer_fn: Callable = None,
+    model_sync_fn: Callable = None,
+    shutdown_fn: Callable = None,
 ) -> grpc.Server:
     """Create and start a gRPC server running FlowerServiceServicer.
 
     If used in a main function server.wait_for_termination(timeout=None)
     should be called as otherwise the server will immediately stop.
 
     **SSL**
@@ -125,15 +128,21 @@
     >>>         Path("/crts/root.pem").read_bytes(),
     >>>         Path("/crts/localhost.crt").read_bytes(),
     >>>         Path("/crts/localhost.key").read_bytes(),
     >>>     ),
     >>> )
     """
 
-    servicer = FlowerServiceServicer(client_manager, server_address)
+    servicer = MasterServiceServicer(client_manager, server_address)
+    if chain_transfer_fn is not None:
+        servicer.set_chain_transfer_fn(chain_transfer_fn)
+    if model_sync_fn is not None:
+        servicer.set_model_sync_fn(model_sync_fn)
+    if shutdown_fn is not None:
+        servicer.set_shutdown_fn(shutdown_fn)
     add_servicer_to_server_fn = add_FlowerServiceServicer_to_server
 
     server = generic_create_grpc_server(
         servicer_and_add_fn=(servicer, add_servicer_to_server_fn),
         server_address=server_address,
         max_concurrent_workers=max_concurrent_workers,
         max_message_length=max_message_length,
@@ -143,15 +152,15 @@
 
     server.start()
 
     return server
 
 
 def generic_create_grpc_server(  # pylint: disable=too-many-arguments
-    servicer_and_add_fn: Tuple[FlowerServiceServicer, AddServicerToServerFn],
+    servicer_and_add_fn: Tuple[MasterServiceServicer, AddServicerToServerFn],
     server_address: str,
     max_concurrent_workers: int = 1000,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     keepalive_time_ms: int = 210000,
     certificates: Optional[Tuple[bytes, bytes, bytes]] = None,
 ) -> grpc.Server:
     """Generic function to create a gRPC server with a single servicer.
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/history.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/history.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/server.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Flower server."""
 
 
 import concurrent.futures
 import timeit
 from threading import Event, Condition, Lock, Timer, Thread
 from queue import Queue
-from logging import DEBUG, INFO
+from logging import DEBUG, INFO, WARNING, ERROR
 from typing import Dict, List, Optional, Tuple, Union, Callable
 import gc
 from daisyfl.common import (
     Task,
     Report,
     CURRENT_ROUND,
     EVALUATE,
@@ -42,45 +42,60 @@
     ReconnectIns,
     Scalar,
     CurrentReturns,
     TID,
     CID,
     ROAMING_TIMEOUT,
     IS_ROAMER,
+    CREDENTIAL,
+    ModelSyncMessage,
+    serde,
+    ChainTransferSignal,
+    ChainProceedingSignal,
 )
 from daisyfl.common.logger import log
 from daisyfl.common.typing import GetParametersIns
-from daisyfl.server.client_manager import ClientManager
-from daisyfl.server.client_proxy import ClientProxy
-from daisyfl.server.history import History
-from daisyfl.server.criterion import Criterion
+from daisyfl.utils.client_manager import ClientManager
+from daisyfl.utils.client_proxy import ClientProxy
+from daisyfl.utils.criterion import Criterion
+from daisyfl.utils.model_sync import send_model
 
 FitResultsAndFailures = Tuple[
     List[Tuple[ClientProxy, FitRes]],
     List[Union[Tuple[ClientProxy, FitRes], BaseException]],
 ]
 EvaluateResultsAndFailures = Tuple[
     List[Tuple[ClientProxy, EvaluateRes]],
     List[Union[Tuple[ClientProxy, EvaluateRes], BaseException]],
 ]
 ReconnectResultsAndFailures = Tuple[
     List[Tuple[ClientProxy, DisconnectRes]],
     List[Union[Tuple[ClientProxy, DisconnectRes], BaseException]],
 ]
 
+class Find(Criterion):
+    def __init__(self, cid: str):
+        self.cid = cid
+
+    def select(self, client: ClientProxy) -> bool:
+        if client.cid == self.cid:
+            return True
+        return False
 
 class SubtaskManager:
     def __init__(self,) -> None:
         self.subtasks: Dict[int, CurrentReturns] = {}
         self.queues: Dict[int, Queue] = {}
         self.roaming_queues_fit: Dict[str, Queue[FitRes, int, float]] = {} # {"tid": Queue[res, timeout, time_stamp]}
         self.roaming_queues_evaluate: Dict[str, Queue[EvaluateRes, int, float]] = {} # {"tid": Queue[res, timeout, time_stamp]}
         self.client_previous_subtask: Dict[str, int] = {}
         self.timeouts: Dict[int, List] = {} # [TIMEOUT, start_time] 
+        self.edge_model_buf: Dict[str, List(ModelSyncMessage)] = {}
         self._generator_lock: Lock = Lock()
+        self._server_sync_lock: Lock = Lock()
         self._roaming_lock: Lock = Lock()
         self._subtask_num = 0
         self.scheduler = Thread(target=self.check_timeout, args=())
         self.scheduler.setDaemon(True)
         self.scheduler.start()
     
     def subtask_id_generator(self,) -> int:
@@ -225,14 +240,39 @@
             return
         self.subtasks[subtask_id].roaming_num += 1
         del self.client_previous_subtask[cid]
         with self.subtasks[subtask_id].cnd:
             self.subtasks[subtask_id].cnd.notify_all()
         return
     
+    def chain_transfer_fn(self, cid: str, cts: ChainTransferSignal) -> None:
+        subtask_id = self.client_previous_subtask[cid]
+        del self.client_previous_subtask[cid]
+        self.client_previous_subtask[cts.transfer_to] = subtask_id
+        return
+
+    def server_sync_fn(self, server_sync_message: ModelSyncMessage) -> bool:
+        with self._server_sync_lock:
+            if not server_sync_message.config.__contains__(TID):
+                log(WARNING, "Ignore an edge model without task ID. Please send it with a key of \"TID\" in the dictionary")
+                return False
+            if not self.edge_model_buf.__contains__(server_sync_message.config[TID]):
+                self.edge_model_buf[server_sync_message.config[TID]] = []
+            self.edge_model_buf[server_sync_message.config[TID]].append(server_sync_message)
+            return True
+    
+    def get_server_sync_message(self, tid: str) -> List[ModelSyncMessage]:
+        with self._server_sync_lock:
+            if not self.edge_model_buf.__contains__(tid):
+                return []
+            else:
+                tmp = self.edge_model_buf[tid]
+                self.edge_model_buf[tid] = []
+                return tmp
+
     def get_current_returns(self, subtask_id: int) -> CurrentReturns:
         return self.subtasks[subtask_id]
     
     def get_results(self, subtask_id: int) -> List[Tuple[ClientProxy, Union[FitRes, EvaluateRes]]]:
         results = []
         q = self.queues[subtask_id]
         for _ in range(q.qsize()):
@@ -257,15 +297,17 @@
 
 
 class Server:
     """Flower server."""
     def __init__(
         self, *, 
         client_manager: ClientManager,
+        server_address: str,
     ) -> None:
+        self.server_address: str = server_address
         self._client_manager: ClientManager = client_manager
         self._max_workers: Optional[int] = None
         self._subtask_manager: SubtaskManager = SubtaskManager()
         self._client_manager.set_submit_subtask_fn(self._subtask_manager.submit_subtask)
         self._client_manager.set_check_waiting_fn(self._subtask_manager.check_waiting)
         self._client_manager.set_client_fail_fn(self._subtask_manager.client_fail)
         self._client_manager.set_client_roam_fn(self._subtask_manager.client_roam)
@@ -330,14 +372,44 @@
     
     def get_results(self, subtask_id: int) -> List[Tuple[ClientProxy, Union[FitRes, EvaluateRes]]]:
         return self._subtask_manager.get_results(subtask_id)
     
     def get_results_roaming(self, tid: str, fit: bool=True) -> List[Tuple[ClientProxy, Union[FitRes, EvaluateRes]]]:
         return self._subtask_manager.get_results_roaming(tid=tid, fit=fit)
 
+    def get_server_sync_message(self, tid: str) -> List[ModelSyncMessage]:
+        return self._subtask_manager.get_server_sync_message(tid=tid)
+
+    def synchronize_edge_model(self, dest: str, model_sync_message: ModelSyncMessage) -> None:
+        if not model_sync_message.config.__contains__(TID):
+            log(WARNING, "Ignore an edge model without task ID. Please send it with a key of \"TID\" in the dictionary")
+            return
+        send_model(dest=dest, model_sync_message=model_sync_message)
+        return
+    
+    def server_sync_fn(self, server_sync_message: ModelSyncMessage):
+        self._subtask_manager.server_sync_fn(server_sync_message)
+        return
+
+    def chain_transfer_fn(self, cid: str, credential: str, cts: ChainTransferSignal):
+        self._subtask_manager.chain_transfer_fn(cid, cts)
+        # TODO: send message
+        cps = ChainProceedingSignal(config=cts.config)
+        criterion = Find(cts.transfer_to)
+        for trials in range(10):
+            clients = self.sample(num_clients=1, min_num_clients=1, credential=credential,criterion=criterion)
+            if len(clients) == 0:
+                # Selection Failure
+                log(WARNING, "Can't find the objective client_proxy.")
+                Event().wait(timeout=3)
+            else:
+                # Selection Success
+                clients[0].fit(cps)
+                return
+
     # TODO:
     def disconnect_all_clients(self,) -> None:
         """Send shutdown signal to all clients."""
         clients = self.get_client_manager().all() 
         instruction = ReconnectIns(seconds=None)
         client_instructions = [(client_proxy, instruction) for client_proxy in clients]
         _ = self._reconnect_clients(
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/server_api_handler.py` & `daisyfl-0.5.3/src/py/daisyfl/master/server_api_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from flask import Flask, request, make_response, Response
 from typing import Callable
-from daisyfl.server.task_manager import TaskManager
+from daisyfl.utils.task_manager import TaskManager
 import threading
 from daisyfl.common import (
     CURRENT_ROUND,
     PARTICIPATION,
     SUBTASK_RETURNS_SELECTED,
     SUBTASK_RETURNS_RESULTS,
     SUBTASK_RETURNS_FAILURES,
@@ -18,30 +18,22 @@
 
 class ServerListener:
     def __init__(
             self,
             ip: str,
             port: int,
             task_manager: TaskManager,
-            cnd_stop: threading.Condition,
         ):
         self.app = Flask(__name__)
         self._ip: str = ip
         self._port: int = port
         self._task_manager: TaskManager = task_manager
-        self._cnd_stop: threading.Condition = cnd_stop
         
-        @self.app.route("/shutdown", methods=["POST"])
-        def shutdown():
-            with self._cnd_stop:
-                self._cnd_stop.notify()
-            return {}, 200
-        
-        @self.app.route("/receive_task", methods=["POST"])
-        def receive_task():
+        @self.app.route("/publish_task", methods=["POST"])
+        def publish_task():
             js = request.get_json()
             self._task_manager.receive_task(task_config=js)
             return js, 200
         
         @self.app.route("/metrics")
         def metrics():
             res = ""
@@ -136,15 +128,15 @@
                             )
                             res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
                                 "loss_class", "loss_class_of_the_individual_clients", "gauge", labels, loss_list[2]
                             )
                         res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
                             "loss_individual", "loss_of_the_individual_clients", "gauge", labels, client_metrics[LOSS]
                         )
-            print(res)
+            # print(res)
             response = make_response(res)
             response.headers["content-type"] = "text/plain"
             return response
 
     def run(self,):
         self.app.run(host=self._ip, port=self._port)
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/server_operator_manager.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/server_operator_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     Task,
     Report,
     TID,
     REMOVE_OPERATOR,
     OPERATORS,
     STRATEGIES,
 )
-from daisyfl.server.server import Server
+from daisyfl.utils.server import Server
 from threading import Lock
+
 @dataclass
 class TaskOperator:
     tid: str
     operator_path: List[str]
     strategy_path: List[str]
     operator: ServerLogic
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/server/task_manager.py` & `daisyfl-0.5.3/src/py/daisyfl/utils/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     EVALUATE_INTERVAL,
     EVALUATE_INIT_MODEL_MASTER,
     REMOVE_OPERATOR,
     OPERATORS,
     MASTER_SERVER_OPERATOR,
     CLIENT_OPERATOR,
     ZONE_SERVER_OPERATOR,
-    ZONE_CLIENT_OPERATOR,
     STRATEGIES,
     MASTER_STRATEGY,
     ZONE_STRATEGY,
     PERIOD,
     PERIOD_MASTER,
     PERIOD_ZONE,
     SUBTASK_RETURNS_SELECTED,
@@ -53,20 +52,18 @@
     INDIVIDUAL_CLIENT_METRICS,
     PARTICIPATION,
     SAVE_MODEL,
     ROAMING_TIMEOUT,
 )
 from daisyfl.common.logger import log
 from daisyfl.common.typing import GetParametersIns
-from daisyfl.server.server_operator_manager import ServerOperatorManager
-from daisyfl.server.history import History
+from daisyfl.utils.server_operator_manager import ServerOperatorManager
+from daisyfl.utils.history import History
 from daisyfl.common import Type
 
-from daisyfl.client import ZoneClient
-import threading
 import numpy as np
 from dataclasses import dataclass
 
 @dataclass
 class MetaTask:
     """local information."""
     tid: str
@@ -126,18 +123,14 @@
 
         # history & report
         log(INFO, "app_fit: losses_distributed %s", str(meta_task.history.losses_distributed))
         log(INFO, "app_fit: metrics_distributed %s", str(meta_task.history.metrics_distributed))
         log(INFO, "app_fit: losses_centralized %s", str(meta_task.history.losses_centralized))
         log(INFO, "app_fit: metrics_centralized %s", str(meta_task.history.metrics_centralized))
         
-
-        # housekeeping
-        if self.type == Type.MASTER and task_config[SAVE_MODEL]:
-            np.save(task_config[MODEL_PATH], np.array(parameters_to_ndarrays(parameters), dtype=object))
         end_time = timeit.default_timer()
         elapsed = end_time - meta_task.start_time
         log(INFO, "FL finished in %s", elapsed)
         # NOTE: keep main task in master to export metrics
         if self.type == Type.ZONE:
             self.task_complete(tid=task_config[TID])
 
@@ -189,17 +182,16 @@
             log(WARNING, "Use default evaluate_init_model_master")
             task_config[EVALUATE_INIT_MODEL_MASTER] = False
 
         if not (task_config.__contains__(OPERATORS)):
             log(WARNING, "No operator was specified. Use base operators.")
             task_config[OPERATORS] = {
 		        MASTER_SERVER_OPERATOR: ["daisyfl.operator.base.server_logic", "ServerLogic"],
-		        CLIENT_OPERATOR: ["daisyfl.operator.base.client_logic", "ClientLogic"],
 		        ZONE_SERVER_OPERATOR: ["daisyfl.operator.base.server_logic", "ServerLogic"],
-		        ZONE_CLIENT_OPERATOR: ["daisyfl.operator.base.client_logic", "ClientLogic"],
+                CLIENT_OPERATOR: ["daisyfl.operator.base.client_logic", "ClientLogic"],
 	        }            
         if not (task_config.__contains__(STRATEGIES)):
             log(WARNING, "No strategy was specified. Use FedAvg.")
             task_config[STRATEGIES] = {
 		        MASTER_STRATEGY: ["daisyfl.operator.strategy", "FedAvg"],
 		        ZONE_STRATEGY: ["daisyfl.operator.strategy", "FedAvg"],
 	        }
@@ -299,14 +291,16 @@
             if self.type == Type.MASTER:
                 meta_task.history.add_loss_distributed(
                     server_round=report.config[CURRENT_ROUND_MASTER], loss=report.config[LOSS]
                 )
                 meta_task.history.add_metrics_distributed(
                     server_round=report.config[CURRENT_ROUND_MASTER], metrics=report.config[METRICS]
                 )
+                if task.config[SAVE_MODEL]:
+                    np.save(task.config[MODEL_PATH], np.array(parameters_to_ndarrays(parameters), dtype=object))
             else:
                 meta_task.history.add_loss_distributed(
                     server_round=report.config[CURRENT_ROUND_ZONE], loss=report.config[LOSS]
                 )
                 meta_task.history.add_metrics_distributed(
                     server_round=report.config[CURRENT_ROUND_ZONE], metrics=report.config[METRICS]
                 )
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/simulation/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.5.2/src/py/daisyfl/simulation/app.py` & `daisyfl-0.5.3/src/py/daisyfl/simulation/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from logging import ERROR, INFO
 from typing import Any, Callable, Dict, List, Optional
 
 import ray
 
 from daisyfl.client.client import Client
 from daisyfl.common.logger import log
-from daisyfl.server import Server
-from daisyfl.server.app import _init_defaults
-from daisyfl.server.client_manager import ClientManager
-from daisyfl.server.history import History
+from daisyfl.utils.server import Server
+from daisyfl.master.app import _init_defaults
+from daisyfl.utils.client_manager import ClientManager
+from daisyfl.utils.history import History
 from daisyfl.simulation.ray_transport.ray_client_proxy import RayClientProxy
 
 INVALID_ARGUMENTS_START_SIMULATION = """
 INVALID ARGUMENTS ERROR
 
 Invalid Arguments in method:
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/simulation/ray_transport/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/master/grpc_server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Ray-based Flower ClientProxy implementation."""
+"""Server-side networking package."""
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py` & `daisyfl-0.5.3/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from typing import Callable, Dict, Optional, cast
 
 import ray
 
 from daisyfl import common
 from daisyfl.client import Client, ClientLike, to_client
-from daisyfl.server.client_proxy import ClientProxy
+from daisyfl.utils.client_proxy import ClientProxy
 
 ClientFn = Callable[[str], ClientLike]
 
 
 class RayClientProxy(ClientProxy):
     """Flower client proxy which delegates work using Ray."""
```

### Comparing `daisyfl-0.5.2/src/py/daisyfl/utils/__init__.py` & `daisyfl-0.5.3/src/py/daisyfl/master/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Contains server side utilities to be used in combination with various
-components."""
+"""Flower server."""
 
 
-from .dynamic_loader import dynamic_load as dynamic_load
-
+from .app import start_master as start_master
 
 __all__ = [
-    "dynamic_load",
+    "start_master",
 ]
```

### Comparing `daisyfl-0.5.2/setup.py` & `daisyfl-0.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,50 +4,53 @@
 package_dir = \
 {'': 'src/py'}
 
 packages = \
 ['daisyfl',
  'daisyfl.client',
  'daisyfl.client.grpc_client',
+ 'daisyfl.client.grpc_server',
  'daisyfl.common',
+ 'daisyfl.master',
+ 'daisyfl.master.grpc_server',
  'daisyfl.operator',
  'daisyfl.operator.base',
  'daisyfl.operator.base_async',
  'daisyfl.operator.msg_demo',
  'daisyfl.operator.sec_agg',
  'daisyfl.operator.strategy',
  'daisyfl.operator.utils',
  'daisyfl.proto',
- 'daisyfl.server',
- 'daisyfl.server.grpc_server',
  'daisyfl.simulation',
  'daisyfl.simulation.ray_transport',
- 'daisyfl.utils']
+ 'daisyfl.utils',
+ 'daisyfl.zone',
+ 'daisyfl.zone.grpc_client',
+ 'daisyfl.zone.grpc_server']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Flask>=2.2.2,<3.0.0',
  'cryptography>=38.0.4,<39.0.0',
  'dataclasses-json>=0.5.7,<0.6.0',
  'grpcio>=1.43.0,<2.0.0',
  'iterators>=0.0.2,<0.0.3',
  'numpy>=1.21.0,<2.0.0',
  'protobuf>=3.19.0,<4.0.0',
- 'pycryptodome>=3.16.0,<4.0.0',
- 'urllib3==1.26.15']
+ 'pycryptodome>=3.16.0,<4.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'],
  'simulation': ['ray[default]>=2.0.0,<2.1.0']}
 
 setup_kwargs = {
     'name': 'daisyfl',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': 'Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing',
     'long_description': "# Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing\n\n\n## dev mode (virtual environment)\n### 1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n### 2. build up environment\nprepare and activate your virtual environment (python=3.8^)\n```\ncd daisy\n./dev/bootstrap.sh\n```\n### develop<br>\n### setup examples\ndon't overwrite daisyfl dependency in this step.<br>\n```\ncd <example_path>\npip install <pkgs_for_your_example>\n```\n### 5. run examples\n\n## dev mode (docker)\n### 1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n### 2. build up environment\n```\ndocker run -it -v <daisy_source_code>:/root/daisy tcfwbper/daisyfl-dev:<version_tag> /bin/bash\n```\n### 3. develop<br>\n### 4. setup examples<br>\ndon't overwrite daisyfl dependency in this step.<br>\n```\ndocker attach <container_id>\n```\n```\ncd <example_path> && conda activate daisy\npip install <pkgs_for_your_example>\n```\n### 5. run examples\n\n## user mode\n### 1. install daisyfl\n```\npip install <daisyfl_version>\n```\n### 2. setup examples\n```\npip install <pkgs_for_your_example>\n```\n### 3. run examples",
     'author': 'tcfwbper',
     'author_email': 'b05208031@ntu.edu.tw',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Intelligent-Systems-Lab/daisy',
```

### Comparing `daisyfl-0.5.2/PKG-INFO` & `daisyfl-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daisyfl
-Version: 0.5.2
+Version: 0.5.3
 Summary: Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing
 Home-page: https://github.com/Intelligent-Systems-Lab/daisy
 License: Apache-2.0
 Author: tcfwbper
 Author-email: b05208031@ntu.edu.tw
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,15 +35,14 @@
 Requires-Dist: grpcio (>=1.43.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.0.0,<5.0.0); python_version < "3.8"
 Requires-Dist: iterators (>=0.0.2,<0.0.3)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: protobuf (>=3.19.0,<4.0.0)
 Requires-Dist: pycryptodome (>=3.16.0,<4.0.0)
 Requires-Dist: ray[default] (>=2.0.0,<2.1.0); extra == "simulation"
-Requires-Dist: urllib3 (==1.26.15)
 Project-URL: Documentation, https://github.com/Intelligent-Systems-Lab/daisy/tree/main/doc/daisy
 Project-URL: Repository, https://github.com/Intelligent-Systems-Lab/daisy
 Description-Content-Type: text/markdown
 
 # Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing
```


# Comparing `tmp/snet-cli-2.1.1.tar.gz` & `tmp/snet.cli-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snet-cli-2.1.1.tar", last modified: Fri Mar 15 10:47:25 2024, max compression
+gzip compressed data, was "snet.cli-2.1.2.tar", last modified: Fri Apr 26 15:35:38 2024, max compression
```

## Comparing `snet-cli-2.1.1.tar` & `snet.cli-2.1.2.tar`

### file list

```diff
@@ -1,78 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.197041 snet-cli-2.1.1/
--rw-r--r--   0 root         (0) root         (0)     1071 2024-03-15 10:47:03.000000 snet-cli-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      306 2024-03-15 10:47:03.000000 snet-cli-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      945 2024-03-15 10:47:25.197041 snet-cli-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2929 2024-03-15 10:47:03.000000 snet-cli-2.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-15 10:47:25.197041 snet-cli-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      955 2024-03-15 10:47:03.000000 snet-cli-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.189041 snet-cli-2.1.1/snet/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.193041 snet-cli-2.1.1/snet/snet_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/contract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.193041 snet-cli-2.1.1/snet/snet_cli/metadata/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12915 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/metadata/organization.py
--rw-r--r--   0 root         (0) root         (0)    22830 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/metadata/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.193041 snet-cli-2.1.1/snet/snet_cli/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.189041 snet-cli-2.1.1/snet/snet_cli/resources/contracts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.193041 snet-cli-2.1.1/snet/snet_cli/resources/contracts/abi/
--rw-r--r--   0 root         (0) root         (0)     8656 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/contracts/abi/MultiPartyEscrow.json
--rw-r--r--   0 root         (0) root         (0)     5433 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/contracts/abi/Registry.json
--rw-r--r--   0 root         (0) root         (0)     7461 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/contracts/abi/SingularityNetToken.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.193041 snet-cli-2.1.1/snet/snet_cli/resources/contracts/networks/
--rw-r--r--   0 root         (0) root         (0)     9214 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/contracts/networks/MultiPartyEscrow.json
--rw-r--r--   0 root         (0) root         (0)     7520 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/contracts/networks/Registry.json
--rw-r--r--   0 root         (0) root         (0)     6206 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/contracts/networks/SingularityNetToken.json
--rw-r--r--   0 root         (0) root         (0)       54 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.193041 snet-cli-2.1.1/snet/snet_cli/resources/proto/
--rw-r--r--   0 root         (0) root         (0)     1639 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/control_service.proto
--rw-r--r--   0 root         (0) root         (0)     2335 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/control_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5986 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/control_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      466 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/merckledag.proto
--rw-r--r--   0 root         (0) root         (0)     1250 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/merckledag_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/merckledag_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3338 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/state_service.proto
--rw-r--r--   0 root         (0) root         (0)     2777 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/state_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6235 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/state_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2886 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/token_service.proto
--rw-r--r--   0 root         (0) root         (0)     1846 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/token_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5078 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/token_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3395 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/training.proto
--rw-r--r--   0 root         (0) root         (0)     5030 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/training_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9006 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/training_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      397 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/unixfs.proto
--rw-r--r--   0 root         (0) root         (0)     1650 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/unixfs_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2024-03-15 10:47:23.000000 snet-cli-2.1.1/snet/snet_cli/resources/proto/unixfs_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)   277620 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/resources/root_certificate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.193041 snet-cli-2.1.1/snet/snet_cli/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4294 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/utils/ipfs_utils.py
--rw-r--r--   0 root         (0) root         (0)     3898 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/utils/proto_utils.py
--rw-r--r--   0 root         (0) root         (0)    11201 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet/snet_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.193041 snet-cli-2.1.1/snet_cli/
--rw-r--r--   0 root         (0) root         (0)      780 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57419 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/arguments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.197041 snet-cli-2.1.1/snet_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35054 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/commands/commands.py
--rw-r--r--   0 root         (0) root         (0)     1788 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/commands/mpe_account.py
--rw-r--r--   0 root         (0) root         (0)    31282 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/commands/mpe_channel.py
--rw-r--r--   0 root         (0) root         (0)    13771 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/commands/mpe_client.py
--rw-r--r--   0 root         (0) root         (0)    27976 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/commands/mpe_service.py
--rw-r--r--   0 root         (0) root         (0)     8580 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/commands/mpe_treasurer.py
--rw-r--r--   0 root         (0) root         (0)     1941 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/commands/sdk_command.py
--rw-r--r--   0 root         (0) root         (0)    11113 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/config.py
--rw-r--r--   0 root         (0) root         (0)    13255 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/identity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.197041 snet-cli-2.1.1/snet_cli/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      841 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/utils/agix2cogs.py
--rw-r--r--   0 root         (0) root         (0)     2630 2024-03-15 10:47:03.000000 snet-cli-2.1.1/snet_cli/utils/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:47:25.197041 snet-cli-2.1.1/snet_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      945 2024-03-15 10:47:25.000000 snet-cli-2.1.1/snet_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2359 2024-03-15 10:47:25.000000 snet-cli-2.1.1/snet_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 10:47:25.000000 snet-cli-2.1.1/snet_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-03-15 10:47:25.000000 snet-cli-2.1.1/snet_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-15 10:47:25.000000 snet-cli-2.1.1/snet_cli.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      373 2024-03-15 10:47:25.000000 snet-cli-2.1.1/snet_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-15 10:47:25.000000 snet-cli-2.1.1/snet_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.802034 snet.cli-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-26 15:35:12.000000 snet.cli-2.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      195 2024-04-26 15:35:12.000000 snet.cli-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5677 2024-04-26 15:35:38.802034 snet.cli-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-04-26 15:35:12.000000 snet.cli-2.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 15:35:38.802034 snet.cli-2.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-26 15:35:12.000000 snet.cli-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.798034 snet.cli-2.1.2/snet/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.798034 snet.cli-2.1.2/snet/cli/
+-rw-r--r--   0 root         (0) root         (0)      781 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57420 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/arguments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.798034 snet.cli-2.1.2/snet/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35002 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/commands/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/commands/mpe_account.py
+-rw-r--r--   0 root         (0) root         (0)    31284 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/commands/mpe_channel.py
+-rw-r--r--   0 root         (0) root         (0)    13979 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/commands/mpe_client.py
+-rw-r--r--   0 root         (0) root         (0)    27870 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/commands/mpe_service.py
+-rw-r--r--   0 root         (0) root         (0)     8570 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/commands/mpe_treasurer.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/commands/sdk_command.py
+-rw-r--r--   0 root         (0) root         (0)    11113 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/contract.py
+-rw-r--r--   0 root         (0) root         (0)    13237 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/identity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.798034 snet.cli-2.1.2/snet/cli/metadata/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13162 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/metadata/organization.py
+-rw-r--r--   0 root         (0) root         (0)    22825 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/metadata/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.802034 snet.cli-2.1.2/snet/cli/resources/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/resources/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.802034 snet.cli-2.1.2/snet/cli/resources/proto/
+-rw-r--r--   0 root         (0) root         (0)     1639 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/resources/proto/control_service.proto
+-rw-r--r--   0 root         (0) root         (0)     2335 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/control_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5986 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/control_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      466 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/resources/proto/merckledag.proto
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/merckledag_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/merckledag_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/resources/proto/state_service.proto
+-rw-r--r--   0 root         (0) root         (0)     2777 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/state_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6235 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/state_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/resources/proto/token_service.proto
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/token_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5078 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/token_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/resources/proto/training.proto
+-rw-r--r--   0 root         (0) root         (0)     5030 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/training_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9006 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/training_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      397 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/resources/proto/unixfs.proto
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/unixfs_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-26 15:35:37.000000 snet.cli-2.1.2/snet/cli/resources/proto/unixfs_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)   277620 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/resources/root_certificate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.798034 snet.cli-2.1.2/snet/cli/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.798034 snet.cli-2.1.2/snet/cli/test/functional_tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.802034 snet.cli-2.1.2/snet/cli/test/functional_tests/mint/
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/test/functional_tests/mint/mint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.802034 snet.cli-2.1.2/snet/cli/test/functional_tests/simple_daemon/
+-rw-r--r--   0 root         (0) root         (0)     7328 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/test/functional_tests/simple_daemon/test_simple_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.802034 snet.cli-2.1.2/snet/cli/test/unit_tests/
+-rw-r--r--   0 root         (0) root         (0)     1495 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/test/unit_tests/test_mpe_service_metadata_1.py
+-rw-r--r--   0 root         (0) root         (0)     5566 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/test/unit_tests/test_mpe_service_metadata_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.802034 snet.cli-2.1.2/snet/cli/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      841 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/utils/agix2cogs.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     4303 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/utils/ipfs_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/utils/proto_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2024-04-26 15:35:12.000000 snet.cli-2.1.2/snet/cli/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 15:35:38.802034 snet.cli-2.1.2/snet.cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5677 2024-04-26 15:35:38.000000 snet.cli-2.1.2/snet.cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1999 2024-04-26 15:35:38.000000 snet.cli-2.1.2/snet.cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 15:35:38.000000 snet.cli-2.1.2/snet.cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-26 15:35:38.000000 snet.cli-2.1.2/snet.cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-26 15:35:38.000000 snet.cli-2.1.2/snet.cli.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      414 2024-04-26 15:35:38.000000 snet.cli-2.1.2/snet.cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-26 15:35:38.000000 snet.cli-2.1.2/snet.cli.egg-info/top_level.txt
```

### Comparing `snet-cli-2.1.1/LICENSE` & `snet.cli-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/contract.py` & `snet.cli-2.1.2/snet/cli/contract.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/metadata/organization.py` & `snet.cli-2.1.2/snet/cli/metadata/organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 from enum import Enum
 from json import JSONEncoder
-
 import json
 
+import validators
+
 
 class DefaultEncoder(JSONEncoder):
     def default(self, o):
         return o.__dict__
 
 
 class AssetType(Enum):
@@ -26,14 +27,19 @@
     def add_payment_storage_client_details(self, connection_time_out, request_timeout, endpoints):
         self.connection_timeout = connection_time_out
         self.request_timeout = request_timeout
         self.endpoints = endpoints
 
     @classmethod
     def from_json(cls, json_data: dict):
+        endpoints = json_data["endpoints"]
+        if endpoints:
+            for endpoint in endpoints:
+                if not validators.url(endpoint):
+                    raise Exception("Invalid endpoint passed in json file")
         return cls(**json_data)
 
     def validate(self):
         if len(self.endpoints) < 1:
             raise Exception(
                 "At least one endpoint is required for payment channel ")
```

### Comparing `snet-cli-2.1.1/snet/snet_cli/metadata/service.py` & `snet.cli-2.1.2/snet/cli/metadata/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import re
 import json
 import base64
 
 from collections import defaultdict
 from enum import Enum
 
-from snet.snet_cli.utils.utils import is_valid_endpoint
+from snet.cli.utils.utils import is_valid_endpoint
 
 
 # Supported Asset types
 class AssetType(Enum):
     HERO_IMAGE = "hero_image"
     IMAGES = "images"
     DOCUMENTATION = "documentation"
```

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/control_service.proto` & `snet.cli-2.1.2/snet/cli/resources/proto/control_service.proto`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/control_service_pb2.py` & `snet.cli-2.1.2/snet/cli/resources/proto/control_service_pb2.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/control_service_pb2_grpc.py` & `snet.cli-2.1.2/snet/cli/resources/proto/control_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/merckledag_pb2.py` & `snet.cli-2.1.2/snet/cli/resources/proto/merckledag_pb2.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/state_service.proto` & `snet.cli-2.1.2/snet/cli/resources/proto/state_service.proto`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/state_service_pb2.py` & `snet.cli-2.1.2/snet/cli/resources/proto/state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/state_service_pb2_grpc.py` & `snet.cli-2.1.2/snet/cli/resources/proto/state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/token_service.proto` & `snet.cli-2.1.2/snet/cli/resources/proto/token_service.proto`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/token_service_pb2.py` & `snet.cli-2.1.2/snet/cli/resources/proto/token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/token_service_pb2_grpc.py` & `snet.cli-2.1.2/snet/cli/resources/proto/token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/training.proto` & `snet.cli-2.1.2/snet/cli/resources/proto/training.proto`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/training_pb2.py` & `snet.cli-2.1.2/snet/cli/resources/proto/training_pb2.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/training_pb2_grpc.py` & `snet.cli-2.1.2/snet/cli/resources/proto/training_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/proto/unixfs_pb2.py` & `snet.cli-2.1.2/snet/cli/resources/proto/unixfs_pb2.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/resources/root_certificate.py` & `snet.cli-2.1.2/snet/cli/resources/root_certificate.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet/snet_cli/utils/ipfs_utils.py` & `snet.cli-2.1.2/snet/cli/utils/ipfs_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
 def get_from_ipfs_and_checkhash(ipfs_client, ipfs_hash_base58, validate=True):
     """
     Get file from ipfs
     We must check the hash becasue we cannot believe that ipfs_client wasn't been compromise
     """
     if validate:
-        from snet.snet_cli.resources.proto.unixfs_pb2 import Data
-        from snet.snet_cli.resources.proto.merckledag_pb2 import MerkleNode
+        from snet.cli.resources.proto.unixfs_pb2 import Data
+        from snet.cli.resources.proto.merckledag_pb2 import MerkleNode
 
         # No nice Python library to parse ipfs blocks, so do it ourselves.
         block_data = ipfs_client.block.get(ipfs_hash_base58)
         mn = MerkleNode()
         mn.ParseFromString(block_data)
         unixfs_data = Data()
         unixfs_data.ParseFromString(mn.Data)
@@ -112,10 +112,11 @@
                 raise Exception(
                     "tarball has directories. We do not support it.")
             if not m.isfile():
                 raise Exception(
                     "tarball contains %s which is not a files" % m.name)
             fullname = os.path.join(protodir, m.name)
             if os.path.exists(fullname):
-                raise Exception("%s already exists." % fullname)
+                os.remove(fullname)
+                print("%s removed." % fullname)
         # now it is safe to call extractall
         f.extractall(protodir)
```

### Comparing `snet-cli-2.1.1/snet/snet_cli/utils/proto_utils.py` & `snet.cli-2.1.2/snet/cli/utils/proto_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Utils related to protobuf """
 import sys
 from pathlib import Path
 import os
+
 from google.protobuf import json_format
 
 
 def import_protobuf_from_dir(proto_dir, method_name, service_name=None):
     """
     Dynamic import of grpc-protobuf from given directory (proto_dir)
     service_name should be provided only in the case of conflicting method names (two methods with the same name in difference services).
```

### Comparing `snet-cli-2.1.1/snet/snet_cli/utils/utils.py` & `snet.cli-2.1.2/snet/cli/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import json
 import os
 import subprocess
 import functools
 import sys
-
+import importlib.resources
+from importlib.metadata import distribution
 from urllib.parse import urlparse
 from pathlib import Path, PurePath
 
 import web3
-
-import importlib.resources
-from importlib.metadata import distribution
-
 import grpc
 from grpc_tools.protoc import main as protoc
 
-from snet import snet_cli
-from snet.snet_cli.resources.root_certificate import certificate
+from snet import cli
+from snet.cli.resources.root_certificate import certificate
 
-RESOURCES_PATH = PurePath(os.path.dirname(snet_cli.__file__)).joinpath("resources")
+RESOURCES_PATH = PurePath(os.path.dirname(cli.__file__)).joinpath("resources")
 
 
 class DefaultAttributeObject(object):
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             if v is not None:
                 setattr(self, k, v)
@@ -129,35 +126,22 @@
         if os.path.isfile(path):
             _add_next_paths(path, entry_path, seen_paths, next_paths)
         else:
             raise IOError("Import path must be a valid file: {}".format(path))
     return seen_paths
 
 
-def get_contract_def(contract_name, contract_artifacts_root=RESOURCES_PATH.joinpath("contracts")):
-    contract_def = {}
-    with open(Path(__file__).absolute().parent.joinpath(contract_artifacts_root, "abi",
-                                                        "{}.json".format(contract_name))) as f:
-        contract_def["abi"] = json.load(f)
-    if os.path.isfile(Path(__file__).absolute().parent.joinpath(contract_artifacts_root, "networks",
-                                                                "{}.json".format(contract_name))):
-        with open(Path(__file__).absolute().parent.joinpath(contract_artifacts_root, "networks",
-                                                            "{}.json".format(contract_name))) as f:
-            contract_def["networks"] = json.load(f)
-    return contract_def
-
-
 def read_temp_tar(f):
     f.flush()
     f.seek(0)
     return f
 
 
 def get_cli_version():
-    return distribution("snet-cli").version
+    return distribution("snet.cli").version
 
 
 def compile_proto(entry_path, codegen_dir, proto_file=None, target_language="python"):
     try:
         if not os.path.exists(codegen_dir):
             os.makedirs(codegen_dir)
         proto_include = importlib.resources.files('grpc_tools') / '_proto'
@@ -276,38 +260,14 @@
     1
     >>> rgetattr(args, "b.c")
     2
     """
     return functools.reduce(getattr, [obj] + attr.split('.'))
 
 
-def get_contract_object(w3, contract_file, address=None):
-    with open(RESOURCES_PATH.joinpath("contracts", "abi", contract_file)) as f:
-        abi = json.load(f)
-    if address:
-        return w3.eth.contract(abi=abi, address=w3.to_checksum_address(address))
-    with open(RESOURCES_PATH.joinpath("contracts", "networks", contract_file)) as f:
-        networks = json.load(f)
-        address = w3.to_checksum_address(networks[w3.net.version]["address"])
-    return w3.eth.contract(abi=abi, address=address)
-
-
-def get_contract_deployment_block(w3, contract_file):
-    try:
-        with open(RESOURCES_PATH.joinpath("contracts", "networks", contract_file)) as f:
-            networks = json.load(f)
-            txn_hash = networks[w3.net.version]["transactionHash"]
-        return w3.eth.get_transaction_receipt(txn_hash).blockNumber
-    except Exception:
-        # TODO Hack as currenlty dependecy is on snet-cli so for test purpose return 0,need to remove dependecies from snet-cli ,currently very tightly coupled with it
-        if w3.net.version in [1, 5, 11155111]:
-            raise Exception("Transaction hash not found for deployed mpe contract")
-        return 0
-
-
 def normalize_private_key(private_key):
     if private_key.startswith("0x"):
         private_key = bytes(bytearray.fromhex(private_key[2:]))
     else:
         private_key = bytes(bytearray.fromhex(private_key))
     return private_key
 
@@ -324,7 +284,14 @@
         sys.path.insert(0, self.path)
 
     def __exit__(self, exc_type, exc_value, traceback):
         try:
             sys.path.remove(self.path)
         except ValueError:
             pass
+
+
+def find_file_by_keyword(directory, keyword):
+        for root, dirs, files in os.walk(directory):
+            for file in files:
+                if keyword in file:
+                    return file
```

### Comparing `snet-cli-2.1.1/snet_cli/__init__.py` & `snet.cli-2.1.2/snet/cli/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 # PYTHON_ARGCOMPLETE_OK
 
 import sys
 
-from snet_cli import arguments
-from snet_cli.config import Config
 import argcomplete
 
+from snet.cli import arguments
+from snet.cli.config import Config
+
 
 def main():
     try:
         argv = sys.argv[1:]
         conf   = Config()
         parser = arguments.get_root_parser(conf)
         argcomplete.autocomplete(parser)
```

### Comparing `snet-cli-2.1.1/snet_cli/arguments.py` & `snet.cli-2.1.2/snet/cli/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import argparse
 import os
 import re
 import sys
-from pathlib import Path
 
-from snet_cli.commands.commands import IdentityCommand, SessionSetCommand, SessionShowCommand, NetworkCommand, ContractCommand, \
-    OrganizationCommand, VersionCommand
-from snet_cli.identity import get_identity_types
-from snet_cli.commands.mpe_account import MPEAccountCommand
-from snet_cli.commands.mpe_service import MPEServiceCommand
-from snet_cli.commands.mpe_client import MPEClientCommand
-from snet_cli.commands.mpe_treasurer import MPETreasurerCommand
-from snet_cli.commands.sdk_command import SDKCommand
-from snet_cli.utils.agix2cogs import stragix2cogs
-from snet_cli.config import Config, get_session_keys, get_session_network_keys_removable
+from snet.contracts import get_all_abi_contract_files, get_contract_def
 
-from snet_cli.commands.mpe_channel import MPEChannelCommand
-from snet.snet_cli.utils.utils import type_converter, get_contract_def, RESOURCES_PATH
+from snet.cli.commands.commands import ContractCommand, IdentityCommand, NetworkCommand, OrganizationCommand, SessionSetCommand, SessionShowCommand, VersionCommand
+from snet.cli.commands.mpe_account import MPEAccountCommand
+from snet.cli.commands.mpe_channel import MPEChannelCommand
+from snet.cli.commands.mpe_client import MPEClientCommand
+from snet.cli.commands.mpe_service import MPEServiceCommand
+from snet.cli.commands.mpe_treasurer import MPETreasurerCommand
+from snet.cli.commands.sdk_command import SDKCommand
+from snet.cli.config import Config, get_session_keys, get_session_network_keys_removable
+from snet.cli.identity import get_identity_types
+from snet.cli.utils.agix2cogs import stragix2cogs
+from snet.cli.utils.utils import type_converter
 
 
 class CustomParser(argparse.ArgumentParser):
     def __init__(self, default_choice=None, *args, **kwargs):
         self.default_choice = default_choice
         super().__init__(*args, **kwargs)
 
@@ -229,15 +228,16 @@
 
 def add_contract_options(parser):
     parser.set_defaults(cmd=ContractCommand)
 
     subparsers = parser.add_subparsers(title="contracts", metavar="CONTRACT")
     subparsers.required = True
 
-    for path in Path(RESOURCES_PATH.joinpath("contracts", "abi")).glob("*json"):
+    contracts = get_all_abi_contract_files()
+    for path in contracts:
         contract_name = re.search(
             r"([^.]*)\.json", os.path.basename(path)).group(1)
         contract_p = subparsers.add_parser(
             contract_name, help="{} contract".format(contract_name))
         add_contract_function_options(contract_p, contract_name)
 
 
@@ -261,15 +261,15 @@
 def add_organization_options(parser):
     parser.set_defaults(cmd=OrganizationCommand)
 
     subparsers = parser.add_subparsers(
         title="Organization commands", metavar="COMMAND")
     subparsers.required = True
 
-    p = subparsers.add_parser("metadata-init", help="Initalize matadata for organization ")
+    p = subparsers.add_parser("metadata-init", help="Initialize metadata for organization")
     p.set_defaults(fn="initialize_metadata")
     p.add_argument("org_name", help="Organization name", metavar="ORG_NAME")
     p.add_argument("org_id", default=None, help="Unique organization Id", metavar="ORG_ID")
     p.add_argument("org_type", help="organization type based on creator of organization whether it is individual or business/organization "
                                     "[ individual | organization ]",
                    choices=["individual", "organization"], metavar="ORG_TYPE")
     add_p_registry_address_opt(p)
@@ -959,15 +959,15 @@
     p.add_argument("--encoding",
                    default="proto",
                    choices=['proto', 'json'],
                    help="Service encoding")
 
     p.add_argument("--service-type",
                    default="grpc",
-                   choices=['grpc', 'jsonrpc', 'process'],
+                   choices=['grpc', 'http', 'jsonrpc', 'process'],
                    help="Service type")
 
     p = subparsers.add_parser("metadata-set-model",
                               help="Publish protobuf model in ipfs and update existed metadata file")
     p.set_defaults(fn="publish_proto_metadata_update")
     p.add_argument("protodir",
                    help="Directory which contains protobuf files",
```

### Comparing `snet-cli-2.1.1/snet_cli/commands/commands.py` & `snet.cli-2.1.2/snet/cli/commands/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 import sys
 from textwrap import indent
 from urllib.parse import urljoin
 
 import ipfshttpclient
 import yaml
 from rfc3986 import urlparse
-from snet.snet_cli.contract import Contract
-from snet.snet_cli.metadata.organization import OrganizationMetadata, PaymentStorageClient, Payment, Group
-from snet.snet_cli.utils.ipfs_utils import bytesuri_to_hash, get_from_ipfs_and_checkhash, hash_to_bytesuri
-from snet.snet_cli.utils.ipfs_utils import publish_file_in_ipfs
-from snet.snet_cli.utils.utils import DefaultAttributeObject, get_web3, serializable, type_converter, get_contract_def, \
-    get_cli_version, bytes32_to_str
-from snet_cli.identity import RpcIdentityProvider, MnemonicIdentityProvider, TrezorIdentityProvider, \
-    LedgerIdentityProvider, KeyIdentityProvider, KeyStoreIdentityProvider
-from snet_cli.identity import get_kws_for_identity_type
-from snet_cli.utils.config import get_contract_address, get_field_from_args_or_session, read_default_contract_address
 import web3
+from snet.contracts import get_contract_def
+
+from snet.cli.contract import Contract
+from snet.cli.identity import KeyIdentityProvider, KeyStoreIdentityProvider, LedgerIdentityProvider, \
+    MnemonicIdentityProvider, RpcIdentityProvider, TrezorIdentityProvider, get_kws_for_identity_type
+from snet.cli.metadata.organization import OrganizationMetadata, PaymentStorageClient, Payment, Group
+from snet.cli.utils.config import get_contract_address, get_field_from_args_or_session, \
+    read_default_contract_address
+from snet.cli.utils.ipfs_utils import bytesuri_to_hash, get_from_ipfs_and_checkhash, \
+    hash_to_bytesuri, publish_file_in_ipfs
+from snet.cli.utils.utils import DefaultAttributeObject, get_web3, serializable, type_converter, \
+    get_cli_version, bytes32_to_str
 
 
 class Command(object):
     def __init__(self, config, args, out_f=sys.stdout, err_f=sys.stderr):
         self.config = config
         self.args = args
         self.out_f = out_f
```

### Comparing `snet-cli-2.1.1/snet_cli/commands/mpe_account.py` & `snet.cli-2.1.2/snet/cli/commands/mpe_account.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from snet_cli.commands.commands import BlockchainCommand
-from snet_cli.utils.agix2cogs import cogs2stragix
-from snet_cli.utils.config import get_contract_address
+from snet.cli.commands.commands import BlockchainCommand
+from snet.cli.utils.agix2cogs import cogs2stragix
 
 
 class MPEAccountCommand(BlockchainCommand):
 
     def print_account(self):
         self._printout(self.ident.address)
```

### Comparing `snet-cli-2.1.1/snet_cli/commands/mpe_channel.py` & `snet.cli-2.1.2/snet/cli/commands/mpe_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import os
 import pickle
 import shutil
 import tempfile
 from collections import defaultdict
 from pathlib import Path
 
-from snet.snet_cli.metadata.service import mpe_service_metadata_from_json, load_mpe_service_metadata
-from snet.snet_cli.metadata.organization import OrganizationMetadata
-from snet.snet_cli.utils.ipfs_utils import safe_extract_proto_from_ipfs, get_from_ipfs_and_checkhash, bytesuri_to_hash
-from snet.snet_cli.utils.utils import compile_proto, get_contract_def, abi_get_element_by_name, \
-    abi_decode_struct_to_dict, \
-    type_converter
-from snet_cli.commands.commands import OrganizationCommand
-from snet_cli.utils.agix2cogs import cogs2stragix
+from eth_abi.codec import ABICodec
 from web3._utils.encoding import pad_hex
 from web3._utils.events import get_event_data
-from eth_abi.codec import ABICodec
+from snet.contracts import get_contract_def
+
+from snet.cli.commands.commands import OrganizationCommand
+from snet.cli.metadata.service import mpe_service_metadata_from_json, load_mpe_service_metadata
+from snet.cli.metadata.organization import OrganizationMetadata
+from snet.cli.utils.agix2cogs import cogs2stragix
+from snet.cli.utils.ipfs_utils import bytesuri_to_hash, get_from_ipfs_and_checkhash, safe_extract_proto_from_ipfs
+from snet.cli.utils.utils import abi_decode_struct_to_dict, abi_get_element_by_name, \
+    compile_proto, type_converter
+
 
 # we inherit MPEServiceCommand because we need _get_service_metadata_from_registry
 class MPEChannelCommand(OrganizationCommand):
 
     def _get_persistent_mpe_dir(self):
         """ get persistent storage for mpe """
         mpe_address = self.get_mpe_address().lower()
```

### Comparing `snet-cli-2.1.1/snet_cli/commands/mpe_client.py` & `snet.cli-2.1.2/snet/cli/commands/mpe_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import base64
 import json
 import sys
 from pathlib import Path
 
 from eth_account.messages import encode_defunct
-from snet.snet_cli.utils.proto_utils import import_protobuf_from_dir, switch_to_json_payload_encoding
-from snet.snet_cli.utils.utils import open_grpc_channel, rgetattr, RESOURCES_PATH
-from snet_cli.commands.mpe_channel import MPEChannelCommand
-from snet_cli.utils.agix2cogs import cogs2stragix
+
+from snet.cli.commands.mpe_channel import MPEChannelCommand
+from snet.cli.utils.agix2cogs import cogs2stragix
+from snet.cli.utils.proto_utils import import_protobuf_from_dir, switch_to_json_payload_encoding
+from snet.cli.utils.utils import open_grpc_channel, rgetattr, RESOURCES_PATH
 
 
 # we inherit MPEChannelCommand because client needs channels
 class MPEClientCommand(MPEChannelCommand):
     prefixInSignature = "__MPE_claim_message"
 
     # I. Signature related functions
@@ -177,42 +178,64 @@
     def _get_channel_state_from_server(self, grpc_channel, channel_id):
 
         # We should simply statically import everything, but it doesn't work because of the following issue in protobuf: https://github.com/protocolbuffers/protobuf/issues/1491
         #from snet_cli.resources.proto.state_service_pb2      import ChannelStateRequest            as request_class
         #from snet_cli.resources.proto.state_service_pb2_grpc import PaymentChannelStateServiceStub as stub_class
         proto_dir = RESOURCES_PATH.joinpath("proto")
         stub_class, request_class, _ = import_protobuf_from_dir(
-            proto_dir, "GetChannelState")
+            proto_dir,
+            "GetChannelState"
+        )
         current_block = self.ident.w3.eth.block_number
         mpe_address = self.get_mpe_address()
-        message = self.w3.solidity_keccak(["string",             "address",    "uint256",   "uint256"],
-                                       ["__get_channel_state", mpe_address, channel_id, current_block])
+        message = self.w3.solidity_keccak(
+            ["string", "address", "uint256", "uint256"],
+            ["__get_channel_state", mpe_address, channel_id, current_block]
+        )
         signature = self.ident.sign_message_after_solidity_keccak(message)
 
-        request = request_class(channel_id=self.w3.to_bytes(
-            channel_id), signature=bytes(signature), current_block=current_block)
+        request = request_class(
+            channel_id=self.w3.to_bytes(channel_id),
+            signature=bytes(signature),
+            current_block=current_block
+        )
 
         stub = stub_class(grpc_channel)
         response = getattr(stub, "GetChannelState")(request)
         # convert bytes to int
         state = dict()
         state["current_nonce"] = int.from_bytes(
-            response.current_nonce,         byteorder='big')
+            response.current_nonce,
+            byteorder='big'
+        )
         state["current_signed_amount"] = int.from_bytes(
-            response.current_signed_amount, byteorder='big')
+            response.current_signed_amount,
+            byteorder='big'
+        )
 
         error_message = "Error in _get_channel_state_from_server. My own signature from the server is not valid."
-        self._assert_validity_of_my_signature_or_zero_amount(bytes(
-            response.current_signature),  channel_id, state["current_nonce"],     state["current_signed_amount"],  error_message)
+        self._assert_validity_of_my_signature_or_zero_amount(
+            bytes(response.current_signature),
+            channel_id, state["current_nonce"],
+            state["current_signed_amount"],
+            error_message
+        )
 
         if hasattr(response, "old_nonce_signed_amount"):
             state["old_nonce_signed_amount"] = int.from_bytes(
-                response.old_nonce_signed_amount, byteorder='big')
-            self._assert_validity_of_my_signature_or_zero_amount(bytes(
-                response.old_nonce_signature), channel_id, state["current_nonce"] - 1, state["old_nonce_signed_amount"], error_message)
+                response.old_nonce_signed_amount,
+                byteorder='big'
+            )
+            self._assert_validity_of_my_signature_or_zero_amount(
+                bytes(response.old_nonce_signature),
+                channel_id,
+                state["current_nonce"] - 1,
+                state["old_nonce_signed_amount"],
+                error_message
+            )
 
         return state
 
     def _calculate_unspent_amount(self, blockchain, server):
         if server["current_nonce"] == blockchain["nonce"]:
             return blockchain["value"] - server["current_signed_amount"]
         if server["current_nonce"] - 1 != blockchain["nonce"]:
@@ -239,19 +262,20 @@
 
         return server["current_nonce"], server["current_signed_amount"], unspent_amount
 
     def print_channel_state_statelessly(self):
         grpc_channel = open_grpc_channel(self.args.endpoint)
 
         current_nonce, current_amount, unspent_amount = self._get_channel_state_statelessly(
-            grpc_channel, self.args.channel_id)
+            grpc_channel,
+            self.args.channel_id
+        )
         self._printout("current_nonce                  = %i" % current_nonce)
         self._printout("current_signed_amount_in_cogs  = %i" % current_amount)
-        self._printout("current_unspent_amount_in_cogs = %s" %
-                       str(unspent_amount))
+        self._printout("current_unspent_amount_in_cogs = %s" % str(unspent_amount))
 
     def _get_price_from_metadata(self, service_metadata, group_name):
         for group in service_metadata.m["groups"]:
             if group["group_name"] == group_name:
                 pricings = group["pricing"]
                 for pricing in pricings:
                     if pricing["price_model"] == "fixed_price":
@@ -268,19 +292,20 @@
         org_metadata = self._read_metadata_for_org(self.args.org_id)
         service_metadata = self._get_service_metadata()
         endpoint = self._get_endpoint_from_metadata_or_args(service_metadata)
         grpc_channel = open_grpc_channel(endpoint)
 
         # if channel was not initilized we will try to initailize it (it will work only in simple case of signer == sender)
         channel = self._smart_get_initialized_channel_for_org(
-            org_metadata, filter_by="signer")
+            org_metadata,
+            filter_by="signer"
+        )
         channel_id = channel["channelId"]
         price = self._get_price_from_metadata(service_metadata, group_name)
-        server_state = self._get_channel_state_from_server(
-            grpc_channel, channel_id)
+        server_state = self._get_channel_state_from_server(grpc_channel, channel_id)
 
         proceed = self.args.yes or input(
             "Price for this call will be %s AGIX (use -y to remove this warning). Proceed? (y/n): " % (cogs2stragix(price))) == "y"
         if not proceed:
             self._error("Cancelled")
 
         return self._call_server_via_grpc_channel(grpc_channel, channel_id, server_state["current_nonce"], server_state["current_signed_amount"] + price, params, service_metadata)
```

### Comparing `snet-cli-2.1.1/snet_cli/commands/mpe_service.py` & `snet.cli-2.1.2/snet/cli/commands/mpe_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import json
 from collections import defaultdict
 from pathlib import Path
 from re import search
 from sys import exit
 
-from jsonschema import validate, ValidationError
-
-import snet.snet_cli.utils.ipfs_utils as ipfs_utils
 from grpc_health.v1 import health_pb2 as heartb_pb2
 from grpc_health.v1 import health_pb2_grpc as heartb_pb2_grpc
-from snet.snet_cli.metadata.service import MPEServiceMetadata, load_mpe_service_metadata, \
-    mpe_service_metadata_from_json
-from snet.snet_cli.metadata.organization import OrganizationMetadata
-from snet.snet_cli.utils.ipfs_utils import hash_to_bytesuri, bytesuri_to_hash, get_from_ipfs_and_checkhash, \
-    safe_extract_proto_from_ipfs
-from snet.snet_cli.utils.utils import type_converter, bytes32_to_str, open_grpc_channel
-from snet_cli.commands.commands import BlockchainCommand
+from jsonschema import validate, ValidationError
+
+from snet.cli.commands.commands import BlockchainCommand
+from snet.cli.metadata.organization import OrganizationMetadata
+from snet.cli.metadata.service import MPEServiceMetadata, load_mpe_service_metadata, mpe_service_metadata_from_json
+from snet.cli.utils import ipfs_utils
+from snet.cli.utils.utils import open_grpc_channel, type_converter
 
 
 class MPEServiceCommand(BlockchainCommand):
 
     def publish_proto_in_ipfs(self):
         """ Publish proto files in ipfs and print hash """
         ipfs_hash_base58 = ipfs_utils.publish_proto_in_ipfs(
@@ -406,16 +403,16 @@
         self._printout(self._publish_metadata_in_ipfs(self.args.metadata_file))
 
     #def _get_converted_tags(self):
     #    return [type_converter("bytes32")(tag) for tag in self.args.tags]
 
     def _get_organization_metadata_from_registry(self, org_id):
         rez = self._get_organization_registration(org_id)
-        metadata_hash = bytesuri_to_hash(rez["orgMetadataURI"])
-        metadata = get_from_ipfs_and_checkhash(
+        metadata_hash = ipfs_utils.bytesuri_to_hash(rez["orgMetadataURI"])
+        metadata = ipfs_utils.get_from_ipfs_and_checkhash(
             self._get_ipfs_client(), metadata_hash)
         metadata = metadata.decode("utf-8")
         return OrganizationMetadata.from_json(json.loads(metadata))
 
     def _get_organization_registration(self, org_id):
         params = [type_converter("bytes32")(org_id)]
         result = self.call_contract_command(
@@ -439,27 +436,27 @@
             else:
                 raise Exception(
                     "Group name %s does not exist in organization" % group["group_name"])
 
     def publish_service_with_metadata(self):
         self._validate_service_group_with_org_group_and_update_group_id(
             self.args.org_id, self.args.metadata_file)
-        metadata_uri = hash_to_bytesuri(
+        metadata_uri = ipfs_utils.hash_to_bytesuri(
             self._publish_metadata_in_ipfs(self.args.metadata_file))
         #tags = self._get_converted_tags()
         params = [type_converter("bytes32")(self.args.org_id), type_converter(
             "bytes32")(self.args.service_id), metadata_uri]
         self.transact_contract_command(
             "Registry", "createServiceRegistration", params)
 
     def publish_metadata_in_ipfs_and_update_registration(self):
         # first we check that we do not change payment_address or group_id in existed payment groups
         self._validate_service_group_with_org_group_and_update_group_id(
             self.args.org_id, self.args.metadata_file)
-        metadata_uri = hash_to_bytesuri(
+        metadata_uri = ipfs_utils.hash_to_bytesuri(
             self._publish_metadata_in_ipfs(self.args.metadata_file))
         params = [type_converter("bytes32")(self.args.org_id), type_converter(
             "bytes32")(self.args.service_id), metadata_uri]
         self.transact_contract_command(
             "Registry", "updateServiceRegistration", params)
 
     #def _get_params_for_tags_update(self):
@@ -492,16 +489,16 @@
         if rez[0] == False:
             raise Exception("Cannot find Service with id=%s in Organization with id=%s" % (
                 self.args.service_id, self.args.org_id))
         return {"metadataURI": rez[2]}
 
     def _get_service_metadata_from_registry(self):
         rez = self._get_service_registration()
-        metadata_hash = bytesuri_to_hash(rez["metadataURI"])
-        metadata = get_from_ipfs_and_checkhash(
+        metadata_hash = ipfs_utils.bytesuri_to_hash(rez["metadataURI"])
+        metadata = ipfs_utils.get_from_ipfs_and_checkhash(
             self._get_ipfs_client(), metadata_hash)
         metadata = metadata.decode("utf-8")
         metadata = mpe_service_metadata_from_json(metadata)
         return metadata
 
     def print_service_metadata_from_registry(self):
         metadata = self._get_service_metadata_from_registry()
@@ -541,20 +538,20 @@
 
     def print_service_tags_from_registry(self):
         metadata = self._get_service_metadata_from_registry()
         self._printout(" ".join(metadata.get_tags()))
 
     def extract_service_api_from_metadata(self):
         metadata = load_mpe_service_metadata(self.args.metadata_file)
-        safe_extract_proto_from_ipfs(self._get_ipfs_client(
+        ipfs_utils.safe_extract_proto_from_ipfs(self._get_ipfs_client(
         ), metadata["model_ipfs_hash"], self.args.protodir)
 
     def extract_service_api_from_registry(self):
         metadata = self._get_service_metadata_from_registry()
-        safe_extract_proto_from_ipfs(self._get_ipfs_client(
+        ipfs_utils.safe_extract_proto_from_ipfs(self._get_ipfs_client(
         ), metadata["model_ipfs_hash"], self.args.protodir)
 
     def delete_service_registration(self):
         params = [type_converter("bytes32")(self.args.org_id), type_converter(
             "bytes32")(self.args.service_id)]
         self.transact_contract_command(
             "Registry", "deleteServiceRegistration", params)
```

### Comparing `snet-cli-2.1.1/snet_cli/commands/mpe_treasurer.py` & `snet.cli-2.1.2/snet/cli/commands/mpe_treasurer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 import web3
-from snet.snet_cli.utils.proto_utils import import_protobuf_from_dir
-from snet.snet_cli.utils.utils import compile_proto, open_grpc_channel, int4bytes_big, RESOURCES_PATH
-from snet_cli.commands.mpe_client import MPEClientCommand
-from snet_cli.utils.agix2cogs import cogs2stragix
+from snet.cli.utils.proto_utils import import_protobuf_from_dir
+from snet.cli.utils.utils import compile_proto, open_grpc_channel, int4bytes_big, RESOURCES_PATH
+from snet.cli.commands.mpe_client import MPEClientCommand
+from snet.cli.utils.agix2cogs import cogs2stragix
 
 
 class MPETreasurerCommand(MPEClientCommand):
     """ We inherit MPEChannelCommand because we need _get_channel_state_from_blockchain """
 
     def _sign_message_list_unclaimed(self, mpe_address, current_block):
         message = self.w3.solidity_keccak(
```

### Comparing `snet-cli-2.1.1/snet_cli/commands/sdk_command.py` & `snet.cli-2.1.2/snet/cli/commands/sdk_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 from pathlib import Path, PurePath
-from tempfile import TemporaryDirectory
 
-from snet.snet_cli.utils.ipfs_utils import safe_extract_proto_from_ipfs
-from snet.snet_cli.utils.utils import compile_proto
-from snet_cli.commands.mpe_service import MPEServiceCommand
+from snet.cli.utils.ipfs_utils import safe_extract_proto_from_ipfs
+from snet.cli.utils.utils import compile_proto
+from snet.cli.commands.mpe_service import MPEServiceCommand
 
 
 class SDKCommand(MPEServiceCommand):
     def generate_client_library(self):
 
         if os.path.isabs(self.args.protodir):
             client_libraries_base_dir_path = PurePath(self.args.protodir)
@@ -24,19 +23,17 @@
         library_service_id = self.args.service_id
 
         library_dir_path = client_libraries_base_dir_path.joinpath(library_org_id, library_service_id, library_language)
 
         metadata = self._get_service_metadata_from_registry()
         model_ipfs_hash = metadata["model_ipfs_hash"]
 
-        with TemporaryDirectory() as temp_dir:
-            temp_dir_path = PurePath(temp_dir)
-            proto_temp_dir_path = temp_dir_path.joinpath(library_org_id, library_service_id, library_language)
-            safe_extract_proto_from_ipfs(self._get_ipfs_client(), model_ipfs_hash, proto_temp_dir_path)
+        # Receive proto files
+        safe_extract_proto_from_ipfs(self._get_ipfs_client(), model_ipfs_hash, library_dir_path)
 
-            # Compile proto files
-            compile_proto(Path(proto_temp_dir_path), library_dir_path, target_language=self.args.language)
+        # Compile proto files
+        compile_proto(Path(library_dir_path), library_dir_path, target_language=self.args.language)
 
         self._printout(
             'client libraries for service with id "{}" in org with id "{}" generated at {}'.format(library_service_id,
                                                                                                    library_org_id,
                                                                                                    library_dir_path))
```

### Comparing `snet-cli-2.1.1/snet_cli/config.py` & `snet.cli-2.1.2/snet/cli/config.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet_cli/identity.py` & `snet.cli-2.1.2/snet/cli/identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 import abc
 import json
 import struct
 import time
 import getpass
 
-from eth_account import Account
 import rlp
-
-from eth_account._utils.legacy_transactions import (
-    serializable_unsigned_transaction_from_dict,
-    encode_transaction,
-    UnsignedTransaction
-)
-
+from eth_account import Account
 from eth_account.messages import defunct_hash_message
-
+from eth_account._utils.legacy_transactions import encode_transaction, \
+    UnsignedTransaction, serializable_unsigned_transaction_from_dict
+from ledgerblue.comm import getDongle
+from ledgerblue.commException import CommException
 from trezorlib.client import TrezorClient
 from trezorlib import messages as proto
 from trezorlib.transport.hid import HidTransport
 
-from ledgerblue.comm import getDongle
-from ledgerblue.commException import CommException
 
-from snet.snet_cli.utils.utils import get_address_from_private, normalize_private_key
+from snet.cli.utils.utils import get_address_from_private, normalize_private_key
 
 BIP32_HARDEN = 0x80000000
 
 
 class IdentityProvider(abc.ABC):
     @abc.abstractmethod
     def get_address(self):
```

### Comparing `snet-cli-2.1.1/snet_cli/utils/agix2cogs.py` & `snet.cli-2.1.2/snet/cli/utils/agix2cogs.py`

 * *Files identical despite different names*

### Comparing `snet-cli-2.1.1/snet_cli/utils/config.py` & `snet.cli-2.1.2/snet/cli/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from snet.snet_cli.utils.utils import get_contract_def
+from snet.contracts import get_contract_def
 
 
 def get_contract_address(cmd, contract_name, error_message=None):
     """
     We try to get config address from the different sources.
     The order of priorioty is following:
     - command line argument (at)
```

### Comparing `snet-cli-2.1.1/snet_cli.egg-info/SOURCES.txt` & `snet.cli-2.1.2/snet.cli.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-snet/snet_cli/__init__.py
-snet/snet_cli/contract.py
-snet/snet_cli/version.py
-snet/snet_cli/metadata/__init__.py
-snet/snet_cli/metadata/organization.py
-snet/snet_cli/metadata/service.py
-snet/snet_cli/resources/package.json
-snet/snet_cli/resources/root_certificate.py
-snet/snet_cli/resources/contracts/abi/MultiPartyEscrow.json
-snet/snet_cli/resources/contracts/abi/Registry.json
-snet/snet_cli/resources/contracts/abi/SingularityNetToken.json
-snet/snet_cli/resources/contracts/networks/MultiPartyEscrow.json
-snet/snet_cli/resources/contracts/networks/Registry.json
-snet/snet_cli/resources/contracts/networks/SingularityNetToken.json
-snet/snet_cli/resources/proto/control_service.proto
-snet/snet_cli/resources/proto/control_service_pb2.py
-snet/snet_cli/resources/proto/control_service_pb2_grpc.py
-snet/snet_cli/resources/proto/merckledag.proto
-snet/snet_cli/resources/proto/merckledag_pb2.py
-snet/snet_cli/resources/proto/merckledag_pb2_grpc.py
-snet/snet_cli/resources/proto/state_service.proto
-snet/snet_cli/resources/proto/state_service_pb2.py
-snet/snet_cli/resources/proto/state_service_pb2_grpc.py
-snet/snet_cli/resources/proto/token_service.proto
-snet/snet_cli/resources/proto/token_service_pb2.py
-snet/snet_cli/resources/proto/token_service_pb2_grpc.py
-snet/snet_cli/resources/proto/training.proto
-snet/snet_cli/resources/proto/training_pb2.py
-snet/snet_cli/resources/proto/training_pb2_grpc.py
-snet/snet_cli/resources/proto/unixfs.proto
-snet/snet_cli/resources/proto/unixfs_pb2.py
-snet/snet_cli/resources/proto/unixfs_pb2_grpc.py
-snet/snet_cli/utils/__init__.py
-snet/snet_cli/utils/ipfs_utils.py
-snet/snet_cli/utils/proto_utils.py
-snet/snet_cli/utils/utils.py
-snet_cli/__init__.py
-snet_cli/arguments.py
-snet_cli/config.py
-snet_cli/identity.py
-snet_cli.egg-info/PKG-INFO
-snet_cli.egg-info/SOURCES.txt
-snet_cli.egg-info/dependency_links.txt
-snet_cli.egg-info/entry_points.txt
-snet_cli.egg-info/namespace_packages.txt
-snet_cli.egg-info/requires.txt
-snet_cli.egg-info/top_level.txt
-snet_cli/commands/__init__.py
-snet_cli/commands/commands.py
-snet_cli/commands/mpe_account.py
-snet_cli/commands/mpe_channel.py
-snet_cli/commands/mpe_client.py
-snet_cli/commands/mpe_service.py
-snet_cli/commands/mpe_treasurer.py
-snet_cli/commands/sdk_command.py
-snet_cli/utils/__init__.py
-snet_cli/utils/agix2cogs.py
-snet_cli/utils/config.py
+snet.cli.egg-info/PKG-INFO
+snet.cli.egg-info/SOURCES.txt
+snet.cli.egg-info/dependency_links.txt
+snet.cli.egg-info/entry_points.txt
+snet.cli.egg-info/namespace_packages.txt
+snet.cli.egg-info/requires.txt
+snet.cli.egg-info/top_level.txt
+snet/cli/__init__.py
+snet/cli/arguments.py
+snet/cli/config.py
+snet/cli/contract.py
+snet/cli/identity.py
+snet/cli/commands/__init__.py
+snet/cli/commands/commands.py
+snet/cli/commands/mpe_account.py
+snet/cli/commands/mpe_channel.py
+snet/cli/commands/mpe_client.py
+snet/cli/commands/mpe_service.py
+snet/cli/commands/mpe_treasurer.py
+snet/cli/commands/sdk_command.py
+snet/cli/metadata/__init__.py
+snet/cli/metadata/organization.py
+snet/cli/metadata/service.py
+snet/cli/resources/package.json
+snet/cli/resources/root_certificate.py
+snet/cli/resources/proto/control_service.proto
+snet/cli/resources/proto/control_service_pb2.py
+snet/cli/resources/proto/control_service_pb2_grpc.py
+snet/cli/resources/proto/merckledag.proto
+snet/cli/resources/proto/merckledag_pb2.py
+snet/cli/resources/proto/merckledag_pb2_grpc.py
+snet/cli/resources/proto/state_service.proto
+snet/cli/resources/proto/state_service_pb2.py
+snet/cli/resources/proto/state_service_pb2_grpc.py
+snet/cli/resources/proto/token_service.proto
+snet/cli/resources/proto/token_service_pb2.py
+snet/cli/resources/proto/token_service_pb2_grpc.py
+snet/cli/resources/proto/training.proto
+snet/cli/resources/proto/training_pb2.py
+snet/cli/resources/proto/training_pb2_grpc.py
+snet/cli/resources/proto/unixfs.proto
+snet/cli/resources/proto/unixfs_pb2.py
+snet/cli/resources/proto/unixfs_pb2_grpc.py
+snet/cli/test/functional_tests/mint/mint.py
+snet/cli/test/functional_tests/simple_daemon/test_simple_daemon.py
+snet/cli/test/unit_tests/test_mpe_service_metadata_1.py
+snet/cli/test/unit_tests/test_mpe_service_metadata_2.py
+snet/cli/utils/__init__.py
+snet/cli/utils/agix2cogs.py
+snet/cli/utils/config.py
+snet/cli/utils/ipfs_utils.py
+snet/cli/utils/proto_utils.py
+snet/cli/utils/utils.py
```


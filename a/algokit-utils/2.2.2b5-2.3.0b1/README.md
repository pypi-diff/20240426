# Comparing `tmp/algokit_utils-2.2.2b5-py3-none-any.whl.zip` & `tmp/algokit_utils-2.3.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,26 @@
-Zip file size: 46801 bytes, number of entries: 20
+Zip file size: 58581 bytes, number of entries: 24
 -rw-r--r--  2.0 unx     4963 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx    10732 b- defN 80-Jan-01 00:00 algokit_utils/_debugging.py
 -rw-r--r--  2.0 unx     6786 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     5947 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    59092 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx     7216 b- defN 80-Jan-01 00:00 algokit_utils/asset.py
+-rw-r--r--  2.0 unx     8015 b- defN 80-Jan-01 00:00 algokit_utils/beta/account_manager.py
+-rw-r--r--  2.0 unx    12649 b- defN 80-Jan-01 00:00 algokit_utils/beta/algorand_client.py
+-rw-r--r--  2.0 unx     3117 b- defN 80-Jan-01 00:00 algokit_utils/beta/client_manager.py
+-rw-r--r--  2.0 unx    28627 b- defN 80-Jan-01 00:00 algokit_utils/beta/composer.py
 -rw-r--r--  2.0 unx      812 b- defN 80-Jan-01 00:00 algokit_utils/common.py
 -rw-r--r--  2.0 unx     4279 b- defN 80-Jan-01 00:00 algokit_utils/config.py
 -rw-r--r--  2.0 unx    35110 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     5584 b- defN 80-Jan-01 00:00 algokit_utils/dispenser_api.py
 -rw-r--r--  2.0 unx     2617 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx    12803 b- defN 80-Jan-01 00:00 algokit_utils/models.py
--rw-r--r--  2.0 unx     5313 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
+-rw-r--r--  2.0 unx     5929 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-2.2.2b5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2207 b- defN 80-Jan-01 00:00 algokit_utils-2.2.2b5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-2.2.2b5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1674 b- defN 16-Jan-01 00:00 algokit_utils-2.2.2b5.dist-info/RECORD
-20 files, 181129 bytes uncompressed, 44079 bytes compressed:  75.7%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-2.3.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2207 b- defN 80-Jan-01 00:00 algokit_utils-2.3.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-2.3.0b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2044 b- defN 16-Jan-01 00:00 algokit_utils-2.3.0b1.dist-info/RECORD
+24 files, 234523 bytes uncompressed, 55275 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -18,14 +18,26 @@
 
 Filename: algokit_utils/application_specification.py
 Comment: 
 
 Filename: algokit_utils/asset.py
 Comment: 
 
+Filename: algokit_utils/beta/account_manager.py
+Comment: 
+
+Filename: algokit_utils/beta/algorand_client.py
+Comment: 
+
+Filename: algokit_utils/beta/client_manager.py
+Comment: 
+
+Filename: algokit_utils/beta/composer.py
+Comment: 
+
 Filename: algokit_utils/common.py
 Comment: 
 
 Filename: algokit_utils/config.py
 Comment: 
 
 Filename: algokit_utils/deploy.py
@@ -42,20 +54,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-2.2.2b5.dist-info/LICENSE
+Filename: algokit_utils-2.3.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-2.2.2b5.dist-info/METADATA
+Filename: algokit_utils-2.3.0b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-2.2.2b5.dist-info/WHEEL
+Filename: algokit_utils-2.3.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-2.2.2b5.dist-info/RECORD
+Filename: algokit_utils-2.3.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/network_clients.py

```diff
@@ -14,14 +14,16 @@
     "get_default_localnet_config",
     "get_indexer_client",
     "get_kmd_client_from_algod_client",
     "get_purestake_config",
     "is_localnet",
     "is_mainnet",
     "is_testnet",
+    "AlgoClientConfigs",
+    "get_kmd_client",
 ]
 
 _PURE_STAKE_HOST = "purestake.io"
 
 
 @dataclasses.dataclass
 class AlgoClientConfig:
@@ -30,14 +32,21 @@
 
     server: str
     """URL for the service e.g. `http://localhost:4001` or `https://testnet-api.algonode.cloud`"""
     token: str
     """API Token to authenticate with the service"""
 
 
+@dataclasses.dataclass
+class AlgoClientConfigs:
+    algod_config: AlgoClientConfig
+    indexer_config: AlgoClientConfig
+    kmd_config: AlgoClientConfig | None
+
+
 def get_default_localnet_config(config: Literal["algod", "indexer", "kmd"]) -> AlgoClientConfig:
     """Returns the client configuration to point to the default LocalNet"""
     port = {"algod": 4001, "indexer": 8980, "kmd": 4002}[config]
     return AlgoClientConfig(server=f"http://localhost:{port}", token="a" * 64)
 
 
 def get_algonode_config(
@@ -65,14 +74,22 @@
 
     If no configuration provided will use environment variables `ALGOD_SERVER`, `ALGOD_PORT` and `ALGOD_TOKEN`"""
     config = config or _get_config_from_environment("ALGOD")
     headers = _get_headers(config, "X-Algo-API-Token")
     return AlgodClient(config.token, config.server, headers)
 
 
+def get_kmd_client(config: AlgoClientConfig | None = None) -> KMDClient:
+    """Returns an {py:class}`algosdk.kmd.KMDClient` from `config` or environment
+
+    If no configuration provided will use environment variables `KMD_SERVER`, `KMD_PORT` and `KMD_TOKEN`"""
+    config = config or _get_config_from_environment("KMD")
+    return KMDClient(config.token, config.server)  # type: ignore[no-untyped-call]
+
+
 def get_indexer_client(config: AlgoClientConfig | None = None) -> IndexerClient:
     """Returns an {py:class}`algosdk.v2client.indexer.IndexerClient` from `config` or environment.
 
     If no configuration provided will use environment variables `INDEXER_SERVER`, `INDEXER_PORT` and `INDEXER_TOKEN`"""
     config = config or _get_config_from_environment("INDEXER")
     headers = _get_headers(config, "X-Indexer-API-Token")
     return IndexerClient(config.token, config.server, headers)  # type: ignore[no-untyped-call]
```

## Comparing `algokit_utils-2.2.2b5.dist-info/LICENSE` & `algokit_utils-2.3.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-2.2.2b5.dist-info/METADATA` & `algokit_utils-2.3.0b1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 2.2.2b5
+Version: 2.3.0b1
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-2.2.2b5.dist-info/RECORD` & `algokit_utils-2.3.0b1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 algokit_utils/_debugging.py,sha256=4UC5NZGqxF32y742TUB34rX9kWaObXCCPOs-lbkQjGQ,10732
 algokit_utils/_ensure_funded.py,sha256=ZdEdUB43QGIQrg7cSSgNrDmWaLSUhli9x9I6juwKfgo,6786
 algokit_utils/_transfer.py,sha256=CyXGOR_Zy-2crQhk-78uUbB8Sj_ZeTzxPwOAHU7wwno,5947
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
 algokit_utils/application_client.py,sha256=qylA2aI4Ecs532bIs6fyc6FgLnWey9PBzZBZW_jnYtk,59092
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/asset.py,sha256=jsc7T1dH9HZA3Yve2gRLObwUlK6xLDoQz0NxLLnqaGs,7216
+algokit_utils/beta/account_manager.py,sha256=dSb-jpBAWRfmKFYzG6T8t5vkh6ysX2NkZXl5UcZY5WA,8015
+algokit_utils/beta/algorand_client.py,sha256=y1CYYn_ADwgOLTVID9BFMvdubDgKqUfx9R6XH3PrzsA,12649
+algokit_utils/beta/client_manager.py,sha256=rW58VVBdYAV_5QwXNyt3VMP8NGon_IRhq1Dr35Mp31g,3117
+algokit_utils/beta/composer.py,sha256=qpIWQ6Xeysk1FzqW8AntHJ_go_W2qIEDB4uvGFOOdgM,28627
 algokit_utils/common.py,sha256=K6-3_9dv2clDn0WMYb8AWE_N46kWWIXglZIPfHIowDs,812
 algokit_utils/config.py,sha256=oY3o1kPzVPRiQH--f4HzrMMNPojT078CSudqS9WQaEc,4279
 algokit_utils/deploy.py,sha256=BxIFPtZd1lO8o_JmQQDIKk0O93E_bE-ZzglEWXwbefw,35110
 algokit_utils/dispenser_api.py,sha256=BpwEhKDig6qz54wbO-htG8hmLxFIrvdzXpESUb7Y1zw,5584
 algokit_utils/logic_error.py,sha256=YeE70qHZ6WBeoKCXqnto3uBg8R4ODXiNZkLmfEmASQo,2617
 algokit_utils/models.py,sha256=iJUiV6eLq5N_FKki4X5ll5rYQslU_wSPiSTtl61Z1CI,12803
-algokit_utils/network_clients.py,sha256=sj5y_g5uclddWCEyUCptA-KjWuAtLV06hZH4QIGM1yE,5313
+algokit_utils/network_clients.py,sha256=O4nJ3ECms4hFbuB1X64nzTMNOfK1Uj2oyjKxeieri-g,5929
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-2.2.2b5.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-2.2.2b5.dist-info/METADATA,sha256=8mkuN9VkBEa_Z2oH1GmzccM-SH63NFZmlBsXxc5CHQ4,2207
-algokit_utils-2.2.2b5.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-algokit_utils-2.2.2b5.dist-info/RECORD,,
+algokit_utils-2.3.0b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-2.3.0b1.dist-info/METADATA,sha256=dybj019jKMUl-xvnqX0pKgaKzNT2snOiY_APCekP21Q,2207
+algokit_utils-2.3.0b1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+algokit_utils-2.3.0b1.dist-info/RECORD,,
```


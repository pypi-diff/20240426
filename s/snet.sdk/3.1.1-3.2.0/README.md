# Comparing `tmp/snet.sdk-3.1.1.tar.gz` & `tmp/snet.sdk-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snet.sdk-3.1.1.tar", last modified: Fri Mar 15 10:48:46 2024, max compression
+gzip compressed data, was "snet.sdk-3.2.0.tar", last modified: Fri Apr 26 16:00:23 2024, max compression
```

## Comparing `snet.sdk-3.1.1.tar` & `snet.sdk-3.2.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:48:46.534368 snet.sdk-3.1.1/
--rw-r--r--   0 root         (0) root         (0)     1071 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10434 2024-03-15 10:48:46.534368 snet.sdk-3.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10079 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-15 10:48:46.534368 snet.sdk-3.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2055 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:48:46.530368 snet.sdk-3.1.1/snet/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:48:46.534368 snet.sdk-3.1.1/snet/sdk/
--rw-r--r--   0 root         (0) root         (0)     5194 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4091 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/account.py
--rw-r--r--   0 root         (0) root         (0)     3564 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/concurrency_manager.py
--rw-r--r--   0 root         (0) root         (0)     2547 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/generic_client_interceptor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:48:46.534368 snet.sdk-3.1.1/snet/sdk/metadata_provider/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/metadata_provider/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2194 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/metadata_provider/ipfs_metadata_provider.py
--rw-r--r--   0 root         (0) root         (0)      250 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/metadata_provider/metadata_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:48:46.534368 snet.sdk-3.1.1/snet/sdk/mpe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/mpe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2524 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/mpe/mpe_contract.py
--rw-r--r--   0 root         (0) root         (0)     2727 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/mpe/payment_channel.py
--rw-r--r--   0 root         (0) root         (0)     3503 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/mpe/payment_channel_provider.py
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/payment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:48:46.534368 snet.sdk-3.1.1/snet/sdk/payment_strategies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/payment_strategies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1795 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/payment_strategies/default_payment_strategy.py
--rw-r--r--   0 root         (0) root         (0)     4125 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/payment_strategies/freecall_payment_strategy.py
--rw-r--r--   0 root         (0) root         (0)     3775 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/payment_strategies/paidcall_payment_strategy.py
--rw-r--r--   0 root         (0) root         (0)      150 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/payment_strategies/payment_staregy.py
--rw-r--r--   0 root         (0) root         (0)     3351 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/payment_strategies/prepaid_payment_strategy.py
--rw-r--r--   0 root         (0) root         (0)   277625 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/root_certificate.py
--rw-r--r--   0 root         (0) root         (0)     8405 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/service_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:48:46.534368 snet.sdk-3.1.1/snet/sdk/training/
--rw-r--r--   0 root         (0) root         (0)     7951 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/training/training.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-15 10:48:29.000000 snet.sdk-3.1.1/snet/sdk/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 10:48:46.534368 snet.sdk-3.1.1/snet.sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10434 2024-03-15 10:48:46.000000 snet.sdk-3.1.1/snet.sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1044 2024-03-15 10:48:46.000000 snet.sdk-3.1.1/snet.sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 10:48:46.000000 snet.sdk-3.1.1/snet.sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-15 10:48:46.000000 snet.sdk-3.1.1/snet.sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-15 10:48:46.000000 snet.sdk-3.1.1/snet.sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-15 10:48:46.000000 snet.sdk-3.1.1/snet.sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:00:23.912613 snet.sdk-3.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5636 2024-04-26 16:00:23.912613 snet.sdk-3.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4632 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 16:00:23.912613 snet.sdk-3.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      947 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:00:23.908613 snet.sdk-3.2.0/snet/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:00:23.912613 snet.sdk-3.2.0/snet/sdk/
+-rw-r--r--   0 root         (0) root         (0)     7423 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4102 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/account.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/concurrency_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2547 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/generic_client_interceptor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:00:23.912613 snet.sdk-3.2.0/snet/sdk/metadata_provider/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/metadata_provider/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/metadata_provider/ipfs_metadata_provider.py
+-rw-r--r--   0 root         (0) root         (0)      250 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/metadata_provider/metadata_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:00:23.912613 snet.sdk-3.2.0/snet/sdk/mpe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/mpe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/mpe/mpe_contract.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/mpe/payment_channel.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/mpe/payment_channel_provider.py
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/payment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:00:23.912613 snet.sdk-3.2.0/snet/sdk/payment_strategies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/payment_strategies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/payment_strategies/default_payment_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     4122 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/payment_strategies/freecall_payment_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/payment_strategies/paidcall_payment_strategy.py
+-rw-r--r--   0 root         (0) root         (0)      150 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/payment_strategies/payment_staregy.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/payment_strategies/prepaid_payment_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     8746 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/service_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:00:23.912613 snet.sdk-3.2.0/snet/sdk/training/
+-rw-r--r--   0 root         (0) root         (0)     7946 2024-04-26 15:59:59.000000 snet.sdk-3.2.0/snet/sdk/training/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 16:00:23.912613 snet.sdk-3.2.0/snet.sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5636 2024-04-26 16:00:23.000000 snet.sdk-3.2.0/snet.sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1007 2024-04-26 16:00:23.000000 snet.sdk-3.2.0/snet.sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 16:00:23.000000 snet.sdk-3.2.0/snet.sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-26 16:00:23.000000 snet.sdk-3.2.0/snet.sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      377 2024-04-26 16:00:23.000000 snet.sdk-3.2.0/snet.sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-26 16:00:23.000000 snet.sdk-3.2.0/snet.sdk.egg-info/top_level.txt
```

### Comparing `snet.sdk-3.1.1/LICENSE` & `snet.sdk-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snet.sdk-3.1.1/snet/sdk/account.py` & `snet.sdk-3.2.0/snet/sdk/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 
-from snet.snet_cli.utils.utils import get_address_from_private, get_contract_object, normalize_private_key
+from snet.cli.utils.utils import get_address_from_private, normalize_private_key
+from snet.contracts import get_contract_object
 
 DEFAULT_GAS = 300000
 TRANSACTION_TIMEOUT = 500
 
 
 class TransactionError(Exception):
     """Raised when an Ethereum transaction receipt has a status of 0. Can provide a custom message. Optionally includes receipt"""
@@ -22,18 +23,18 @@
     def __init__(self, w3, config, mpe_contract):
         self.config = config
         self.web3 = w3
         self.mpe_contract = mpe_contract
         _token_contract_address = self.config.get("token_contract_address", None)
         if _token_contract_address is None:
             self.token_contract = get_contract_object(
-                self.web3, "SingularityNetToken.json")
+                self.web3, "SingularityNetToken")
         else:
             self.token_contract = get_contract_object(
-                self.web3, "SingularityNetToken.json", _token_contract_address)
+                self.web3, "SingularityNetToken", _token_contract_address)
 
         private_key = config.get("private_key", None)
         signer_private_key = config.get("signer_private_key", None)
         if private_key is not None:
             self.private_key = normalize_private_key(config["private_key"])
         if signer_private_key is not None:
             self.signer_private_key = normalize_private_key(
```

### Comparing `snet.sdk-3.1.1/snet/sdk/concurrency_manager.py` & `snet.sdk-3.2.0/snet/sdk/concurrency_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib
 
 import grpc
 import web3
-from snet.snet_cli.utils.utils import RESOURCES_PATH, add_to_path
+
+from snet.cli.utils.utils import RESOURCES_PATH, add_to_path
 
 
 class ConcurrencyManager:
     def __init__(self, concurrent_calls):
         self.__concurrent_calls = concurrent_calls
         self.__token = ''
         self.__planned_amount = 0
```

### Comparing `snet.sdk-3.1.1/snet/sdk/generic_client_interceptor.py` & `snet.sdk-3.2.0/snet/sdk/generic_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `snet.sdk-3.1.1/snet/sdk/metadata_provider/ipfs_metadata_provider.py` & `snet.sdk-3.2.0/snet/sdk/metadata_provider/ipfs_metadata_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from snet.snet_cli.metadata.service import mpe_service_metadata_from_json
-
-from snet.snet_cli.utils.ipfs_utils import bytesuri_to_hash, get_from_ipfs_and_checkhash
-import web3
 import json
+import web3
+
+from snet.cli.metadata.service import mpe_service_metadata_from_json
+from snet.cli.utils.ipfs_utils import bytesuri_to_hash, get_from_ipfs_and_checkhash
 
 
 class IPFSMetadataProvider(object):
 
     def __init__(self, ipfs_client, registry_contract):
         self.registry_contract = registry_contract
         self._ipfs_client = ipfs_client
```

### Comparing `snet.sdk-3.1.1/snet/sdk/mpe/mpe_contract.py` & `snet.sdk-3.2.0/snet/sdk/mpe/mpe_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from snet.snet_cli.utils.utils import get_contract_deployment_block, get_contract_object
+from snet.contracts import get_contract_deployment_block, get_contract_object
 
 
 class MPEContract:
     def __init__(self, w3, address=None):
         self.web3 = w3
         if address is None:
-            self.contract = get_contract_object(self.web3, "MultiPartyEscrow.json")
+            self.contract = get_contract_object(self.web3, "MultiPartyEscrow")
         else:
-            self.contract = get_contract_object(self.web3, "MultiPartyEscrow.json", address)
+            self.contract = get_contract_object(self.web3, "MultiPartyEscrow", address)
         self.event_topics = [self.web3.keccak(
             text="ChannelOpen(uint256,uint256,address,address,address,bytes32,uint256,uint256)").hex()]
-        self.deployment_block = get_contract_deployment_block(
-            self.web3, "MultiPartyEscrow.json")
+        self.deployment_block = get_contract_deployment_block(self.web3, "MultiPartyEscrow")
 
     def balance(self, address):
         return self.contract.functions.balances(address).call()
 
     def deposit(self, account, amount_in_cogs):
         return account.send_transaction(self.contract.functions.deposit, amount_in_cogs)
```

### Comparing `snet.sdk-3.1.1/snet/sdk/mpe/payment_channel.py` & `snet.sdk-3.2.0/snet/sdk/mpe/payment_channel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import web3
 import importlib
 from eth_account.messages import defunct_hash_message
 
-from snet.snet_cli.utils.utils import RESOURCES_PATH, add_to_path
+from snet.cli.utils.utils import RESOURCES_PATH, add_to_path
 
 
 class PaymentChannel:
-
     def __init__(self, channel_id, w3, account, payment_channel_state_service_client, mpe_contract):
         self.channel_id = channel_id
         self.web3 = w3
         self.account = account
         self.mpe_contract = mpe_contract
         self.payment_channel_state_service_client = payment_channel_state_service_client
         self.state = {
@@ -42,14 +41,25 @@
             "expiration": expiration,
             "available_amount": available_amount
         }
 
     def _get_current_channel_state(self):
         stub = self.payment_channel_state_service_client
         current_block_number = self.web3.eth.get_block("latest").number
-        message = web3.Web3.solidity_keccak(["string","address","uint256","uint256"], ["__get_channel_state",web3.Web3.to_checksum_address(self.mpe_contract.contract.address),self.channel_id,current_block_number])
+        message = web3.Web3.solidity_keccak(
+            ["string", "address", "uint256", "uint256"],
+            [
+                "__get_channel_state",
+                web3.Web3.to_checksum_address(self.mpe_contract.contract.address),
+                self.channel_id,current_block_number
+            ]
+        )
         signature = self.web3.eth.account.signHash(defunct_hash_message(message), self.account.signer_private_key).signature
         with add_to_path(str(RESOURCES_PATH.joinpath("proto"))):
             state_service_pb2 = importlib.import_module("state_service_pb2")
-        request = state_service_pb2.ChannelStateRequest(channel_id=web3.Web3.to_bytes(self.channel_id), signature=bytes(signature),current_block=current_block_number)
+        request = state_service_pb2.ChannelStateRequest(
+            channel_id=web3.Web3.to_bytes(self.channel_id),
+            signature=bytes(signature),
+            current_block=current_block_number
+        )
         response = stub.GetChannelState(request)
-        return int.from_bytes(response.current_nonce, byteorder="big"), int.from_bytes(response.current_signed_amount, byteorder="big")
+        return int.from_bytes(response.current_nonce, byteorder="big"),int.from_bytes(response.current_signed_amount, byteorder="big")
```

### Comparing `snet.sdk-3.1.1/snet/sdk/mpe/payment_channel_provider.py` & `snet.sdk-3.2.0/snet/sdk/mpe/payment_channel_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-import web3
 from web3._utils.events import get_event_data
 from eth_abi.codec import ABICodec
 
-from snet.sdk.mpe.mpe_contract import MPEContract
-
 from snet.sdk.mpe.payment_channel import PaymentChannel
-from snet.snet_cli.utils.utils import get_contract_deployment_block
+from snet.contracts import get_contract_deployment_block
 
 
 BLOCKS_PER_BATCH = 5000
 
 
 class PaymentChannelProvider(object):
-
     def __init__(self, w3, payment_channel_state_service_client, mpe_contract):
         self.web3 = w3
 
         self.mpe_contract = mpe_contract
         self.event_topics = [self.web3.keccak(
             text="ChannelOpen(uint256,uint256,address,address,address,bytes32,uint256,uint256)").hex()]
-        self.deployment_block = get_contract_deployment_block(
-            self.web3, "MultiPartyEscrow.json")
+        self.deployment_block = get_contract_deployment_block(self.web3, "MultiPartyEscrow")
         self.payment_channel_state_service_client = payment_channel_state_service_client
 
     def get_past_open_channels(self, account, payment_address, group_id, starting_block_number=0, to_block_number=None):
         if to_block_number is None:
             to_block_number = self.web3.eth.block_number
 
         if starting_block_number == 0:
@@ -37,16 +32,15 @@
         while from_block <= to_block_number:
             to_block = min(from_block + BLOCKS_PER_BATCH, to_block_number)
             logs = logs + self.web3.eth.get_logs({"fromBlock": from_block, "toBlock": to_block,
                                                  "address": self.mpe_contract.contract.address,
                                                  "topics": self.event_topics})
             from_block = to_block + 1
 
-        event_abi = self.mpe_contract.contract._find_matching_event_abi(
-            event_name="ChannelOpen")
+        event_abi = self.mpe_contract.contract._find_matching_event_abi(event_name="ChannelOpen")
         channels_opened = list(filter(
             lambda
                 channel: (channel.sender == account.address or channel.signer == account.signer_address) and channel.recipient ==
                          payment_address and channel.groupId == group_id,
 
             [get_event_data(codec, event_abi, l)["args"] for l in logs]
         ))
```

### Comparing `snet.sdk-3.1.1/snet/sdk/payment_strategies/default_payment_strategy.py` & `snet.sdk-3.2.0/snet/sdk/payment_strategies/default_payment_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from snet.sdk.concurrency_manager import ConcurrencyManager
-from snet.sdk.payment_strategies.paidcall_payment_strategy import PaidCallPaymentStrategy
 from snet.sdk.payment_strategies.freecall_payment_strategy import FreeCallPaymentStrategy
-from snet.sdk.payment_strategies.payment_staregy import PaymentStrategy
+from snet.sdk.payment_strategies.paidcall_payment_strategy import PaidCallPaymentStrategy
 from snet.sdk.payment_strategies.prepaid_payment_strategy import PrePaidPaymentStrategy
+from snet.sdk.payment_strategies.payment_staregy import PaymentStrategy
 
 
 class DefaultPaymentStrategy(PaymentStrategy):
 
     def __init__(self, concurrent_calls=1):
         self.concurrent_calls = concurrent_calls
         self.concurrencyManager = ConcurrencyManager(concurrent_calls)
@@ -35,8 +35,7 @@
 
     def get_price(self, service_client):
         pass
 
     def get_concurrency_token_and_channel(self, service_client):
         payment_strategy = PrePaidPaymentStrategy(self.concurrencyManager)
         return payment_strategy.get_concurrency_token_and_channel(service_client)
-
```

### Comparing `snet.sdk-3.1.1/snet/sdk/payment_strategies/freecall_payment_strategy.py` & `snet.sdk-3.2.0/snet/sdk/payment_strategies/freecall_payment_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import importlib
 from urllib.parse import urlparse
 
 import grpc
 import web3
+from snet.cli.resources.root_certificate import certificate
+from snet.cli.utils.utils import RESOURCES_PATH, add_to_path
+
 from snet.sdk.payment_strategies.payment_staregy import PaymentStrategy
-from snet.snet_cli.utils.utils import RESOURCES_PATH, add_to_path
-from snet.sdk.root_certificate import root_certificate
+
 
 class FreeCallPaymentStrategy(PaymentStrategy):
 
     def is_free_call_available(self, service_client):
         try:
             org_id, service_id, group_id, daemon_endpoint = service_client.get_service_details()
             email, token_for_free_call, token_expiry_date_block = service_client.get_free_call_config()
@@ -36,15 +38,15 @@
                 channel_endpoint = endpoint_object.hostname + ":" + str(endpoint_object.port)
             else:
                 channel_endpoint = endpoint_object.hostname
 
             if endpoint_object.scheme == "http":
                 channel = grpc.insecure_channel(channel_endpoint)
             elif endpoint_object.scheme == "https":
-                channel = grpc.secure_channel(channel_endpoint, grpc.ssl_channel_credentials(root_certificates=root_certificate))
+                channel = grpc.secure_channel(channel_endpoint, grpc.ssl_channel_credentials(root_certificates=certificate))
             else:
                 raise ValueError('Unsupported scheme in service metadata ("{}")'.format(endpoint_object.scheme))
 
             stub = state_service_pb2_grpc.FreeCallStateServiceStub(channel)
             response = stub.GetFreeCallsAvailable(request)
             if response.free_calls_available > 0:
                 return True
```

### Comparing `snet.sdk-3.1.1/snet/sdk/payment_strategies/paidcall_payment_strategy.py` & `snet.sdk-3.2.0/snet/sdk/payment_strategies/paidcall_payment_strategy.py`

 * *Files identical despite different names*

### Comparing `snet.sdk-3.1.1/snet/sdk/payment_strategies/prepaid_payment_strategy.py` & `snet.sdk-3.2.0/snet/sdk/payment_strategies/prepaid_payment_strategy.py`

 * *Files identical despite different names*

### Comparing `snet.sdk-3.1.1/snet/sdk/service_client.py` & `snet.sdk-3.2.0/snet/sdk/service_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 import collections
 import importlib
 
 import grpc
 import web3
 from eth_account.messages import defunct_hash_message
 from rfc3986 import urlparse
+from snet.cli.resources.root_certificate import certificate
+from snet.cli.utils.utils import RESOURCES_PATH, add_to_path
 
 import snet.sdk.generic_client_interceptor as generic_client_interceptor
 from snet.sdk.mpe.payment_channel_provider import PaymentChannelProvider
-from snet.sdk.root_certificate import root_certificate
-from snet.snet_cli.utils.utils import RESOURCES_PATH, add_to_path
 
 
 class _ClientCallDetails(
     collections.namedtuple(
         '_ClientCallDetails',
         ('method', 'timeout', 'metadata', 'credentials')),
     grpc.ClientCallDetails):
     pass
 
 
 class ServiceClient:
     def __init__(self, org_id, service_id, service_metadata, group, service_stub, payment_strategy,
-                 options, mpe_contract, account, sdk_web3):
+                 options, mpe_contract, account, sdk_web3, pb2_module):
         self.org_id = org_id
         self.service_id = service_id
         self.options = options
         self.group = group
         self.service_metadata = service_metadata
 
         self.payment_strategy = payment_strategy
@@ -35,20 +35,26 @@
         self.__base_grpc_channel = self._get_grpc_channel()
         self.grpc_channel = grpc.intercept_channel(self.__base_grpc_channel,
                                                    generic_client_interceptor.create(self._intercept_call))
         self.payment_channel_provider = PaymentChannelProvider(sdk_web3,
                                                                self._generate_payment_channel_state_service_client(),
                                                                mpe_contract)
         self.service = self._generate_grpc_stub(service_stub)
+        self.pb2_module = importlib.import_module(pb2_module) if isinstance(pb2_module, str) else pb2_module
         self.payment_channels = []
         self.last_read_block = 0
         self.account = account
         self.sdk_web3 = sdk_web3
         self.mpe_address = mpe_contract.contract.address
 
+    def call_rpc(self, rpc_name: str, message_class: str, **kwargs):
+        rpc_method = getattr(self.service, rpc_name)
+        request = getattr(self.pb2_module, message_class)(**kwargs)
+        return rpc_method(request)
+
     def _get_payment_expiration_threshold_for_group(self):
         pass
 
     def _generate_grpc_stub(self, service_stub):
         grpc_channel = self.__base_grpc_channel
         disable_blockchain_operations = self.options.get("disable_blockchain_operations", False)
         if disable_blockchain_operations is False:
@@ -69,15 +75,15 @@
         else:
             channel_endpoint = endpoint_object.hostname
 
         if endpoint_object.scheme == "http":
             return grpc.insecure_channel(channel_endpoint)
         elif endpoint_object.scheme == "https":
             return grpc.secure_channel(channel_endpoint,
-                                       grpc.ssl_channel_credentials(root_certificates=root_certificate))
+                                       grpc.ssl_channel_credentials(root_certificates=certificate))
         else:
             raise ValueError('Unsupported scheme in service metadata ("{}")'.format(endpoint_object.scheme))
 
     def _get_service_call_metadata(self):
         metadata = self.payment_strategy.get_payment_metadata(self)
         return metadata
 
@@ -178,8 +184,8 @@
         return self.options.get('concurrency', True)
 
     def get_concurrency_token_and_channel(self):
         return self.payment_strategy.get_concurrency_token_and_channel(self)
 
     def set_concurrency_token_and_channel(self, token, channel):
         self.payment_strategy.concurrency_token = token
-        self.payment_strategy.channel = channel
+        self.payment_strategy.channel = channel
```

### Comparing `snet.sdk-3.1.1/snet/sdk/training/training.py` & `snet.sdk-3.2.0/snet/sdk/training/training.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import enum
 import importlib
 from urllib.parse import urlparse
 
 import grpc
 import web3
 
-from snet.sdk.root_certificate import root_certificate
-from snet.snet_cli.utils.utils import RESOURCES_PATH, add_to_path
+from snet.cli.resources.root_certificate import certificate
+from snet.cli.utils.utils import add_to_path, RESOURCES_PATH
 
 
 # for local debug
 # from snet.snet_cli.resources.proto import training_pb2_grpc
 # from snet.snet_cli.resources.proto import training_pb2
 
 
@@ -42,15 +42,15 @@
             channel_endpoint = endpoint_object.hostname
 
         if endpoint_object.scheme == "http":
             print("creating http channel: ", channel_endpoint)
             channel = grpc.insecure_channel(channel_endpoint)
         elif endpoint_object.scheme == "https":
             channel = grpc.secure_channel(channel_endpoint,
-                                          grpc.ssl_channel_credentials(root_certificates=root_certificate))
+                                          grpc.ssl_channel_credentials(root_certificates=certificate))
         else:
             raise ValueError('Unsupported scheme in service metadata ("{}")'.format(endpoint_object.scheme))
 
         current_block_number = service_client.get_current_block_number()
         signature = service_client.generate_training_signature(msg.value, web3.Web3.to_checksum_address(
             service_client.account.address), current_block_number)
         auth_req = self.training_pb2.AuthorizationDetails(signature=bytes(signature),
```

### Comparing `snet.sdk-3.1.1/snet.sdk.egg-info/SOURCES.txt` & `snet.sdk-3.2.0/snet.sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 snet.sdk.egg-info/PKG-INFO
 snet.sdk.egg-info/SOURCES.txt
 snet.sdk.egg-info/dependency_links.txt
 snet.sdk.egg-info/namespace_packages.txt
 snet.sdk.egg-info/requires.txt
 snet.sdk.egg-info/top_level.txt
 snet/sdk/__init__.py
 snet/sdk/account.py
 snet/sdk/concurrency_manager.py
 snet/sdk/generic_client_interceptor.py
 snet/sdk/payment.py
-snet/sdk/root_certificate.py
 snet/sdk/service_client.py
-snet/sdk/version.py
 snet/sdk/metadata_provider/__init__.py
 snet/sdk/metadata_provider/ipfs_metadata_provider.py
 snet/sdk/metadata_provider/metadata_provider.py
 snet/sdk/mpe/__init__.py
 snet/sdk/mpe/mpe_contract.py
 snet/sdk/mpe/payment_channel.py
 snet/sdk/mpe/payment_channel_provider.py
```


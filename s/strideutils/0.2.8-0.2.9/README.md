# Comparing `tmp/strideutils-0.2.8.tar.gz` & `tmp/strideutils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strideutils-0.2.8.tar", max compression
+gzip compressed data, was "strideutils-0.2.9.tar", max compression
```

## Comparing `strideutils-0.2.8.tar` & `strideutils-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1835 2024-04-25 17:35:49.280978 strideutils-0.2.8/README.md
--rw-r--r--   0        0        0      709 2024-04-25 17:35:49.280978 strideutils-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      373 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/Makefile
--rw-r--r--   0        0        0        0 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/coingecko.py
--rw-r--r--   0        0        0     5267 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/config_examples/strideutils_config.yaml.example
--rw-r--r--   0        0        0      443 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/config_examples/strideutils_secrets.yaml.example
--rw-r--r--   0        0        0     1270 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/cryptography.py
--rw-r--r--   0        0        0     1835 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/exec_tx.py
--rw-r--r--   0        0        0     1669 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/invariant_helpers.py
--rw-r--r--   0        0        0     1509 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/run_safely.py
--rw-r--r--   0        0        0     6793 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/sheets_connector.py
--rw-r--r--   0        0        0     1512 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/slack_connector.py
--rw-r--r--   0        0        0     5509 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/stride_alerts.py
--rw-r--r--   0        0        0    10449 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/stride_config.py
--rw-r--r--   0        0        0    32831 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/stride_requests.py
--rw-r--r--   0        0        0     2438 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/stride_upstash.py
--rw-r--r--   0        0        0     1064 2024-04-25 17:35:49.280978 strideutils-0.2.8/strideutils/twilio_connector.py
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1835 2024-04-26 19:50:03.632984 strideutils-0.2.9/README.md
+-rw-r--r--   0        0        0      709 2024-04-26 19:50:03.632984 strideutils-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/Makefile
+-rw-r--r--   0        0        0        0 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/coingecko.py
+-rw-r--r--   0        0        0     5267 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/config_examples/strideutils_config.yaml.example
+-rw-r--r--   0        0        0      443 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/config_examples/strideutils_secrets.yaml.example
+-rw-r--r--   0        0        0     1270 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/cryptography.py
+-rw-r--r--   0        0        0     1835 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/exec_tx.py
+-rw-r--r--   0        0        0     1669 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/invariant_helpers.py
+-rw-r--r--   0        0        0     1509 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/run_safely.py
+-rw-r--r--   0        0        0     6793 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/sheets_connector.py
+-rw-r--r--   0        0        0     1512 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/slack_connector.py
+-rw-r--r--   0        0        0     5509 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/stride_alerts.py
+-rw-r--r--   0        0        0    10449 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/stride_config.py
+-rw-r--r--   0        0        0    33566 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/stride_requests.py
+-rw-r--r--   0        0        0     2438 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/stride_upstash.py
+-rw-r--r--   0        0        0     1064 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/twilio_connector.py
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.2.9/PKG-INFO
```

### Comparing `strideutils-0.2.8/README.md` & `strideutils-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/pyproject.toml` & `strideutils-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strideutils"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 google-api-python-client = ">=2.100.0"
```

### Comparing `strideutils-0.2.8/strideutils/coingecko.py` & `strideutils-0.2.9/strideutils/coingecko.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/config_examples/strideutils_config.yaml.example` & `strideutils-0.2.9/strideutils/config_examples/strideutils_config.yaml.example`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/cryptography.py` & `strideutils-0.2.9/strideutils/cryptography.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/exec_tx.py` & `strideutils-0.2.9/strideutils/exec_tx.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/invariant_helpers.py` & `strideutils-0.2.9/strideutils/invariant_helpers.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/run_safely.py` & `strideutils-0.2.9/strideutils/run_safely.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/sheets_connector.py` & `strideutils-0.2.9/strideutils/sheets_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/slack_connector.py` & `strideutils-0.2.9/strideutils/slack_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/stride_alerts.py` & `strideutils-0.2.9/strideutils/stride_alerts.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/stride_config.py` & `strideutils-0.2.9/strideutils/stride_config.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/stride_requests.py` & `strideutils-0.2.9/strideutils/stride_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 ACCOUNT_QUERY = "cosmos/auth/v1beta1/accounts/{address}"
 ACCOUNT_BALANCE_QUERY = "cosmos/bank/v1beta1/balances/{address}"
 ACCOUNT_DELEGATIONS_QUERY = "cosmos/staking/v1beta1/delegations/{delegator_address}"
 ACCOUNT_UNBONDINGS_QUERY = "cosmos/staking/v1beta1/delegators/{delegator_address}/unbonding_delegations"
 MODULE_ACCOUNTS_QUERY = "cosmos/auth/v1beta1/module_accounts"
 SUPPLY_QUERY = "cosmos/bank/v1beta1/supply/by_denom"
+VALIDATORS_QUERY = "cosmos/staking/v1beta1/validators"
+VALIDATOR_SLASHES_QUERY = "cosmos/distribution/v1beta1/validators/{validator_address}/slashes"
 
 CONNECTION_QUERY = "ibc/core/connection/v1/connections/{connection_id}"
 CHANNELS_QUERY = "ibc/core/channel/v1/connections/{connection_id}/channels"
 CHANNEL_QUERY = "ibc/core/channel/v1/channels/{channel_id}/ports/{port_id}"
 
 TXS_QUERY = "cosmos/tx/v1beta1/txs"
 TX_BY_ACCOUNT_EVENT = "tx.acc_seq='{address}/{sequence}'"
@@ -97,25 +99,26 @@
 
 
 def query_list_with_pagination(
     endpoint: str,
     rel_key: str,
     block_height: int = 0,
     max_pages: int = 50,
+    params: Union[dict, List[Tuple[str, str]]] = {},
 ) -> List[Dict]:
     """
     Query a list with pagination
     Returns the concatenated list from all the responses
     """
     data = []
     query_url = endpoint
     query_count = 0
 
     while True:
-        res = request(url=query_url, block_height=block_height)
+        res = request(url=query_url, block_height=block_height, params=params)
         data += res[rel_key]
 
         query_count += 1
         if query_count >= max_pages:
             print(f"Max pages {max_pages} reached - results are truncated")
             break
 
@@ -389,24 +392,33 @@
              'channel_value': '15104662663116448541290611'}}, ...]
     """
     endpoint = f"{config.stride.api_endpoint}/{RATE_LIMIT_QUERY}"
     host_zone = request(endpoint, **kwargs)["rate_limits"]
     return host_zone
 
 
-def get_validators(
-    api_endpoint: str = config.stride.api_endpoint,
-) -> List[Dict[str, Any]]:
+def get_validators(api_endpoint: str = config.stride.api_endpoint) -> List[Dict[str, Any]]:
     """
     Queries the list of validators from a chain
     """
-    url = f"{api_endpoint}/cosmos/staking/v1beta1/validators"
+    url = f"{api_endpoint}/{VALIDATORS_QUERY}"
     return query_list_with_pagination(url, rel_key="validators")
 
 
+def get_validator_slashes(api_endpoint: str, validator_address: str) -> List[Dict[str, str]]:
+    """
+    Queries the list of all slashes for a particular validator
+    The start and end heights are required with the query
+    An arbitrarily large end height to get all slashes
+    """
+    url = f"{api_endpoint}/{VALIDATOR_SLASHES_QUERY.format(validator_address=validator_address)}"
+    params = {"starting_height": "0", "ending_height": "10000000000000000"}
+    return query_list_with_pagination(url, rel_key="slashes", params=params)
+
+
 def get_redemption_rate(token: str) -> float:
     """
     Queries the redemption rate for a particular token
     """
     js = get_host_zone_json(config.get_chain(ticker=token).id)
     return float(js["redemption_rate"])
```

### Comparing `strideutils-0.2.8/strideutils/stride_upstash.py` & `strideutils-0.2.9/strideutils/stride_upstash.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/strideutils/twilio_connector.py` & `strideutils-0.2.9/strideutils/twilio_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.8/PKG-INFO` & `strideutils-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strideutils
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


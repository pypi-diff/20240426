# Comparing `tmp/trio_bybit-0.1.4.tar.gz` & `tmp/trio_bybit-0.1.5.tar.gz`

## Comparing `trio_bybit-0.1.4.tar` & `trio_bybit-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/pytest.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/tests/test_async_client.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/tests/test_streams.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/trio_bybit/__init__.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/trio_bybit/client.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/trio_bybit/enums.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/trio_bybit/exceptions.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/trio_bybit/helpers.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/trio_bybit/streams.py
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/LICENSE
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/README.md
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 trio_bybit-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/pytest.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/tests/test_async_client.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/tests/test_streams.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/__init__.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/client.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/enums.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/exceptions.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/helpers.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/streams.py
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/LICENSE
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/README.md
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/PKG-INFO
```

### Comparing `trio_bybit-0.1.4/tests/test_async_client.py` & `trio_bybit-0.1.5/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.4/tests/test_streams.py` & `trio_bybit-0.1.5/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.4/trio_bybit/client.py` & `trio_bybit-0.1.5/trio_bybit/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,23 @@
 
     async def get_symbol_info(self, **kwargs) -> dict:
         return await self._get("market/instruments-info", **kwargs)
 
     async def get_orderbook(self, **kwargs) -> dict:
         return await self._get("market/orderbook", **kwargs)
 
+    async def get_klines(self, **kwargs) -> dict:
+        return await self._get("market/kline", **kwargs)
+
+    async def get_funding_history(self, **kwargs) -> dict:
+        return await self._get("market/funding/history", **kwargs)
+
+    async def get_ticker(self, **kwargs) -> dict:
+        return await self._get("market/tickers", **kwargs)
+
     async def place_order(self, **kwargs) -> dict:
         return await self._post("order/create", **kwargs, signed=True)
 
     async def amend_order(self, **kwargs) -> dict:
         return await self._post("order/amend", **kwargs, signed=True)
 
     async def cancel_order(self, **kwargs) -> dict:
```

### Comparing `trio_bybit-0.1.4/trio_bybit/exceptions.py` & `trio_bybit-0.1.5/trio_bybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.4/trio_bybit/helpers.py` & `trio_bybit-0.1.5/trio_bybit/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.4/trio_bybit/streams.py` & `trio_bybit-0.1.5/trio_bybit/streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,25 @@
         "test": {
             "spot": "wss://stream-testnet.bybit.com/v5/public/spot",
             "linear": "wss://stream-testnet.bybit.com/v5/public/linear",
             "inverse": "wss://stream-testnet.bybit.com/v5/public/inverse",
             "private": "wss://stream-testnet.bybit.com/v5/private",
         },
         "demo": {
-            "private":  "wss://stream-demo.bybit.com",
-        }
+            "private": "wss://stream-demo.bybit.com",
+        },
     }
 
-    def __init__(self, endpoint: str = "spot", api_key: str | None = None, api_secret: str | None = None, alternative_net: str = ""):
+    def __init__(
+        self,
+        endpoint: str = "spot",
+        api_key: str | None = None,
+        api_secret: str | None = None,
+        alternative_net: str = "",
+    ):
         self.ws: trio_websocket.WebSocketConnection | None = None
         self.endpoint: str = endpoint
         self.alternative_net: str = alternative_net if alternative_net else "main"
         if self.endpoint == "private" and (api_key is None or api_secret is None):
             raise ValueError("api_key and api_secret must be provided for private streams")
         self.api_key = api_key
         self.api_secret = api_secret
```

### Comparing `trio_bybit-0.1.4/.gitignore` & `trio_bybit-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.4/LICENSE` & `trio_bybit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.4/README.md` & `trio_bybit-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.4/pyproject.toml` & `trio_bybit-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trio-bybit"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python bybit async SDK based on trio."
 authors = [
     { name = "Shu Wang", email = "halfelf.ronin@gmail.com" }
 ]
 dependencies = [
     "trio>=0.25.0",
     "httpx[http2]>=0.27.0",
```

### Comparing `trio_bybit-0.1.4/PKG-INFO` & `trio_bybit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trio-bybit
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python bybit async SDK based on trio.
 Project-URL: Repository, https://github.com/halfelf/trio-bybit
 Author-email: Shu Wang <halfelf.ronin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shu Wang <halfelf.ronin@gmail.com>
```


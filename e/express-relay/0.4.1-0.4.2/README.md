# Comparing `tmp/express_relay-0.4.1.tar.gz` & `tmp/express_relay-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express_relay-0.4.1.tar", max compression
+gzip compressed data, was "express_relay-0.4.2.tar", max compression
```

## Comparing `express_relay-0.4.1.tar` & `express_relay-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      949 2024-04-22 16:47:08.169835 express_relay-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-04-22 16:47:08.169835 express_relay-0.4.1/express_relay/__init__.py
--rw-r--r--   0        0        0    17136 2024-04-22 16:47:08.169835 express_relay-0.4.1/express_relay/client.py
--rw-r--r--   0        0        0     9468 2024-04-22 16:47:08.169835 express_relay-0.4.1/express_relay/express_relay_types.py
--rw-r--r--   0        0        0     5174 2024-04-22 16:47:08.169835 express_relay-0.4.1/express_relay/searcher/examples/simple_searcher.py
--rw-r--r--   0        0        0      612 2024-04-22 16:47:08.173835 express_relay-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 express_relay-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      949 2024-04-26 12:32:02.467973 express_relay-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 12:32:02.467973 express_relay-0.4.2/express_relay/__init__.py
+-rw-r--r--   0        0        0    17136 2024-04-26 12:32:02.467973 express_relay-0.4.2/express_relay/client.py
+-rw-r--r--   0        0        0     9559 2024-04-26 12:32:02.467973 express_relay-0.4.2/express_relay/express_relay_types.py
+-rw-r--r--   0        0        0     5045 2024-04-26 12:32:02.467973 express_relay-0.4.2/express_relay/searcher/examples/simple_searcher.py
+-rw-r--r--   0        0        0      612 2024-04-26 12:32:02.471973 express_relay-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 express_relay-0.4.2/PKG-INFO
```

### Comparing `express_relay-0.4.1/README.md` & `express_relay-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `express_relay-0.4.1/express_relay/client.py` & `express_relay-0.4.2/express_relay/client.py`

 * *Files identical despite different names*

### Comparing `express_relay-0.4.1/express_relay/express_relay_types.py` & `express_relay-0.4.2/express_relay/express_relay_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,33 +101,37 @@
     permission_key: HexString
 
 
 class BidStatus(Enum):
     SUBMITTED = "submitted"
     LOST = "lost"
     PENDING = "pending"
+    SIMULATION_FAILED = "simulation_failed"
 
 
 class BidStatusUpdate(BaseModel):
     """
     Attributes:
         id: The ID of the bid.
-        bid_status: The status enum, either SUBMITTED, LOST, or PENDING.
+        bid_status: The current status of the bid.
         result: The result of the bid: a transaction hash if the status is SUBMITTED or LOST, else None.
         index: The index of the bid in the submitted transaction; None if the status is not SUBMITTED.
     """
 
     id: UUIDString
     bid_status: BidStatus
     result: Bytes32 | None = Field(default=None)
     index: int | None = Field(default=None)
 
     @model_validator(mode="after")
     def check_result(self):
-        if self.bid_status == BidStatus("pending"):
+        if self.bid_status in [
+            BidStatus("pending"),
+            BidStatus("simulation_failed"),
+        ]:
             assert self.result is None, "result must be None"
         else:
             assert self.result is not None, "result must be a valid 32-byte hash"
         return self
 
     @model_validator(mode="after")
     def check_index(self):
```

### Comparing `express_relay-0.4.1/express_relay/searcher/examples/simple_searcher.py` & `express_relay-0.4.2/express_relay/searcher/examples/simple_searcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,26 +72,24 @@
         Args:
             bid_status_update: An object representing an update to the status of a bid.
         """
         id = bid_status_update.id
         bid_status = bid_status_update.bid_status
         result = bid_status_update.result
 
+        result_details = ""
         if bid_status == BidStatus("submitted"):
-            logger.info(
-                f"Bid {id} has been submitted in transaction {result} at index {bid_status_update.index} of the multicall"
+            result_details = (
+                f", transaction {result}, index {bid_status_update.index} of multicall"
             )
         elif bid_status == BidStatus("lost"):
-            logger.info(
-                f"Bid {id} was unsuccessful, not included in transaction {result}"
-            )
-        elif bid_status == BidStatus("pending"):
-            logger.info(f"Bid {id} is pending")
-        else:
-            logger.error(f"Unrecognized status {bid_status} for bid {id}")
+            result_details = f", transaction {result}"
+        logger.error(
+            f"Bid status for bid {id}: {bid_status.value.replace('_', ' ')}{result_details}"
+        )
 
 
 async def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument(
         "--private-key",
```

### Comparing `express_relay-0.4.1/pyproject.toml` & `express_relay-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "express-relay"
-version = "0.4.1"
+version = "0.4.2"
 description = "Utilities for searchers and protocols to interact with the Express Relay protocol."
 authors = ["dourolabs"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `express_relay-0.4.1/PKG-INFO` & `express_relay-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-relay
-Version: 0.4.1
+Version: 0.4.2
 Summary: Utilities for searchers and protocols to interact with the Express Relay protocol.
 License: Proprietary
 Author: dourolabs
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


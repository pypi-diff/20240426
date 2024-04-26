# Comparing `tmp/izihawa_trident_client-1.3.3.tar.gz` & `tmp/izihawa_trident_client-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_trident_client-1.3.3.tar", max compression
+gzip compressed data, was "izihawa_trident_client-1.3.4.tar", max compression
```

## Comparing `izihawa_trident_client-1.3.3.tar` & `izihawa_trident_client-1.3.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.3/README.md
--rw-r--r--   0        0        0      423 2024-04-26 19:52:25.443364 izihawa_trident_client-1.3.3/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.3/trident/__init__.py
--rw-r--r--   0        0        0      721 2024-04-26 19:24:10.303987 izihawa_trident_client-1.3.3/trident/cli.py
--rw-r--r--   0        0        0     6323 2024-04-26 19:49:12.841636 izihawa_trident_client-1.3.3/trident/client.py
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-10 19:54:01.661696 izihawa_trident_client-1.3.4/README.md
+-rw-r--r--   0        0        0      423 2024-04-26 19:54:44.950924 izihawa_trident_client-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-26 19:52:25.445233 izihawa_trident_client-1.3.4/trident/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-26 19:54:39.941952 izihawa_trident_client-1.3.4/trident/cli.py
+-rw-r--r--   0        0        0     6323 2024-04-26 19:49:12.841636 izihawa_trident_client-1.3.4/trident/client.py
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 izihawa_trident_client-1.3.4/PKG-INFO
```

### Comparing `izihawa_trident_client-1.3.3/trident/cli.py` & `izihawa_trident_client-1.3.4/trident/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 import fire
 from termcolor import colored
 
 from trident import TridentClient
 
 
-async def client_cli(endpoint: str = '127.0.0.1:7080'):
+async def client_cli(base_url: str = 'http://127.0.0.1', timeout: float = 3.0):
     try:
-        client = TridentClient(endpoint=endpoint, connection_timeout=3.0)
+        client = TridentClient(base_url=base_url, timeout=timeout)
         await client.start()
         print(f"{colored('SERVER_RESPONDED', 'green')}:", file=sys.stderr)
         return client.get_interface()
     except asyncio.exceptions.TimeoutError:
         # ToDo: process exception through fire.core.FireError
-        print(f"{colored('ERROR', 'red')}: {endpoint} timeout", file=sys.stderr)
+        print(f"{colored('ERROR', 'red')}: {base_url} timeout", file=sys.stderr)
         sys.exit(1)
 
 
 def main():
     fire.Fire(client_cli, name='trident-client')
```

### Comparing `izihawa_trident_client-1.3.3/trident/client.py` & `izihawa_trident_client-1.3.4/trident/client.py`

 * *Files identical despite different names*

### Comparing `izihawa_trident_client-1.3.3/PKG-INFO` & `izihawa_trident_client-1.3.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izihawa-trident-client
-Version: 1.3.3
+Version: 1.3.4
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


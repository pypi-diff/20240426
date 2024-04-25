# Comparing `tmp/tastytrade-7.1.tar.gz` & `tmp/tastytrade-7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-7.1.tar", last modified: Fri Apr 19 04:30:20 2024, max compression
+gzip compressed data, was "tastytrade-7.2.tar", last modified: Thu Apr 25 22:34:21 2024, max compression
```

## Comparing `tastytrade-7.1.tar` & `tastytrade-7.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.329897 tastytrade-7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 04:30:15.000000 tastytrade-7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-19 04:30:20.329897 tastytrade-7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-19 04:30:15.000000 tastytrade-7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 04:30:20.329897 tastytrade-7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-19 04:30:15.000000 tastytrade-7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.325897 tastytrade-7.1/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38112 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.325897 tastytrade-7.1/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/timeandsale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/dxfeed/underlying.py
--rw-r--r--   0 runner    (1001) docker     (127)    35007 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-19 04:30:15.000000 tastytrade-7.1/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.329897 tastytrade-7.1/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 04:30:20.000000 tastytrade-7.1/tastytrade.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:30:20.329897 tastytrade-7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_instruments.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-19 04:30:15.000000 tastytrade-7.1/tests/test_watchlists.py
+drwxr-xr-x   0 graeme    (1000) graeme    (1000)        0 2024-04-25 22:34:21.754979 tastytrade-7.2/
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1072 2024-01-31 16:29:22.000000 tastytrade-7.2/LICENSE
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     8297 2024-04-25 22:34:21.754979 tastytrade-7.2/PKG-INFO
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     7844 2024-04-19 03:18:48.000000 tastytrade-7.2/README.rst
+-rw-r--r--   0 graeme    (1000) graeme    (1000)       38 2024-04-25 22:34:21.754979 tastytrade-7.2/setup.cfg
+-rw-r--r--   0 graeme    (1000) graeme    (1000)      720 2024-04-25 22:24:26.000000 tastytrade-7.2/setup.py
+drwxr-xr-x   0 graeme    (1000) graeme    (1000)        0 2024-04-25 22:34:21.751645 tastytrade-7.2/tastytrade/
+-rw-r--r--   0 graeme    (1000) graeme    (1000)      671 2024-04-25 22:24:17.000000 tastytrade-7.2/tastytrade/__init__.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)    38112 2024-04-19 03:18:48.000000 tastytrade-7.2/tastytrade/account.py
+drwxr-xr-x   0 graeme    (1000) graeme    (1000)        0 2024-04-25 22:34:21.754979 tastytrade-7.2/tastytrade/dxfeed/
+-rw-r--r--   0 graeme    (1000) graeme    (1000)      485 2024-04-19 03:23:07.000000 tastytrade-7.2/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1499 2024-04-25 21:39:03.000000 tastytrade-7.2/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1763 2024-04-19 03:23:31.000000 tastytrade-7.2/tastytrade/dxfeed/event.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1203 2024-02-09 19:59:36.000000 tastytrade-7.2/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1962 2024-02-09 19:59:50.000000 tastytrade-7.2/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)      973 2024-02-09 19:59:21.000000 tastytrade-7.2/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1717 2024-03-07 01:25:51.000000 tastytrade-7.2/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1213 2024-02-09 19:59:26.000000 tastytrade-7.2/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     2021 2024-02-09 19:59:41.000000 tastytrade-7.2/tastytrade/dxfeed/timeandsale.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1503 2024-02-09 20:00:01.000000 tastytrade-7.2/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1351 2024-02-09 19:59:56.000000 tastytrade-7.2/tastytrade/dxfeed/underlying.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)    35007 2024-04-19 03:18:48.000000 tastytrade-7.2/tastytrade/instruments.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     6472 2024-04-19 03:18:48.000000 tastytrade-7.2/tastytrade/metrics.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)    13110 2024-04-04 18:36:32.000000 tastytrade-7.2/tastytrade/order.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1123 2024-04-19 03:18:48.000000 tastytrade-7.2/tastytrade/search.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     7624 2024-04-25 22:23:44.000000 tastytrade-7.2/tastytrade/session.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)    23601 2024-04-19 04:07:21.000000 tastytrade-7.2/tastytrade/streamer.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     6979 2024-04-04 18:36:32.000000 tastytrade-7.2/tastytrade/utils.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     6913 2024-04-19 03:18:48.000000 tastytrade-7.2/tastytrade/watchlists.py
+drwxr-xr-x   0 graeme    (1000) graeme    (1000)        0 2024-04-25 22:34:21.754979 tastytrade-7.2/tastytrade.egg-info/
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     8297 2024-04-25 22:34:21.000000 tastytrade-7.2/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 graeme    (1000) graeme    (1000)      901 2024-04-25 22:34:21.000000 tastytrade-7.2/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 graeme    (1000) graeme    (1000)        1 2024-04-25 22:34:21.000000 tastytrade-7.2/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 graeme    (1000) graeme    (1000)       99 2024-04-25 22:34:21.000000 tastytrade-7.2/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 graeme    (1000) graeme    (1000)       11 2024-04-25 22:34:21.000000 tastytrade-7.2/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 graeme    (1000) graeme    (1000)        0 2024-04-25 22:34:21.754979 tastytrade-7.2/tests/
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     6054 2024-04-19 03:18:48.000000 tastytrade-7.2/tests/test_account.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     2627 2024-02-07 15:52:45.000000 tastytrade-7.2/tests/test_instruments.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)      472 2024-01-31 16:29:22.000000 tastytrade-7.2/tests/test_metrics.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)      270 2024-04-19 03:18:48.000000 tastytrade-7.2/tests/test_session.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1149 2024-01-31 16:29:22.000000 tastytrade-7.2/tests/test_streamer.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     3983 2024-02-29 18:01:23.000000 tastytrade-7.2/tests/test_utils.py
+-rw-r--r--   0 graeme    (1000) graeme    (1000)     1379 2024-01-31 16:29:22.000000 tastytrade-7.2/tests/test_watchlists.py
```

### Comparing `tastytrade-7.1/LICENSE` & `tastytrade-7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/PKG-INFO` & `tastytrade-7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 7.1
+Version: 7.2
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `tastytrade-7.1/README.rst` & `tastytrade-7.2/README.rst`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/setup.py` & `tastytrade-7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 f = open('README.rst', 'r')
 LONG_DESCRIPTION = f.read()
 f.close()
 
 setup(
     name='tastytrade',
-    version='7.1',
+    version='7.2',
     description='An unofficial SDK for Tastytrade!',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
     author='Graeme Holliday',
     author_email='graeme.holliday@pm.me',
     url='https://github.com/tastyware/tastytrade',
     license='MIT',
```

### Comparing `tastytrade-7.1/tastytrade/__init__.py` & `tastytrade-7.2/tastytrade/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 API_URL = 'https://api.tastyworks.com'
 CERT_URL = 'https://api.cert.tastyworks.com'
-VERSION = '7.1'
+VERSION = '7.2'
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 from .account import Account  # noqa: E402
 from .search import symbol_search  # noqa: E402
 from .session import CertificationSession, ProductionSession  # noqa: E402
```

### Comparing `tastytrade-7.1/tastytrade/account.py` & `tastytrade-7.2/tastytrade/account.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/dxfeed/candle.py` & `tastytrade-7.2/tastytrade/dxfeed/candle.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     #: the maximal (high) price of the candle
     high: Optional[Decimal] = None
     #: the minimal (low) price of the candle
     low: Optional[Decimal] = None
     #: the last (close) price of the candle
     close: Optional[Decimal] = None
     #: the total volume of the candle
-    volume: Optional[int] = None
+    volume: Optional[Decimal] = None
     #: volume-weighted average price
     vwap: Optional[Decimal] = None
     #: bid volume in the candle
-    bidVolume: Optional[int] = None
+    bidVolume: Optional[Decimal] = None
     #: ask volume in the candle
-    askVolume: Optional[int] = None
+    askVolume: Optional[Decimal] = None
     #: implied volatility in the candle
     impVolatility: Optional[Decimal] = None
     #: open interest in the candle
     openInterest: Optional[int] = None
```

### Comparing `tastytrade-7.1/tastytrade/dxfeed/event.py` & `tastytrade-7.2/tastytrade/dxfeed/event.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/dxfeed/greeks.py` & `tastytrade-7.2/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/dxfeed/profile.py` & `tastytrade-7.2/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/dxfeed/quote.py` & `tastytrade-7.2/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/dxfeed/summary.py` & `tastytrade-7.2/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/dxfeed/theoprice.py` & `tastytrade-7.2/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/dxfeed/timeandsale.py` & `tastytrade-7.2/tastytrade/dxfeed/timeandsale.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/dxfeed/trade.py` & `tastytrade-7.2/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/dxfeed/underlying.py` & `tastytrade-7.2/tastytrade/dxfeed/underlying.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/instruments.py` & `tastytrade-7.2/tastytrade/instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/metrics.py` & `tastytrade-7.2/tastytrade/metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/order.py` & `tastytrade-7.2/tastytrade/order.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/search.py` & `tastytrade-7.2/tastytrade/search.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/session.py` & `tastytrade-7.2/tastytrade/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -162,39 +162,40 @@
         elif remember_token is not None:
             body['remember-token'] = remember_token
         else:
             raise TastytradeError('You must provide a password or remember '
                                   'token to log in.')
         #: The base url to use for API requests
         self.base_url: str = API_URL
+        #: The headers to use for API requests
+        self.headers: Dict[str, str] = {'User-Agent': UserAgent().random}
 
         if two_factor_authentication is not None:
-            headers = {'X-Tastyworks-OTP': two_factor_authentication}
+            headers = {
+                **self.headers,
+                'X-Tastyworks-OTP': two_factor_authentication
+            }
             response = requests.post(
                 f'{self.base_url}/sessions',
                 json=body,
                 headers=headers
             )
         else:
             response = requests.post(f'{self.base_url}/sessions', json=body)
         validate_response(response)  # throws exception if not 200
 
         json = response.json()
         #: The user dict returned by the API; contains basic user information
         self.user: Dict[str, str] = json['data']['user']
         #: The session token used to authenticate requests
         self.session_token: str = json['data']['session-token']
+        self.headers['Authorization'] = self.session_token
         #: A single-use token which can be used to login without a password
         self.remember_token: Optional[str] = \
             json['data']['remember-token'] if remember_me else None
-        #: The headers to use for API requests
-        self.headers: Dict[str, str] = {
-            'Authorization': self.session_token,
-            'User-Agent': UserAgent().random
-        }
         self.validate()
 
         # Pull streamer tokens and urls
         response = requests.get(
             f'{self.base_url}/quote-streamer-tokens',
             headers=self.headers
         )
```

### Comparing `tastytrade-7.1/tastytrade/streamer.py` & `tastytrade-7.2/tastytrade/streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/utils.py` & `tastytrade-7.2/tastytrade/utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade/watchlists.py` & `tastytrade-7.2/tastytrade/watchlists.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tastytrade.egg-info/PKG-INFO` & `tastytrade-7.2/tastytrade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 7.1
+Version: 7.2
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `tastytrade-7.1/tastytrade.egg-info/SOURCES.txt` & `tastytrade-7.2/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tests/test_account.py` & `tastytrade-7.2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tests/test_instruments.py` & `tastytrade-7.2/tests/test_instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tests/test_streamer.py` & `tastytrade-7.2/tests/test_streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tests/test_utils.py` & `tastytrade-7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tastytrade-7.1/tests/test_watchlists.py` & `tastytrade-7.2/tests/test_watchlists.py`

 * *Files identical despite different names*


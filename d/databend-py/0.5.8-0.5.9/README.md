# Comparing `tmp/databend-py-0.5.8.tar.gz` & `tmp/databend-py-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databend-py-0.5.8.tar", last modified: Mon Mar 25 12:25:59 2024, max compression
+gzip compressed data, was "databend-py-0.5.9.tar", last modified: Fri Apr 26 08:22:16 2024, max compression
```

## Comparing `databend-py-0.5.8.tar` & `databend-py-0.5.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:25:59.438097 databend-py-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-25 12:25:48.000000 databend-py-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 12:25:48.000000 databend-py-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-25 12:25:59.438097 databend-py-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-25 12:25:48.000000 databend-py-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:25:59.438097 databend-py-0.5.8/databend_py/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/datetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/defines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/sdk_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:25:59.438097 databend-py-0.5.8/databend_py/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/util/escape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-25 12:25:48.000000 databend-py-0.5.8/databend_py/util/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:25:59.438097 databend-py-0.5.8/databend_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-25 12:25:59.000000 databend-py-0.5.8/databend_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-25 12:25:59.000000 databend-py-0.5.8/databend_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:25:59.000000 databend-py-0.5.8/databend_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-25 12:25:59.000000 databend-py-0.5.8/databend_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 12:25:59.000000 databend-py-0.5.8/databend_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-25 12:25:59.438097 databend-py-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-25 12:25:48.000000 databend-py-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:16.938605 databend-py-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 08:22:04.000000 databend-py-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 08:22:04.000000 databend-py-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-26 08:22:16.938605 databend-py-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-26 08:22:04.000000 databend-py-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:16.938605 databend-py-0.5.9/databend_py/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/datetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/defines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/sdk_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:16.938605 databend-py-0.5.9/databend_py/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/util/escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-26 08:22:04.000000 databend-py-0.5.9/databend_py/util/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:22:16.938605 databend-py-0.5.9/databend_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 08:22:16.000000 databend-py-0.5.9/databend_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 08:22:16.938605 databend-py-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-26 08:22:04.000000 databend-py-0.5.9/setup.py
```

### Comparing `databend-py-0.5.8/LICENSE` & `databend-py-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/PKG-INFO` & `databend-py-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Platform: UNKNOWN
```

### Comparing `databend-py-0.5.8/README.md` & `databend-py-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/__init__.py` & `databend-py-0.5.9/databend_py/__init__.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/client.py` & `databend-py-0.5.9/databend_py/client.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/connection.py` & `databend-py-0.5.9/databend_py/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,25 +131,38 @@
     def do_query(self, url, query_sql):
         response = self.requests_session.post(url,
                                               data=json.dumps(query_sql),
                                               headers=self.make_headers(),
                                               auth=HTTPBasicAuth(self.user, self.password),
                                               timeout=(self.connect_timeout, self.read_timeout),
                                               verify=True)
-        try:
-            resp_dict = json.loads(response.content)
-        except json.decoder.JSONDecodeError:
-            raise UnexpectedException("failed to parse response: %s" % response.content)
-        if resp_dict and resp_dict.get('error') and "no endpoint" in resp_dict.get('error'):
-            raise WarehouseTimeoutException
-        if resp_dict and resp_dict.get('error'):
-            raise UnexpectedException("failed to query: %s" % response.content)
-        if self.persist_cookies:
-            self.cookies = response.cookies
-        return resp_dict
+        if response.status_code != 200:
+            try:
+                resp_dict = json.loads(response.content)
+                if resp_dict and resp_dict.get('error') and "no endpoint" in resp_dict.get('error'):
+                    raise WarehouseTimeoutException
+            except ValueError:
+                pass
+            raise UnexpectedException("Unexpected status code %d when post query, content: %s" %
+                                      (response.status_code, response.content))
+
+        if response.content:
+            try:
+                resp_dict = json.loads(response.content)
+            except ValueError:
+                raise UnexpectedException("failed to parse response: %s" % response.content)
+            if resp_dict and resp_dict.get('error') and "no endpoint" in resp_dict.get('error'):
+                raise WarehouseTimeoutException
+            if resp_dict and resp_dict.get('error'):
+                raise UnexpectedException("failed to query: %s" % response.content)
+            if self.persist_cookies:
+                self.cookies = response.cookies
+            return resp_dict
+        else:
+            raise UnexpectedException("response content is empty: %s" % response)
 
     def query(self, statement):
         url = self.format_url()
         log.logger.debug(f"http sql: {statement}")
         query_sql = {'sql': statement, "string_fields": True}
         if self.client_session is not None and len(self.client_session) != 0:
             if "database" not in self.client_session:
@@ -188,24 +201,30 @@
 
     def wait_until_has_schema(self, raw_data_dict):
         resp_schema = raw_data_dict.get("schema")
         while resp_schema is not None and len(resp_schema) == 0:
             if raw_data_dict['next_uri'] is None:
                 break
             resp = self.next_page(raw_data_dict['next_uri'])
+
             resp_dict = json.loads(resp.content)
             raw_data_dict = resp_dict
             resp_schema = raw_data_dict.get("schema")
             if resp_schema is not None and (len(resp_schema) != 0 or len(raw_data_dict.get("data")) != 0):
                 break
         return raw_data_dict
 
     def next_page(self, next_uri):
         url = "{}://{}:{}{}".format(self.schema, self.host, self.port, next_uri)
-        return self.requests_session.get(url=url, headers=self.make_headers(), cookies=self.cookies)
+
+        response = self.requests_session.get(url=url, headers=self.make_headers(), cookies=self.cookies)
+        if response.status_code != 200:
+            raise UnexpectedException("Unexpected status code %d when get %s, content: %s" %
+                                      (response.status_code, url, response.content))
+        return response
 
     # return a list of response util empty next_uri
     def query_with_session(self, statement):
         response_list = list()
         response = self.query(statement)
         log.logger.debug(f"response content: {response}")
         response_list.append(response)
```

### Comparing `databend-py-0.5.8/databend_py/context.py` & `databend-py-0.5.9/databend_py/context.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/datetypes.py` & `databend-py-0.5.9/databend_py/datetypes.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/errors.py` & `databend-py-0.5.9/databend_py/errors.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/result.py` & `databend-py-0.5.9/databend_py/result.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/retry.py` & `databend-py-0.5.9/databend_py/retry.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/uploader.py` & `databend-py-0.5.9/databend_py/uploader.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/util/escape.py` & `databend-py-0.5.9/databend_py/util/escape.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py/util/helper.py` & `databend-py-0.5.9/databend_py/util/helper.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/databend_py.egg-info/PKG-INFO` & `databend-py-0.5.9/databend_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Platform: UNKNOWN
```

### Comparing `databend-py-0.5.8/databend_py.egg-info/SOURCES.txt` & `databend-py-0.5.9/databend_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databend-py-0.5.8/setup.py` & `databend-py-0.5.9/setup.py`

 * *Files identical despite different names*


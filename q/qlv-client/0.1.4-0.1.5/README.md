# Comparing `tmp/qlv-client-0.1.4.tar.gz` & `tmp/qlv-client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.1.4.tar", last modified: Thu Apr 25 03:17:18 2024, max compression
+gzip compressed data, was "qlv-client-0.1.5.tar", last modified: Thu Apr 25 14:45:10 2024, max compression
```

## Comparing `qlv-client-0.1.4.tar` & `qlv-client-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 03:17:18.660207 qlv-client-0.1.4/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      456 2024-04-25 03:17:18.659710 qlv-client-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 03:17:18.656234 qlv-client-0.1.4/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.1.4/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.1.4/qlv_client/api.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.1.4/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.1.4/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-17 08:27:22.000000 qlv-client-0.1.4/qlv_client/http_client.py
--rw-rw-rw-   0        0        0     5940 2024-04-25 03:16:49.000000 qlv-client-0.1.4/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.1.4/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.1.4/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.1.4/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 03:17:18.659214 qlv-client-0.1.4/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-04-25 03:17:18.000000 qlv-client-0.1.4/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-04-25 03:17:18.000000 qlv-client-0.1.4/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 03:17:18.000000 qlv-client-0.1.4/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-25 03:17:18.000000 qlv-client-0.1.4/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 03:17:18.000000 qlv-client-0.1.4/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 03:17:18.660207 qlv-client-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-04-25 03:17:15.000000 qlv-client-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:45:10.941520 qlv-client-0.1.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-04-25 14:45:10.941024 qlv-client-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 14:45:10.937546 qlv-client-0.1.5/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.1.5/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.1.5/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.1.5/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.1.5/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-17 08:27:22.000000 qlv-client-0.1.5/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0     6741 2024-04-25 14:41:56.000000 qlv-client-0.1.5/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.1.5/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.1.5/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.1.5/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:45:10.940526 qlv-client-0.1.5/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-04-25 14:45:10.000000 qlv-client-0.1.5/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-04-25 14:45:10.000000 qlv-client-0.1.5/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 14:45:10.000000 qlv-client-0.1.5/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-25 14:45:10.000000 qlv-client-0.1.5/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 14:45:10.000000 qlv-client-0.1.5/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 14:45:10.941520 qlv-client-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-04-25 14:27:19.000000 qlv-client-0.1.5/setup.py
```

### Comparing `qlv-client-0.1.4/LICENSE` & `qlv-client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.4/qlv_client/api.py` & `qlv-client-0.1.5/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.4/qlv_client/config.py` & `qlv-client-0.1.5/qlv_client/config.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.4/qlv_client/converter.py` & `qlv-client-0.1.5/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.4/qlv_client/http_client.py` & `qlv-client-0.1.5/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.4/qlv_client/proxy.py` & `qlv-client-0.1.5/qlv_client/proxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -114,11 +114,25 @@
             args.update(order_itinerary_info)
             order_ser = OrderService(**QlvConfigRepository.get_host_params())
             result = order_ser.fill_order_itinerary_info(**args)
             if result.get("code") == 0:
                 logger.error("向劲旅系统回填乘客票单信息失败...")
                 return False
             else:
-                logger.error("向劲旅系统回填乘客票单信息成功.")
+                logger.info("向劲旅系统回填乘客票单信息成功.")
                 return True
         else:
             return False
+
+    @classmethod
+    def save_new_log(cls, pre_order_id: int, oper: str, logs: str) -> bool:
+        logger.info("开始向劲旅系统给订单<{}>记录新日志...".format(pre_order_id))
+        args = QlvConfigRepository.get_request_base_params(inter_name="write_order_log_new")
+        args.update(dict(pre_order_id=pre_order_id, oper=oper, logs=logs))
+        order_ser = OrderService(**QlvConfigRepository.get_host_params())
+        result = order_ser.write_order_log_new(**args)
+        if result.get("code") == 0:
+            logger.error("向劲旅系统给订单<{}>记录新日志失败...".format(pre_order_id))
+            return False
+        else:
+            logger.info("向劲旅系统给订单<{}>记录新日志成功.".format(pre_order_id))
+            return True
```

### Comparing `qlv-client-0.1.4/qlv_client/repository.py` & `qlv-client-0.1.5/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.4/qlv_client/test.py` & `qlv-client-0.1.5/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.4/qlv_client/utils.py` & `qlv-client-0.1.5/qlv_client/utils.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.4/setup.py` & `qlv-client-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qlv-client',
-    version='0.1.4',
+    version='0.1.5',
     description='This is my qlv proxy qlv_client package',
     long_description='This is my qlv proxy qlv_client package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/qlvClient',
     packages=find_packages(),
     install_requires=[
```


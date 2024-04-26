# Comparing `tmp/ctrip-app-ui-0.1.8.tar.gz` & `tmp/ctrip-app-ui-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.1.8.tar", last modified: Thu Apr 25 10:34:01 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.1.9.tar", last modified: Thu Apr 25 10:58:44 2024, max compression
```

## Comparing `ctrip-app-ui-0.1.8.tar` & `ctrip-app-ui-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 10:34:01.962695 ctrip-app-ui-0.1.8/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-25 10:34:01.960726 ctrip-app-ui-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 10:34:01.947735 ctrip-app-ui-0.1.8/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.1.8/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.1.8/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.1.8/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.1.8/capp_ui/dir.py
--rw-rw-rw-   0        0        0    53666 2024-04-25 10:33:53.000000 ctrip-app-ui-0.1.8/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.1.8/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.1.8/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.1.8/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.1.8/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.1.8/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.1.8/capp_ui/utils.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.1.8/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:34:01.958734 ctrip-app-ui-0.1.8/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-25 10:34:01.000000 ctrip-app-ui-0.1.8/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-25 10:34:01.000000 ctrip-app-ui-0.1.8/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 10:34:01.000000 ctrip-app-ui-0.1.8/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 10:34:01.000000 ctrip-app-ui-0.1.8/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 10:34:01.000000 ctrip-app-ui-0.1.8/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 10:34:01.962695 ctrip-app-ui-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-25 10:33:58.000000 ctrip-app-ui-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:58:44.987601 ctrip-app-ui-0.1.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-25 10:58:44.986604 ctrip-app-ui-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 10:58:44.976631 ctrip-app-ui-0.1.9/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.1.9/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.1.9/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.1.9/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.1.9/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    54496 2024-04-25 10:58:31.000000 ctrip-app-ui-0.1.9/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.1.9/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.1.9/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.1.9/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.1.9/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.1.9/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.1.9/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.1.9/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-25 10:58:44.984638 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 10:58:44.987601 ctrip-app-ui-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-25 10:58:40.000000 ctrip-app-ui-0.1.9/setup.py
```

### Comparing `ctrip-app-ui-0.1.8/LICENSE` & `ctrip-app-ui-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/date_extend.py` & `ctrip-app-ui-0.1.9/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/device.py` & `ctrip-app-ui-0.1.9/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/dir.py` & `ctrip-app-ui-0.1.9/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/domain_service.py` & `ctrip-app-ui-0.1.9/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,35 @@
         except (PocoNoSuchNodeException, PocoTargetTimeout):
             pass
         except Exception as e:
             logger.error(e)
         return flag
 
     @SleepWait(wait_time=1)
+    def get_order_status(self) -> str:
+        """检查搜索列表界面，获取订单的状态"""
+        status = None
+        try:
+            unpaid_status = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="去支付"
+            )
+            cancel_status = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", text="已取消"
+            )
+            if unpaid_status.exists() is True:
+                status = "待支付"
+            elif cancel_status.exists() is True:
+                status = "已取消"
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            pass
+        except Exception as e:
+            logger.error(e)
+        return status
+
+    @SleepWait(wait_time=1)
     def touch_go_back_to_unpaid_list_page(self) -> None:
         """从搜索界面退回到【待支付】列表页"""
         try:
             go_back = self.device.poco(type="android.widget.TextView", name="icon_back")
             if go_back.exists() is True:
                 go_back.click()
                 go_back.click()
```

### Comparing `ctrip-app-ui-0.1.8/capp_ui/fee.py` & `ctrip-app-ui-0.1.9/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/libs.py` & `ctrip-app-ui-0.1.9/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.1.9/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/platforms.py` & `ctrip-app-ui-0.1.9/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/test.py` & `ctrip-app-ui-0.1.9/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/utils.py` & `ctrip-app-ui-0.1.9/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/capp_ui/validators.py` & `ctrip-app-ui-0.1.9/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.8/setup.py` & `ctrip-app-ui-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.1.8',
+    version='0.1.9',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```


# Comparing `tmp/ctrip-app-ui-0.2.0.tar.gz` & `tmp/ctrip-app-ui-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.2.0.tar", last modified: Fri Apr 26 03:59:07 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.2.1.tar", last modified: Fri Apr 26 08:10:06 2024, max compression
```

## Comparing `ctrip-app-ui-0.2.0.tar` & `ctrip-app-ui-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 03:59:07.516895 ctrip-app-ui-0.2.0/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-26 03:59:07.514902 ctrip-app-ui-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 03:59:07.503964 ctrip-app-ui-0.2.0/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.2.0/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.2.0/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.2.0/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.2.0/capp_ui/dir.py
--rw-rw-rw-   0        0        0    54496 2024-04-25 10:58:31.000000 ctrip-app-ui-0.2.0/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.2.0/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.2.0/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.2.0/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.2.0/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.2.0/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.2.0/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3016 2024-04-26 03:58:23.000000 ctrip-app-ui-0.2.0/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-26 03:59:07.513904 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 03:59:07.516895 ctrip-app-ui-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-26 03:59:02.000000 ctrip-app-ui-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:10:06.829502 ctrip-app-ui-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-26 08:10:06.828506 ctrip-app-ui-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 08:10:06.817562 ctrip-app-ui-0.2.1/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.2.1/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3500 2024-04-26 08:02:36.000000 ctrip-app-ui-0.2.1/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.2.1/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.2.1/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    56819 2024-04-26 08:09:49.000000 ctrip-app-ui-0.2.1/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.2.1/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.2.1/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.2.1/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.2.1/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.2.1/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.2.1/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3016 2024-04-26 03:58:23.000000 ctrip-app-ui-0.2.1/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:10:06.826511 ctrip-app-ui-0.2.1/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-26 08:10:06.000000 ctrip-app-ui-0.2.1/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-26 08:10:06.000000 ctrip-app-ui-0.2.1/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 08:10:06.000000 ctrip-app-ui-0.2.1/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-26 08:10:06.000000 ctrip-app-ui-0.2.1/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 08:10:06.000000 ctrip-app-ui-0.2.1/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 08:10:06.830524 ctrip-app-ui-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-26 07:41:15.000000 ctrip-app-ui-0.2.1/setup.py
```

### Comparing `ctrip-app-ui-0.2.0/LICENSE` & `ctrip-app-ui-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/capp_ui/date_extend.py` & `ctrip-app-ui-0.2.1/capp_ui/date_extend.py`

 * *Files 23% similar despite different names*

```diff
@@ -85,7 +85,18 @@
     dt = datetime.strptime(dt_str, standard_date_format)
     dt_step = dt + timedelta(hours=time_zone_step)
     return dt_step.strftime(standard_date_format)
 
 
 def current_datetime_str() -> str:
     return datetime.now().strftime(standard_date_format)
+
+
+def is_later_than_current_time(time_str: str, minutes: int = 5):
+    # 将给定时间字符串转换为 datetime 对象
+    given_time = datetime.strptime(time_str, '%H:%M')
+    # 获取当前时间
+    current_time = datetime.now()
+    # 计算当前时间之后5分钟的时间
+    five_minutes_later = current_time + timedelta(minutes=minutes)
+    # 比较给定时间是否晚于当前时间5分钟后的时间
+    return given_time > five_minutes_later
```

### Comparing `ctrip-app-ui-0.2.0/capp_ui/device.py` & `ctrip-app-ui-0.2.1/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/capp_ui/dir.py` & `ctrip-app-ui-0.2.1/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/capp_ui/domain_service.py` & `ctrip-app-ui-0.2.1/capp_ui/domain_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/04/24
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import re
-import time
 import typing as t
 from decimal import Decimal
 from poco.proxy import UIObjectProxy
 from poco.exceptions import PocoNoSuchNodeException, PocoTargetTimeout
 
 from capp_ui.platforms import PlatformService
 from capp_ui.mobile_terminals import stop_app
 from capp_ui.libs import SleepWait, LoopFindElement
 from capp_ui.utils import logger, get_ui_object_proxy_attr
+from capp_ui.date_extend import is_later_than_current_time
 from capp_ui.dir import get_images_dir, is_exists, join_path
 from capp_ui.date_extend import get_trip_year_month_day, get_datetime_area, is_public_holiday
 
 
 class CtripAppService(PlatformService):
     """
     携程APP
@@ -206,14 +206,69 @@
 
     @SleepWait(wait_time=1)
     def touch_to_payment_at_list_page(self) -> None:
         """进入待付款列表页，点击【去支付】"""
         search_box = self.device.poco(type="android.widget.TextView", name="android.widget.TextView", text="去支付")
         search_box.click()
 
+    @SleepWait(wait_time=1)
+    def is_cancel_order(self, out_total_price: str) -> tuple:
+        """在订单详情页，判断是否需要取消订单"""
+        flag = False
+        remark = None
+        try:
+            is_cancel = self.device.poco(
+                type="android.widget.TextView", name="android.widget.TextView", textMatches=r"^请在\d+:\d+前支付.*"
+            )
+            if is_cancel.exists() is True:
+                text = is_cancel.get_text()
+                time_match = re.search(r'(\d{2}:\d{2})', text)
+                amount_match = re.search(r'¥(\d+)', text)
+                # 提取匹配到的内容
+                if time_match:
+                    time_str = time_match.group(1)
+                    is_later = is_later_than_current_time(time_str=time_str, minutes=5)
+                    if is_later is False:
+                        flag = True
+                        remark = "支付时间少于5分钟"
+                elif amount_match:
+                    amount_str = amount_match.group(1)
+                    if Decimal(amount_str) > Decimal(out_total_price):
+                        flag = True
+                        remark = "航班已变价"
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            pass
+        except Exception as e:
+            logger.error(e)
+        return flag, remark
+
+    @SleepWait(wait_time=1)
+    def touch_cancel_order(self) -> None:
+        try:
+            cancel_order = self.device.poco(
+                type="android.widget.TextView", name="operateBtnList_Text_取消订单", text="取消订单"
+            )
+            cancel_order.click()
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            pass
+        except Exception as e:
+            logger.error(e)
+
+    @SleepWait(wait_time=1)
+    def touch_submit_cancel_order(self) -> None:
+        try:
+            submit_cancel_order = self.device.poco(
+                type="android.widget.TextView", name="Button_Text_取消订单", text="取消订单"
+            )
+            submit_cancel_order.click()
+        except (PocoNoSuchNodeException, PocoTargetTimeout):
+            pass
+        except Exception as e:
+            logger.error(e)
+
     @SleepWait(wait_time=2)
     def touch_to_payment_at_order_detail(self) -> None:
         """在订单详情页，点击【去支付】"""
         search_box = self.device.poco(type="android.widget.TextView", name="pcardLimit_Text_去支付", text="去支付")
         search_box.click()
 
     @SleepWait(wait_time=1)
```

### Comparing `ctrip-app-ui-0.2.0/capp_ui/fee.py` & `ctrip-app-ui-0.2.1/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/capp_ui/libs.py` & `ctrip-app-ui-0.2.1/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.2.1/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/capp_ui/platforms.py` & `ctrip-app-ui-0.2.1/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/capp_ui/test.py` & `ctrip-app-ui-0.2.1/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/capp_ui/utils.py` & `ctrip-app-ui-0.2.1/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/capp_ui/validators.py` & `ctrip-app-ui-0.2.1/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.2.0/setup.py` & `ctrip-app-ui-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.2.0',
+    version='0.2.1',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```


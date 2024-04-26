# Comparing `tmp/ctrip-app-ui-0.1.9.tar.gz` & `tmp/ctrip-app-ui-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.1.9.tar", last modified: Thu Apr 25 10:58:44 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.2.0.tar", last modified: Fri Apr 26 03:59:07 2024, max compression
```

## Comparing `ctrip-app-ui-0.1.9.tar` & `ctrip-app-ui-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 10:58:44.987601 ctrip-app-ui-0.1.9/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-25 10:58:44.986604 ctrip-app-ui-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 10:58:44.976631 ctrip-app-ui-0.1.9/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.1.9/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.1.9/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.1.9/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.1.9/capp_ui/dir.py
--rw-rw-rw-   0        0        0    54496 2024-04-25 10:58:31.000000 ctrip-app-ui-0.1.9/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.1.9/capp_ui/fee.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.1.9/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.1.9/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.1.9/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.1.9/capp_ui/test.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.1.9/capp_ui/utils.py
--rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.1.9/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-25 10:58:44.984638 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 10:58:44.000000 ctrip-app-ui-0.1.9/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 10:58:44.987601 ctrip-app-ui-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-25 10:58:40.000000 ctrip-app-ui-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:59:07.516895 ctrip-app-ui-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-26 03:59:07.514902 ctrip-app-ui-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 03:59:07.503964 ctrip-app-ui-0.2.0/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.2.0/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.2.0/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.2.0/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.2.0/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    54496 2024-04-25 10:58:31.000000 ctrip-app-ui-0.2.0/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.2.0/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.2.0/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-25 08:28:03.000000 ctrip-app-ui-0.2.0/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.2.0/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      689 2024-04-25 07:52:15.000000 ctrip-app-ui-0.2.0/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.2.0/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3016 2024-04-26 03:58:23.000000 ctrip-app-ui-0.2.0/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-26 03:59:07.513904 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-26 03:59:07.000000 ctrip-app-ui-0.2.0/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 03:59:07.516895 ctrip-app-ui-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-26 03:59:02.000000 ctrip-app-ui-0.2.0/setup.py
```

### Comparing `ctrip-app-ui-0.1.9/LICENSE` & `ctrip-app-ui-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/date_extend.py` & `ctrip-app-ui-0.2.0/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/device.py` & `ctrip-app-ui-0.2.0/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/dir.py` & `ctrip-app-ui-0.2.0/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/domain_service.py` & `ctrip-app-ui-0.2.0/capp_ui/domain_service.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/fee.py` & `ctrip-app-ui-0.2.0/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/libs.py` & `ctrip-app-ui-0.2.0/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.2.0/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/platforms.py` & `ctrip-app-ui-0.2.0/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/test.py` & `ctrip-app-ui-0.2.0/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/utils.py` & `ctrip-app-ui-0.2.0/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.1.9/capp_ui/validators.py` & `ctrip-app-ui-0.2.0/capp_ui/validators.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,19 +17,22 @@
 
 
 class FlightTicketValidator(object):
     """机票校验器"""
 
     @classmethod
     def validator_payment_with_deduction(cls, pre_sale_amount: Decimal, actual_amount: Decimal,
-                                         deduction_amount: Decimal) -> bool:
+                                         deduction_amount: Decimal, is_include_tax: bool = False) -> bool:
         """支付校验, 抵扣场景，默认积分抵扣场景，可以抵扣10.00元"""
         if deduction_amount >= 10.00:
-            expected_amount = pre_sale_amount + flight_fee.get("fuel_fee") + flight_fee.get(
-                "airport_fee") - deduction_amount
+            if is_include_tax is False:
+                expected_amount = pre_sale_amount + flight_fee.get("fuel_fee") + flight_fee.get(
+                    "airport_fee") - deduction_amount
+            else:
+                expected_amount = pre_sale_amount - deduction_amount
             if expected_amount >= actual_amount:
                 logger.info("订单的实际支付金额<{}>小于或等于预期的支付金额<{}>，可以正常交易.".format(
                     actual_amount, expected_amount)
                 )
                 return True
             else:
                 logger.error(
@@ -39,17 +42,21 @@
             if deduction_amount > 0:
                 logger.warning("抵扣金额<{}>不足10.00元.".format(deduction_amount))
             else:
                 logger.error("获取到的抵扣金额<{}>有异常.".format(deduction_amount))
             return False
 
     @classmethod
-    def validator_payment_with_wallet(cls, pre_sale_amount: Decimal, actual_amount: Decimal) -> bool:
+    def validator_payment_with_wallet(cls, pre_sale_amount: Decimal, actual_amount: Decimal,
+                                      is_include_tax: bool = False) -> bool:
         """支付校验, 钱包场景"""
-        expected_amount = pre_sale_amount + flight_fee.get("fuel_fee") + flight_fee.get("airport_fee")
+        if is_include_tax is False:
+            expected_amount = pre_sale_amount + flight_fee.get("fuel_fee") + flight_fee.get("airport_fee")
+        else:
+            expected_amount = pre_sale_amount
         if actual_amount >= expected_amount:
             logger.info("钱包的余额<{}>大于或等于预期的支付金额<{}>，可以正常交易.".format(
                 actual_amount, expected_amount)
             )
             return True
         else:
             logger.warning(
```

### Comparing `ctrip-app-ui-0.1.9/setup.py` & `ctrip-app-ui-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.1.9',
+    version='0.2.0',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```


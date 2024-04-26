# Comparing `tmp/pretix-cashpayment-2.0.3.tar.gz` & `tmp/pretix_cashpayment-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-cashpayment-2.0.3.tar", last modified: Wed Jul  5 14:58:07 2023, max compression
+gzip compressed data, was "pretix_cashpayment-2.1.0.tar", last modified: Fri Apr 26 11:52:50 2024, max compression
```

## Comparing `pretix-cashpayment-2.0.3.tar` & `pretix_cashpayment-2.1.0.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/
--rw-rw-r--   0 martin    (1000) martin    (1000)      553 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)      141 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)     4064 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     3705 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/README.rst
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/
--rw-rw-r--   0 martin    (1000) martin    (1000)       22 2023-07-05 14:50:25.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      575 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/apps.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/LC_MESSAGES/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1735 2020-04-17 14:06:38.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 martin    (1000) martin    (1000)     3103 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1722 2020-04-17 14:06:38.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-r--   0 martin    (1000) martin    (1000)     3087 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.po
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1823 2020-04-17 14:06:38.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 martin    (1000) martin    (1000)     2721 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.po
--rw-rw-r--   0 martin    (1000) martin    (1000)     2694 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/payment.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      917 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/signals.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/
--rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/checkout_payment_form.html
--rw-rw-r--   0 martin    (1000) martin    (1000)      998 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/control.html
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/email/
--rw-rw-r--   0 martin    (1000) martin    (1000)      262 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/email/order_pending.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      401 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/pending.html
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     4064 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      979 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       72 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      363 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     1145 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-26 11:52:26.000000 pretix_cashpayment-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4811 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3705 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/pretix_cashpayment/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.058395 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.058395 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3103 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.058395 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/de_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3087 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.058395 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     5007 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.058395 pretix_cashpayment-2.1.0/pretix_cashpayment/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/pretix_cashpayment/templates/pretix_cashpayment/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/templates/pretix_cashpayment/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      998 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/templates/pretix_cashpayment/control.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/pretix_cashpayment/templates/pretix_cashpayment/email/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/templates/pretix_cashpayment/email/order_pending.txt
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pretix_cashpayment/templates/pretix_cashpayment/pending.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/pretix_cashpayment.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4811 2024-04-26 11:52:50.000000 pretix_cashpayment-2.1.0/pretix_cashpayment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      829 2024-04-26 11:52:50.000000 pretix_cashpayment-2.1.0/pretix_cashpayment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 11:52:50.000000 pretix_cashpayment-2.1.0/pretix_cashpayment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-26 11:52:50.000000 pretix_cashpayment-2.1.0/pretix_cashpayment.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-26 11:52:50.000000 pretix_cashpayment-2.1.0/pretix_cashpayment.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-26 11:52:50.062394 pretix_cashpayment-2.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-26 11:49:28.000000 pretix_cashpayment-2.1.0/setup.py
```

### Comparing `pretix-cashpayment-2.0.3/LICENSE` & `pretix_cashpayment-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.3/PKG-INFO` & `pretix_cashpayment-2.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pretix-cashpayment
-Version: 2.0.3
-Summary: pretix plugin that allows you to offer your customers a "pay with cash at the venue" option.
-Home-page: http://www.github.com/pc-coholic/pretix-cashpayment
-Author: Martin Gross
-Author-email: martin@pc-coholic.de
-License: Apache Software License
-Platform: UNKNOWN
-License-File: LICENSE
-
 Pretix Cash Payment plugin
 ==========================
 
 .. image:: https://img.shields.io/pypi/v/pretix-cashpayment.svg
    :target: https://pypi.python.org/pypi/pretix-cashpayment
 
 .. image:: https://img.shields.io/badge/translations-POEditor.com-blue.svg
@@ -84,9 +73,7 @@
 
 
 .. _pretix: https://github.com/pretix/pretix
 .. _pretix development setup: https://docs.pretix.eu/en/latest/development/setup.html
 .. _pretix-cashpoint: https://github.com/pc-coholic/pretix-cashpoint
 .. _de.pccoholic.pretix.cashpoint: https://github.com/pc-coholic/de.pccoholic.pretix.cashpoint
 .. _two available workarounds: https://github.com/pc-coholic/pretix-cashpayment/issues/5#issuecomment-382447489
-
-
```

### Comparing `pretix-cashpayment-2.0.3/README.rst` & `pretix_cashpayment-2.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: pretix-cashpayment
+Version: 2.1.0
+Summary: pretix plugin that allows you to offer your customers a "pay with cash at the venue" option.
+Author-email: Martin Gross <martin@pc-coholic.de>
+Maintainer-email: Martin Gross <martin@pc-coholic.de>
+License: Copyright 2017 Martin Gross
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+            http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+        
+Project-URL: homepage, http://github.com/pc-coholic/pretix-cashpayment
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 Pretix Cash Payment plugin
 ==========================
 
 .. image:: https://img.shields.io/pypi/v/pretix-cashpayment.svg
    :target: https://pypi.python.org/pypi/pretix-cashpayment
 
 .. image:: https://img.shields.io/badge/translations-POEditor.com-blue.svg
```

### Comparing `pretix-cashpayment-2.0.3/pretix_cashpayment/apps.py` & `pretix_cashpayment-2.1.0/pretix_cashpayment/apps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from django.apps import AppConfig
 from django.utils.translation import gettext_lazy as _
+
 from . import __version__
 
+
 class PluginApp(AppConfig):
     name = 'pretix_cashpayment'
     verbose_name = 'Pretix Cash Payment plugin'
 
     class PretixPluginMeta:
         name = _('Cash Payment')
         author = 'Martin Gross'
         description = _('This plugin allows you to offer your customers a "pay with cash at the venue" option.')
         category = 'PAYMENT'
         visible = True
         version = __version__
+        compatibility = "pretix>=2024.4.0.dev0"
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/LC_MESSAGES/django.po` & `pretix_cashpayment-2.1.0/pretix_cashpayment/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.po` & `pretix_cashpayment-2.1.0/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.po` & `pretix_cashpayment-2.1.0/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.3/pretix_cashpayment/signals.py` & `pretix_cashpayment-2.1.0/pretix_cashpayment/signals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.dispatch import receiver
 from django.utils.translation import gettext_noop
 from i18nfield.strings import LazyI18nString
-from rest_framework import serializers
-
 from pretix.base.settings import settings_hierarkey
-from pretix.base.signals import register_payment_providers, api_event_settings_fields
+from pretix.base.signals import (
+    api_event_settings_fields, register_payment_providers,
+)
+from rest_framework import serializers
 
 
 @receiver(register_payment_providers, dispatch_uid="payment_cash")
 def register_payment_provider(sender, **kwargs):
     from .payment import CashPayment
     return CashPayment
```

### Comparing `pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/control.html` & `pretix_cashpayment-2.1.0/pretix_cashpayment/templates/pretix_cashpayment/control.html`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/PKG-INFO` & `pretix_cashpayment-2.1.0/pretix_cashpayment.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 Metadata-Version: 2.1
 Name: pretix-cashpayment
-Version: 2.0.3
+Version: 2.1.0
 Summary: pretix plugin that allows you to offer your customers a "pay with cash at the venue" option.
-Home-page: http://www.github.com/pc-coholic/pretix-cashpayment
-Author: Martin Gross
-Author-email: martin@pc-coholic.de
-License: Apache Software License
-Platform: UNKNOWN
+Author-email: Martin Gross <martin@pc-coholic.de>
+Maintainer-email: Martin Gross <martin@pc-coholic.de>
+License: Copyright 2017 Martin Gross
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+            http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+        
+Project-URL: homepage, http://github.com/pc-coholic/pretix-cashpayment
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Pretix Cash Payment plugin
 ==========================
 
 .. image:: https://img.shields.io/pypi/v/pretix-cashpayment.svg
    :target: https://pypi.python.org/pypi/pretix-cashpayment
@@ -84,9 +99,7 @@
 
 
 .. _pretix: https://github.com/pretix/pretix
 .. _pretix development setup: https://docs.pretix.eu/en/latest/development/setup.html
 .. _pretix-cashpoint: https://github.com/pc-coholic/pretix-cashpoint
 .. _de.pccoholic.pretix.cashpoint: https://github.com/pc-coholic/de.pccoholic.pretix.cashpoint
 .. _two available workarounds: https://github.com/pc-coholic/pretix-cashpayment/issues/5#issuecomment-382447489
-
-
```

### Comparing `pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/SOURCES.txt` & `pretix_cashpayment-2.1.0/pretix_cashpayment.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_cashpayment/__init__.py
 pretix_cashpayment/apps.py
 pretix_cashpayment/payment.py
 pretix_cashpayment/signals.py
 pretix_cashpayment.egg-info/PKG-INFO
 pretix_cashpayment.egg-info/SOURCES.txt
 pretix_cashpayment.egg-info/dependency_links.txt
 pretix_cashpayment.egg-info/entry_points.txt
 pretix_cashpayment.egg-info/top_level.txt
-pretix_cashpayment/locale/de/LC_MESSAGES/django.mo
 pretix_cashpayment/locale/de/LC_MESSAGES/django.po
-pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.mo
 pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.po
-pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.mo
 pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.po
 pretix_cashpayment/templates/pretix_cashpayment/checkout_payment_form.html
 pretix_cashpayment/templates/pretix_cashpayment/control.html
 pretix_cashpayment/templates/pretix_cashpayment/pending.html
 pretix_cashpayment/templates/pretix_cashpayment/email/order_pending.txt
```


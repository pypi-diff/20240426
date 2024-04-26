# Comparing `tmp/oc_python_sdk-2.1.0.tar.gz` & `tmp/oc_python_sdk-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_python_sdk-2.1.0.tar", last modified: Fri Apr 26 12:03:50 2024, max compression
+gzip compressed data, was "oc_python_sdk-3.0.0.tar", last modified: Mon Dec 18 09:16:39 2023, max compression
```

## Comparing `oc_python_sdk-2.1.0.tar` & `oc_python_sdk-3.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:03:50.803359 oc_python_sdk-2.1.0/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2024-02-19 09:17:32.000000 oc_python_sdk-2.1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       71 2024-02-19 09:17:32.000000 oc_python_sdk-2.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      959 2024-04-26 12:03:50.803359 oc_python_sdk-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-02-19 09:17:32.000000 oc_python_sdk-2.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:03:50.799359 oc_python_sdk-2.1.0/oc_python_sdk/
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-04-26 10:00:45.000000 oc_python_sdk-2.1.0/oc_python_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:03:50.803359 oc_python_sdk-2.1.0/oc_python_sdk/models/
--rw-rw-rw-   0 root         (0) root         (0)     3262 2024-04-26 09:37:29.000000 oc_python_sdk-2.1.0/oc_python_sdk/models/application.py
--rwxrwxrwx   0 root         (0) root         (0)     9154 2024-04-26 09:52:52.000000 oc_python_sdk-2.1.0/oc_python_sdk/models/payment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:03:50.803359 oc_python_sdk-2.1.0/oc_python_sdk/utils/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-02-19 09:17:32.000000 oc_python_sdk-2.1.0/oc_python_sdk/utils/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:03:50.803359 oc_python_sdk-2.1.0/oc_python_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      959 2024-04-26 12:03:50.000000 oc_python_sdk-2.1.0/oc_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2024-04-26 12:03:50.000000 oc_python_sdk-2.1.0/oc_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 12:03:50.000000 oc_python_sdk-2.1.0/oc_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-26 12:03:50.000000 oc_python_sdk-2.1.0/oc_python_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-26 12:03:50.000000 oc_python_sdk-2.1.0/oc_python_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-02-19 09:17:32.000000 oc_python_sdk-2.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-26 12:03:50.803359 oc_python_sdk-2.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1646 2024-02-19 09:17:32.000000 oc_python_sdk-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:03:50.803359 oc_python_sdk-2.1.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)       24 2024-02-19 09:17:32.000000 oc_python_sdk-2.1.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11876 2024-04-26 09:52:52.000000 oc_python_sdk-2.1.0/tests/_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2024-04-26 09:37:29.000000 oc_python_sdk-2.1.0/tests/test_application.py
--rw-rw-rw-   0 root         (0) root         (0)     8850 2024-04-26 09:37:29.000000 oc_python_sdk-2.1.0/tests/test_payment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 09:16:39.985403 oc_python_sdk-3.0.0/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-10-27 09:02:30.000000 oc_python_sdk-3.0.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-10-27 09:02:30.000000 oc_python_sdk-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      959 2023-12-18 09:16:39.985403 oc_python_sdk-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-10-27 09:02:30.000000 oc_python_sdk-3.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 09:16:39.985403 oc_python_sdk-3.0.0/oc_python_sdk/
+-rwxrwxrwx   0 root         (0) root         (0)       47 2023-12-18 09:12:28.000000 oc_python_sdk-3.0.0/oc_python_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 09:16:39.985403 oc_python_sdk-3.0.0/oc_python_sdk/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-12-18 08:56:09.000000 oc_python_sdk-3.0.0/oc_python_sdk/models/application.py
+-rwxrwxrwx   0 root         (0) root         (0)     9534 2023-12-18 08:56:09.000000 oc_python_sdk-3.0.0/oc_python_sdk/models/payment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 09:16:39.985403 oc_python_sdk-3.0.0/oc_python_sdk/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-10-27 09:02:30.000000 oc_python_sdk-3.0.0/oc_python_sdk/utils/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 09:16:39.985403 oc_python_sdk-3.0.0/oc_python_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      959 2023-12-18 09:16:39.000000 oc_python_sdk-3.0.0/oc_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-12-18 09:16:39.000000 oc_python_sdk-3.0.0/oc_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-18 09:16:39.000000 oc_python_sdk-3.0.0/oc_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-12-18 09:16:39.000000 oc_python_sdk-3.0.0/oc_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-12-18 09:16:39.000000 oc_python_sdk-3.0.0/oc_python_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-10-27 09:02:30.000000 oc_python_sdk-3.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-12-18 09:16:39.985403 oc_python_sdk-3.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1646 2023-10-28 08:35:06.000000 oc_python_sdk-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 09:16:39.985403 oc_python_sdk-3.0.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)       24 2023-10-27 09:02:30.000000 oc_python_sdk-3.0.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13219 2023-12-18 08:56:09.000000 oc_python_sdk-3.0.0/tests/_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2023-12-12 13:10:28.000000 oc_python_sdk-3.0.0/tests/test_application.py
+-rw-rw-rw-   0 root         (0) root         (0)     9988 2023-12-18 08:56:09.000000 oc_python_sdk-3.0.0/tests/test_payment.py
```

### Comparing `oc_python_sdk-2.1.0/LICENSE` & `oc_python_sdk-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oc_python_sdk-2.1.0/PKG-INFO` & `oc_python_sdk-3.0.0/oc_python_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oc_python_sdk
-Version: 2.1.0
+Name: oc-python-sdk
+Version: 3.0.0
 Summary: Python SDK
 Home-page: https://gitlab.com/opencity-labs/area-personale/python_sdk
 Author: Opencontent
 Author-email: emily.lancietti@opencontent.it
 License: GNU GPLv3 License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `oc_python_sdk-2.1.0/oc_python_sdk/models/application.py` & `oc_python_sdk-3.0.0/oc_python_sdk/models/application.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,21 +41,33 @@
     meta: dict
 
     class Config:
         validate_all = True
         validate_assignment = True
 
 
+class APaymentDataStamp(BaseModel):
+    amount: Optional[float]
+    collection_data: Optional[str]
+    reason: str
+
+    class Config:
+        validate_all = True
+        validate_assignment = True
+
+
 class APaymentData(BaseModel):
     reason: str
     amount: float
     expire_at: str
     split: Union[List[Optional[APaymentDataSplit]], Dict[str, Optional[float]], None]
+    stamps: Union[List[Optional[APaymentDataStamp]], Dict[str, Optional[float]], None]
     notify: ANotify
     landing: Landing
+    config_id: UUID
 
     class Config:
         validate_all = True
         validate_assignment = True
 
     expire_at_must_be_iso8601 = validator('expire_at', allow_reuse=True)(check_iso_format)
 
@@ -86,15 +98,14 @@
     tenant_id: UUID
     service_id: UUID
     user: UUID
     status_name: str
     created_at: str
     payment_data: APaymentData
     applicant: Applicant = Field(alias='data')
-    locale: str = None
     event_version: str
     event_id: UUID
 
     class Config:
         validate_all = True
         validate_assignment = True
```

### Comparing `oc_python_sdk-2.1.0/oc_python_sdk/models/payment.py` & `oc_python_sdk-3.0.0/oc_python_sdk/models/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,27 +48,38 @@
     STATUS_PAYMENT_PENDING = 'PAYMENT_PENDING'
     STATUS_PAYMENT_STARTED = 'PAYMENT_STARTED'
     STATUS_PAYMENT_CONFIRMED = 'PAYMENT_CONFIRMED'
     STATUS_PAYMENT_FAILED = 'PAYMENT_FAILED'
     STATUS_NOTIFICATION_PENDING = 'NOTIFICATION_PENDING'
     STATUS_COMPLETE = 'COMPLETE'
     STATUS_EXPIRED = 'EXPIRED'
-    STATUS_CANCELED = 'CANCELED'
 
     def json(self):
         return json.dumps(self, cls=PaymentEncoder)
 
 
 class PaymentType(Enum):
     TYPE_PAGOPA = 'PAGOPA'
 
     def json(self):
         return json.dumps(self, cls=PaymentEncoder)
 
 
+class RemoteCollectionType(BaseModel):
+    id: UUID
+    type: str
+
+    class Config:
+        validate_all = True
+        validate_assignment = True
+
+    def json(self):
+        return json.dumps(self, cls=PaymentEncoder)
+
+
 class PayerType(Enum):
     TYPE_HUMAN = 'human'
     TYPE_LEGAL = 'legal'
 
     def json(self):
         return json.dumps(self, cls=PaymentEncoder)
 
@@ -82,24 +93,39 @@
         validate_all = True
         validate_assignment = True
 
     def json(self):
         return json.dumps(self, cls=PaymentEncoder)
 
 
+class PaymentDataStamp(BaseModel):
+    amount: float
+    collection_data: Optional[str]
+    reason: str
+    meta: dict
+
+    class Config:
+        validate_all = True
+        validate_assignment = True
+
+    def json(self):
+        return json.dumps(self, cls=PaymentEncoder)
+
+
 class PaymentData(BaseModel):
     transaction_id: Optional[str]
     paid_at: Optional[str]
     expire_at: str
     amount: float
     currency: CurrencyType
     notice_code: Optional[str]
     iud: str
     iuv: Optional[str]
     split: List[Optional[PaymentDataSplit]]
+    stamps: List[Optional[PaymentDataStamp]]
 
     class Config:
         validate_all = True
         validate_assignment = True
 
     paid_at_must_be_iso8601 = validator('paid_at', allow_reuse=True)(check_isoformat_none_case)
     expire_at_must_be_iso8601 = validator('expire_at', allow_reuse=True)(check_iso_format)
@@ -131,22 +157,14 @@
     pass
 
 
 class Receipt(OnlinePaymentBegin):
     pass
 
 
-class Confirm(OnlinePaymentBegin):
-    pass
-
-
-class Cancel(OnlinePaymentBegin):
-    pass
-
-
 class Notify(BaseModel):
     url: Optional[str]
     method: Optional[HttpMethodType]
     sent_at: Optional[str]
 
     sent_at_must_be_iso8601 = validator('sent_at', allow_reuse=True)(check_isoformat_none_case)
 
@@ -178,16 +196,14 @@
 class Links(BaseModel):
     online_payment_begin: OnlinePaymentBegin
     online_payment_landing: OnlinePaymentLanding
     offline_payment: OfflinePayment
     receipt: Receipt
     notify: Optional[List[Notify]]
     update: Update
-    confirm: Confirm
-    cancel: Cancel
 
     class Config:
         validate_all = True
         validate_assignment = True
 
     def append_notify(self, notify):
         for item in notify:
@@ -225,24 +241,23 @@
 
 
 class Payment(BaseModel):
     id: UUID
     user_id: UUID
     type: PaymentType
     tenant_id: UUID
-    service_id: UUID
+    remote_collection: RemoteCollectionType
     created_at: str
     updated_at: str
     status: PaymentStatus
     reason: constr(max_length=140)
     remote_id: UUID
     payment: PaymentData
     links: Links
     payer: Payer
-    locale: str = None
     event_id: UUID
     event_version: str
     event_created_at: str
     app_id: str
 
     class Config:
         validate_all = True
```

### Comparing `oc_python_sdk-2.1.0/oc_python_sdk.egg-info/PKG-INFO` & `oc_python_sdk-3.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oc_python_sdk
-Version: 2.1.0
+Version: 3.0.0
 Summary: Python SDK
 Home-page: https://gitlab.com/opencity-labs/area-personale/python_sdk
 Author: Opencontent
 Author-email: emily.lancietti@opencontent.it
 License: GNU GPLv3 License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `oc_python_sdk-2.1.0/setup.py` & `oc_python_sdk-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `oc_python_sdk-2.1.0/tests/_helpers.py` & `oc_python_sdk-3.0.0/tests/_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,24 +52,37 @@
         'outcome_protocolled_at': None,
         'payment_type': None,
         'payment_data': {
             'reason': 'PagamentoTari-3c819c1d-6587-448d-8ba4-3b6f23e87ed4',
             'amount': '10',
             'expire_at': '2022-04-28T11:18:41+02:00',
             'split': [{'code': '2020/1', 'amount': '8', 'meta': {}}, {'code': '2020/2', 'amount': '2', 'meta': {}}],
+            'stamps': [
+                {
+                    'amount': '16',
+                    'collection_data': '9/123',
+                    'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
+                },
+                {
+                    'amount': '16',
+                    'collection_data': '9/123',
+                    'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
+                },
+            ],
             'notify': {
                 'url': 'https://www2.stanzadelcittadino.it'
                 '/comune-di-bugliano/api/applications/3c819c1d-6587-448d-8ba4-3b6f23e87ed4/payment',
                 'method': 'POST',
             },
             'landing': {
                 'url': 'https://www2.stanzadelcittadino.it'
                 '/comune-di-bugliano/pratiche/3c819c1d-6587-448d-8ba4-3b6f23e87ed4/detail',
                 'method': 'GET',
             },
+            'config_id': 'cf9ece67-1956-49c9-af89-a19120485fef',
         },
         'status': '1500',
         'status_name': 'status_payment_pending',
         'authentication': {
             'authentication_method': 'spid',
             'session_id': 'abc123abc123abc123abc123abc123abc123abc123',
             'spid_code': '123456789',
@@ -81,15 +94,14 @@
             'session_index': 'abc123abc123abc123abc123abc123abc123abc123',
         },
         'links': [],
         'meetings': [],
         'integrations': [],
         'backoffice_data': None,
         'flow_changed_at': '2022-04-28T11:18:41+02:00',
-        'locale': 'IT',
         'event_version': '2.0',
         'event_id': 'bb7044e4-066c-4bf7-915e-87ee97270eae',
         **kwargs,
     }
 
 
 def get_application_minimal_applicant_data(**kwargs):
@@ -104,35 +116,51 @@
 
 def get_application_payment_data(**kwargs):
     return {
         'reason': 'PagamentoTari-3c819c1d-6587-448d-8ba4-3b6f23e87ed4',
         'amount': '10',
         'expire_at': '2022-04-28T11:18:41+02:00',
         'split': [{'code': '2020/1', 'amount': '8', 'meta': {}}, {'code': '2020/2', 'amount': '2', 'meta': {}}],
+        'stamps': [
+            {
+                'amount': '16',
+                'collection_data': '9/123',
+                'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
+            },
+            {
+                'amount': '16',
+                'collection_data': '9/123',
+                'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
+            },
+        ],
         'notify': {
             'url': 'https://www2.stanzadelcittadino.it'
             '/comune-di-bugliano/api/applications/3c819c1d-6587-448d-8ba4-3b6f23e87ed4/payment',
             'method': 'POST',
         },
         'landing': {
             'url': 'https://www2.stanzadelcittadino.it'
             '/comune-di-bugliano/pratiche/3c819c1d-6587-448d-8ba4-3b6f23e87ed4/detail',
             'method': 'GET',
         },
+        'config_id': 'cf9ece67-1956-49c9-af89-a19120485fef',
         **kwargs,
     }
 
 
 def get_payment_event_data(**kwargs):
     return {
         'id': 'bb7044e4-066c-4bf7-915e-87ee97270eae',
         'user_id': '43f619df-3ba2-4d9d-bcdd-270484eac44d',
         'type': 'PAGOPA',
         'tenant_id': '2eeb8374-c8f9-4260-9e94-22504e262eb1',
-        'service_id': 'cf9ece67-1956-49c9-af89-a19120485fef',
+        'remote_collection': {
+            'id': 'cf9ece67-1956-49c9-af89-a19120485fef',
+            'type': 'application',
+        },
         'created_at': '2022-06-08T08:28:42+00:00',
         'updated_at': '2022-06-08T10:29:39+02:00',
         'status': 'CREATION_PENDING',
         'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
         'remote_id': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472',
         'payment': {
             'transaction_id': None,
@@ -140,14 +168,15 @@
             'expire_at': '2022-09-06T10:28:42+02:00',
             'amount': 1,
             'currency': 'EUR',
             'notice_code': None,
             'iud': 'bb7044e4066c4bf7915e87ee97270eae',
             'iuv': None,
             'split': [],
+            'stamps': [],
         },
         'links': {
             'online_payment_begin': {'url': None, 'last_opened_at': None, 'method': 'GET'},
             'online_payment_landing': {
                 'url': 'https://devsdc.opencontent.it/'
                 'comune-di-bugliano/it/pratiche/a51cc065-4fb1-4ace-8d3f-e3a70c867472/detail',
                 'last_opened_at': None,
@@ -160,31 +189,28 @@
                     'url': 'https://devsdc.opencontent.it/'
                     'comune-di-bugliano/api/applications/a51cc065-4fb1-4ace-8d3f-e3a70c867472/payment',
                     'method': 'POST',
                     'sent_at': None,
                 },
             ],
             'update': {'url': None, 'last_check_at': None, 'next_check_at': None, 'method': 'GET'},
-            'confirm': {'url': None, 'last_check_at': None, 'next_check_at': None, 'method': 'POST'},
-            'cancel': {'url': None, 'last_check_at': None, 'next_check_at': None, 'method': 'POST'},
         },
         'payer': {
             'type': 'human',
             'tax_identification_number': 'SLVLNZ76P01G843V',
             'name': 'Lorenzo',
             'family_name': 'Salvadorini',
             'street_name': None,
             'building_number': None,
             'postal_code': None,
             'town_name': None,
             'country_subdivision': None,
             'country': 'IT',
             'email': 'raffaele.luccisano@opencontent.it',
         },
-        'locale': 'IT',
         'event_id': 'c5cebc1a-5d6f-4921-bc15-ff0575ea6f75',
         'event_version': '2.0',
         'event_created_at': '2022-06-08T08:28:42+00:00',
         'app_id': 'payment-dispatcher:1.0.15',
         **kwargs,
     }
 
@@ -196,14 +222,15 @@
         'expire_at': '2022-09-06T10:28:42+02:00',
         'amount': 1,
         'currency': 'EUR',
         'notice_code': None,
         'iud': 'bb7044e4066c4bf7915e87ee97270eae',
         'iuv': None,
         'split': [],
+        'stamps': [],
         **kwargs,
     }
 
 
 def get_split_data(**kwargs):
     return {
         'amount': 1,
@@ -244,14 +271,41 @@
                 'split_budget_chapter': 'Capitolo di bilancio c2',
                 'split_assessment': 'Accertamento c2',
             },
         },
     ]
 
 
+def get_stamps_data(**kwargs):
+    return {
+        'amount': 16,
+        'collection_data': '9/123',
+        'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
+        'meta': {},
+        **kwargs,
+    }
+
+
+def get_stamps_data_complete():
+    return [
+        {
+            'amount': '16.00',
+            'collection_data': '9/123',
+            'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
+            'meta': {},
+        },
+        {
+            'amount': '16.00',
+            'collection_data': '9/123',
+            'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
+            'meta': {},
+        },
+    ]
+
+
 def get_payer_data(**kwargs):
     return {
         'type': 'human',
         'tax_identification_number': 'SLVLNZ76P01G843V',
         'name': 'Lorenzo',
         'family_name': 'Salvadorini',
         'street_name': None,
@@ -281,16 +335,14 @@
                 'url': 'https://devsdc.opencontent.it/'
                 'comune-di-bugliano/api/applications/a51cc065-4fb1-4ace-8d3f-e3a70c867472/payment',
                 'method': 'POST',
                 'sent_at': None,
             },
         ],
         'update': {'url': None, 'last_check_at': None, 'next_check_at': None, 'method': 'GET'},
-        'confirm': {'url': None, 'last_check_at': None, 'next_check_at': None, 'method': 'POST'},
-        'cancel': {'url': None, 'last_check_at': None, 'next_check_at': None, 'method': 'POST'},
         **kwargs,
     }
 
 
 def get_online_payment_begin_data(**kwargs):
     return {'url': None, 'last_opened_at': None, 'method': 'GET', **kwargs}
```

### Comparing `oc_python_sdk-2.1.0/tests/test_application.py` & `oc_python_sdk-3.0.0/tests/test_application.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 
 class ApplicationTestCase(TestCase):
     def test_creation(self):
         application = Application(**get_application_data())
         payment_data_v2 = APaymentData(**get_application_payment_data(split=get_split_data_invalid()))
         application_v2 = Application(**get_application_data(payment_data=payment_data_v2))
         payment_data_empty_split = APaymentData(**get_application_payment_data(split=[]))
+        payment_data_empty_stamps = APaymentData(**get_application_payment_data(stamps=[]))
         applicant_minimal_data = Applicant(**get_application_minimal_applicant_data())
         self.assertEqual(application.id, UUID('3c819c1d-6587-448d-8ba4-3b6f23e87ed4'))
         self.assertEqual(application_v2.payment_data.split, {'c_1': 14.0, 'c_2': None})
         self.assertEqual(payment_data_empty_split.split, [])
+        self.assertEqual(payment_data_empty_stamps.stamps, [])
         with self.assertRaises(ValidationError):
             APaymentData(
                 **get_application_payment_data(
                     split='Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt '
                     'ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco '
                     'laboris nisi ut aliquip ex ea commodo consequat.',
                 ),
```

### Comparing `oc_python_sdk-2.1.0/tests/test_payment.py` & `oc_python_sdk-3.0.0/tests/test_payment.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Notify,
     OnlinePaymentBegin,
     Payer,
     PayerType,
     Payment,
     PaymentData,
     PaymentDataSplit,
+    PaymentDataStamp,
     PaymentStatus,
     PaymentType,
     Update,
 )
 
 from ._helpers import (
     get_empty_notify_data,
@@ -29,14 +30,16 @@
     get_online_payment_begin_data,
     get_payer_data,
     get_payment_data,
     get_payment_event_data,
     get_split_data,
     get_split_data_complete,
     get_split_data_invalid,
+    get_stamps_data,
+    get_stamps_data_complete,
     get_update_data,
 )
 
 NOW = datetime(2022, 9, 19, 16, 0, 0, tzinfo=timezone.utc)
 
 
 class PaymentTestCase(TestCase):
@@ -125,33 +128,40 @@
     def test_payer_country(self):
         with self.assertRaises(ValidationError):
             Payer(**get_payer_data(country='XX'))
 
     def test_encoders(self):
         payment = Payment(**get_payment_event_data())
         empty_split = payment.payment.split
+        empty_stamps = payment.payment.stamps
 
         payment_empty_notify = Payment(**get_payment_event_data())
         payment_empty_notify.links.notify = None
 
         payment_data_with_split = payment.payment
         payment_data_with_split.split = get_split_data_complete()
         payment_with_split = Payment(**get_payment_event_data(payment=payment_data_with_split))
 
+        payment_data_with_stamps = payment.payment
+        payment_data_with_stamps.stamps = get_stamps_data_complete()
+        payment_with_stamps = Payment(**get_payment_event_data(payment=payment_data_with_stamps))
+
         payment_data = PaymentData(**get_payment_data())
         split = PaymentDataSplit(**get_split_data())
+        stamps = PaymentDataStamp(**get_stamps_data())
         online_payment_begin = OnlinePaymentBegin(**get_online_payment_begin_data())
         notify = Notify(**get_notify_data())
         notify_no_data = Notify(**get_empty_notify_data())
         update = Update(**get_update_data())
         links = Links(**get_links_data())
         payer = Payer(**get_payer_data())
 
         self.assertEqual(json.loads(payment.json())['id'], 'bb7044e4-066c-4bf7-915e-87ee97270eae')
         self.assertEqual(empty_split, [])
+        self.assertEqual(empty_stamps, [])
         self.assertEqual(
             json.loads(payment_with_split.json())['payment']['split'],
             [
                 {
                     'code': 'c_1',
                     'amount': 16.0,
                     'meta': {
@@ -171,22 +181,40 @@
                         'split_description': 'Descrizione c12',
                         'split_budget_chapter': 'Capitolo di bilancio c2',
                         'split_assessment': 'Accertamento c2',
                     },
                 },
             ],
         )
+        self.assertEqual(
+            json.loads(payment_with_stamps.json())['payment']['stamps'],
+            [
+                {
+                    'amount': 16.0,
+                    'collection_data': '9/123',
+                    'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
+                    'meta': {},
+                },
+                {
+                    'amount': 16.0,
+                    'collection_data': '9/123',
+                    'reason': 'a51cc065-4fb1-4ace-8d3f-e3a70c867472 - SLVLNZ76P01g843v',
+                    'meta': {},
+                },
+            ],
+        )
         self.assertEqual(json.loads(payment.json())['created_at'], '2022-06-08T08:28:42+00:00')
         self.assertEqual(json.loads(payment.status.json()), PaymentStatus.STATUS_CREATION_PENDING.value)
         self.assertEqual(json.loads(payment.type.json()), PaymentType.TYPE_PAGOPA.value)
         self.assertEqual(json.loads(payment.payer.type.json()), PayerType.TYPE_HUMAN.value)
         self.assertEqual(json.loads(payment.payment.currency.json()), CurrencyType.CURRENCY_EUR.value)
         self.assertEqual(json.loads(payment.links.notify[0].method.json()), HttpMethodType.HTTP_METHOD_POST.value)
         self.assertEqual(json.loads(payment_empty_notify.json())['links']['notify'], None)
         self.assertEqual(json.loads(split.json())['code'], 'CODE')
+        self.assertEqual(json.loads(stamps.json())['collection_data'], '9/123')
         self.assertEqual(json.loads(payment_data.json())['amount'], 1)
         self.assertEqual(json.loads(online_payment_begin.json())['url'], None)
         self.assertEqual(
             json.loads(notify.json())['url'],
             'https://devsdc.opencontent.it/'
             'comune-di-bugliano/api/applications/'
             'a51cc065-4fb1-4ace-8d3f-e3a70c867472/payment',
```


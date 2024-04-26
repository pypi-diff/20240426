# Comparing `tmp/python_trading212-0.1.0.tar.gz` & `tmp/python_trading212-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_trading212-0.1.0.tar", max compression
+gzip compressed data, was "python_trading212-0.1.1.tar", max compression
```

## Comparing `python_trading212-0.1.0.tar` & `python_trading212-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      386 2024-04-25 13:35:24.617277 python_trading212-0.1.0/README.md
--rw-r--r--   0        0        0      449 2024-04-25 13:35:24.617277 python_trading212-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       98 2024-04-25 13:35:24.617277 python_trading212-0.1.0/python_trading212/__init__.py
--rw-r--r--   0        0        0     1598 2024-04-25 13:35:24.617277 python_trading212-0.1.0/python_trading212/models.py
--rw-r--r--   0        0        0     7163 2024-04-25 13:35:24.617277 python_trading212-0.1.0/python_trading212/trading212.py
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 python_trading212-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      386 2024-04-26 08:33:17.850601 python_trading212-0.1.1/README.md
+-rw-r--r--   0        0        0      449 2024-04-26 08:33:17.850601 python_trading212-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-04-26 08:33:17.850601 python_trading212-0.1.1/python_trading212/__init__.py
+-rw-r--r--   0        0        0     1660 2024-04-26 08:33:17.850601 python_trading212-0.1.1/python_trading212/models.py
+-rw-r--r--   0        0        0     7163 2024-04-26 08:33:17.850601 python_trading212-0.1.1/python_trading212/trading212.py
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 python_trading212-0.1.1/PKG-INFO
```

### Comparing `python_trading212-0.1.0/python_trading212/models.py` & `python_trading212-0.1.1/python_trading212/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 from typing import List, Optional
 from pydantic import BaseModel
 
 
 class Position(BaseModel):
-    averagePrice: int
-    currentPrice: int
+    averagePrice: float
+    currentPrice: float
     frontend: str
-    fxPpl: Optional[int]
+    fxPpl: Optional[float]
     initialFillDate: str
-    maxBuy: int
-    maxSell: int
-    pieQuantity: int
-    ppl: int
-    quantity: int
+    maxBuy: float
+    maxSell: float
+    pieQuantity: float
+    ppl: float
+    quantity: float
     ticker: str
 
 
 class TimeEvent(BaseModel):
     date: str
     type: str
 
@@ -33,66 +33,66 @@
     workingSchedules: Optional[List[WorkingSchedule]]
 
 
 class Instrument(BaseModel):
     addedOn: str
     currencyCode: str
     isin: str
-    maxOpenQuantity: int
-    minTradeQuantity: int
+    maxOpenQuantity: float
+    minTradeQuantity: float
     name: str
     shortname: str
     ticker: str
     type: str
     workingScheduleId: int
 
 
 class DividendDetails(BaseModel):
-    gained: int
-    inCash: int
-    reinvested: int
+    gained: float
+    inCash: float
+    reinvested: float
 
 
 class Result(BaseModel):
-    investedValue: int
-    result: int
-    resultCoef: int
-    value: int
+    investedValue: float
+    result: float
+    resultCoef: float
+    value: float
 
 
 class Pie(BaseModel):
-    cash: int
+    cash: float
     dividendDetails: DividendDetails
     id: int
     progress: float
     result: Result
     status: str
 
 
 class Order(BaseModel):
     creationTime: str
-    filledQuantity: int
-    filledValue: int
+    filledQuantity: float
+    filledValue: float
     id: int
-    limitPrice: int
-    quantity: int
+    limitPrice: float
+    quantity: float
     status: str
-    stopPrice: int
+    stopPrice: float
     strategy: str
     ticker: str
     type: str
-    value: int
+    value: float
 
 
 class AccountCash(BaseModel):
-    blocked: int
-    free: int
-    invested: int
-    pieCash: int
-    ppl: int
-    result: int
-    total: int
+    blocked: float
+    free: float
+    invested: float
+    pieCash: float
+    ppl: float
+    result: float
+    total: float
 
 
 class AccountMetadata(BaseModel):
     currencyCode: str
     id: int
```

### Comparing `python_trading212-0.1.0/python_trading212/trading212.py` & `python_trading212-0.1.1/python_trading212/trading212.py`

 * *Files identical despite different names*

### Comparing `python_trading212-0.1.0/PKG-INFO` & `python_trading212-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-trading212
-Version: 0.1.0
+Version: 0.1.1
 Summary: An unofficial client for the official Trading212 API
 Author: José Coelho
 Author-email: 16445494+jcoelho93@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
```


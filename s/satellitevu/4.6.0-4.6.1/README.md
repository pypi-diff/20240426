# Comparing `tmp/satellitevu-4.6.0.tar.gz` & `tmp/satellitevu-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellitevu-4.6.0.tar", max compression
+gzip compressed data, was "satellitevu-4.6.1.tar", max compression
```

## Comparing `satellitevu-4.6.0.tar` & `satellitevu-4.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1080 2024-04-12 09:46:25.230065 satellitevu-4.6.0/LICENSE
--rw-r--r--   0        0        0     3934 2024-04-12 09:46:25.230065 satellitevu-4.6.0/README.md
--rw-r--r--   0        0        0     1082 2024-04-12 09:46:32.958052 satellitevu-4.6.0/pyproject.toml
--rw-r--r--   0        0        0       80 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/archive.py
--rw-r--r--   0        0        0     3012 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/archive_test.py
--rw-r--r--   0        0        0     1519 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/base.py
--rw-r--r--   0        0        0     1287 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/base_test.py
--rw-r--r--   0        0        0     3788 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/catalog.py
--rw-r--r--   0        0        0     3123 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/catalog_test.py
--rw-r--r--   0        0        0     1331 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/contracts.py
--rw-r--r--   0        0        0      814 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/exceptions.py
--rw-r--r--   0        0        0     7623 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/orders.py
--rw-r--r--   0        0        0    11483 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/orders_test.py
--rw-r--r--   0        0        0    24289 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/otm.py
--rw-r--r--   0        0        0    13873 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/apis/otm_test.py
--rw-r--r--   0        0        0      149 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/auth/__init__.py
--rw-r--r--   0        0        0     2799 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/auth/auth.py
--rw-r--r--   0        0        0     1664 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/auth/auth_test.py
--rw-r--r--   0        0        0     1956 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/auth/cache.py
--rw-r--r--   0        0        0     2144 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/auth/cache_test.py
--rw-r--r--   0        0        0      122 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/auth/exc.py
--rw-r--r--   0        0        0     3004 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/client.py
--rw-r--r--   0        0        0     1363 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/config.py
--rw-r--r--   0        0        0     5073 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/conftest.py
--rw-r--r--   0        0        0      148 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/http/__init__.py
--rw-r--r--   0        0        0     2038 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/http/base.py
--rw-r--r--   0        0        0     3327 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/http/http_test.py
--rw-r--r--   0        0        0     1305 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/http/httpx.py
--rw-r--r--   0        0        0     1334 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/http/requests.py
--rw-r--r--   0        0        0     1744 2024-04-12 09:46:25.230065 satellitevu-4.6.0/satellitevu/http/urllib.py
--rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 satellitevu-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-26 13:10:23.664295 satellitevu-4.6.1/LICENSE
+-rw-r--r--   0        0        0     3934 2024-04-26 13:10:23.664295 satellitevu-4.6.1/README.md
+-rw-r--r--   0        0        0     1082 2024-04-26 13:10:33.340248 satellitevu-4.6.1/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/archive.py
+-rw-r--r--   0        0        0     3012 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/archive_test.py
+-rw-r--r--   0        0        0     1519 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/base.py
+-rw-r--r--   0        0        0     1287 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/base_test.py
+-rw-r--r--   0        0        0     3788 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/catalog.py
+-rw-r--r--   0        0        0     3123 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/catalog_test.py
+-rw-r--r--   0        0        0     1331 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/contracts.py
+-rw-r--r--   0        0        0      814 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/exceptions.py
+-rw-r--r--   0        0        0     7623 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/orders.py
+-rw-r--r--   0        0        0    11483 2024-04-26 13:10:23.664295 satellitevu-4.6.1/satellitevu/apis/orders_test.py
+-rw-r--r--   0        0        0    24308 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/apis/otm.py
+-rw-r--r--   0        0        0    13873 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/apis/otm_test.py
+-rw-r--r--   0        0        0      149 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/__init__.py
+-rw-r--r--   0        0        0     2799 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/auth.py
+-rw-r--r--   0        0        0     1664 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/auth_test.py
+-rw-r--r--   0        0        0     1956 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/cache.py
+-rw-r--r--   0        0        0     2144 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/cache_test.py
+-rw-r--r--   0        0        0      122 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/auth/exc.py
+-rw-r--r--   0        0        0     3004 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/client.py
+-rw-r--r--   0        0        0     1363 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/config.py
+-rw-r--r--   0        0        0     5073 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/conftest.py
+-rw-r--r--   0        0        0      148 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/__init__.py
+-rw-r--r--   0        0        0     2038 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/base.py
+-rw-r--r--   0        0        0     3327 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/http_test.py
+-rw-r--r--   0        0        0     1305 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/httpx.py
+-rw-r--r--   0        0        0     1334 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/requests.py
+-rw-r--r--   0        0        0     1744 2024-04-26 13:10:23.668295 satellitevu-4.6.1/satellitevu/http/urllib.py
+-rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 satellitevu-4.6.1/PKG-INFO
```

### Comparing `satellitevu-4.6.0/LICENSE` & `satellitevu-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/README.md` & `satellitevu-4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/pyproject.toml` & `satellitevu-4.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "satellitevu"
-version = "4.6.0"
+version = "4.6.1"
 description = "Client SDK for SatelliteVu's platform APIs"
 authors = ["Christian Wygoda <christian.wygoda@satellitevu.com>", "Zhelini Sivanesan <zhelini.sivanesan@satellitevu.com>", "James Harrison <james.harrison@satellitevu.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `satellitevu-4.6.0/satellitevu/apis/archive.py` & `satellitevu-4.6.1/satellitevu/apis/archive.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/archive_test.py` & `satellitevu-4.6.1/satellitevu/apis/archive_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/base.py` & `satellitevu-4.6.1/satellitevu/apis/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/base_test.py` & `satellitevu-4.6.1/satellitevu/apis/base_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/catalog.py` & `satellitevu-4.6.1/satellitevu/apis/catalog.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/catalog_test.py` & `satellitevu-4.6.1/satellitevu/apis/catalog_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/contracts.py` & `satellitevu-4.6.1/satellitevu/apis/contracts.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/exceptions.py` & `satellitevu-4.6.1/satellitevu/apis/exceptions.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/orders.py` & `satellitevu-4.6.1/satellitevu/apis/orders.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/orders_test.py` & `satellitevu-4.6.1/satellitevu/apis/orders_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/apis/otm.py` & `satellitevu-4.6.1/satellitevu/apis/otm.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         *,
         contract_id: Union[UUID, str],
         coordinates: Union[Tuple[float, float], Tuple[float, float, float]],
         date_from: Optional[datetime] = None,
         date_to: Optional[datetime] = None,
         day_night_mode: Literal["day", "night", "day-night"] = "day-night",
         product: Literal["standard", "assured"] = "standard",
-        max_cloud_cover: Optional[int] = None,
+        max_cloud_cover: Optional[int] = MAX_CLOUD_COVER_DEFAULT,
         min_off_nadir: Optional[int] = None,
         max_off_nadir: Optional[int] = None,
         min_gsd: Optional[float] = None,
         max_gsd: Optional[float] = None,
         signature: Optional[str] = None,
         **kwargs,
     ):
```

### Comparing `satellitevu-4.6.0/satellitevu/apis/otm_test.py` & `satellitevu-4.6.1/satellitevu/apis/otm_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/auth/auth.py` & `satellitevu-4.6.1/satellitevu/auth/auth.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/auth/auth_test.py` & `satellitevu-4.6.1/satellitevu/auth/auth_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/auth/cache.py` & `satellitevu-4.6.1/satellitevu/auth/cache.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/auth/cache_test.py` & `satellitevu-4.6.1/satellitevu/auth/cache_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/client.py` & `satellitevu-4.6.1/satellitevu/client.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/config.py` & `satellitevu-4.6.1/satellitevu/config.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/conftest.py` & `satellitevu-4.6.1/satellitevu/conftest.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/http/base.py` & `satellitevu-4.6.1/satellitevu/http/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/http/http_test.py` & `satellitevu-4.6.1/satellitevu/http/http_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/http/httpx.py` & `satellitevu-4.6.1/satellitevu/http/httpx.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/http/requests.py` & `satellitevu-4.6.1/satellitevu/http/requests.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/satellitevu/http/urllib.py` & `satellitevu-4.6.1/satellitevu/http/urllib.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.6.0/PKG-INFO` & `satellitevu-4.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satellitevu
-Version: 4.6.0
+Version: 4.6.1
 Summary: Client SDK for SatelliteVu's platform APIs
 License: MIT
 Author: Christian Wygoda
 Author-email: christian.wygoda@satellitevu.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


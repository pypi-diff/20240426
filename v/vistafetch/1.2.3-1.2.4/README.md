# Comparing `tmp/vistafetch-1.2.3.tar.gz` & `tmp/vistafetch-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vistafetch-1.2.3.tar", max compression
+gzip compressed data, was "vistafetch-1.2.4.tar", max compression
```

## Comparing `vistafetch-1.2.3.tar` & `vistafetch-1.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2023-11-04 08:09:33.327853 vistafetch-1.2.3/LICENSE
--rw-r--r--   0        0        0     7991 2023-11-04 08:09:33.327853 vistafetch-1.2.3/README.md
--rw-r--r--   0        0        0     2000 2023-11-04 08:09:59.728280 vistafetch-1.2.3/pyproject.toml
--rw-r--r--   0        0        0      139 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/__init__.py
--rw-r--r--   0        0        0     2297 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/client.py
--rw-r--r--   0        0        0      388 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/constants.py
--rw-r--r--   0        0        0      520 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/logs.py
--rw-r--r--   0        0        0      320 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/model/__init__.py
--rw-r--r--   0        0        0      516 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/model/asset/__init__.py
--rw-r--r--   0        0        0      746 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/model/asset/bond.py
--rw-r--r--   0        0        0      612 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/model/asset/derivative.py
--rw-r--r--   0        0        0     5940 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/model/asset/financial_asset.py
--rw-r--r--   0        0        0      965 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/model/asset/financial_asset_type.py
--rw-r--r--   0        0        0     2100 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/model/asset/financial_data.py
--rw-r--r--   0        0        0      794 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/model/asset/fund.py
--rw-r--r--   0        0        0      546 2023-11-04 08:09:33.327853 vistafetch-1.2.3/vistafetch/model/asset/index.py
--rw-r--r--   0        0        0      692 2023-11-04 08:09:33.331853 vistafetch-1.2.3/vistafetch/model/asset/metal.py
--rw-r--r--   0        0        0      584 2023-11-04 08:09:33.331853 vistafetch-1.2.3/vistafetch/model/asset/stock.py
--rw-r--r--   0        0        0     2210 2023-11-04 08:09:33.331853 vistafetch-1.2.3/vistafetch/model/base.py
--rw-r--r--   0        0        0     2605 2023-11-04 08:09:33.331853 vistafetch-1.2.3/vistafetch/model/search_result.py
--rw-r--r--   0        0        0        0 2023-11-04 08:09:33.331853 vistafetch-1.2.3/vistafetch/py.typed
--rw-r--r--   0        0        0      210 2023-11-04 08:09:33.331853 vistafetch-1.2.3/vistafetch/session.py
--rw-r--r--   0        0        0     9384 1970-01-01 00:00:00.000000 vistafetch-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-26 08:10:13.262311 vistafetch-1.2.4/LICENSE
+-rw-r--r--   0        0        0     7991 2024-04-26 08:10:13.262311 vistafetch-1.2.4/README.md
+-rw-r--r--   0        0        0     2007 2024-04-26 08:10:33.754198 vistafetch-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0      139 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/__init__.py
+-rw-r--r--   0        0        0     2298 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/client.py
+-rw-r--r--   0        0        0      388 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/constants.py
+-rw-r--r--   0        0        0      520 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/logs.py
+-rw-r--r--   0        0        0      320 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/bond.py
+-rw-r--r--   0        0        0      612 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/derivative.py
+-rw-r--r--   0        0        0     5940 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/financial_asset.py
+-rw-r--r--   0        0        0      965 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/financial_asset_type.py
+-rw-r--r--   0        0        0     2100 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/financial_data.py
+-rw-r--r--   0        0        0      794 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/fund.py
+-rw-r--r--   0        0        0      546 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/index.py
+-rw-r--r--   0        0        0      692 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/metal.py
+-rw-r--r--   0        0        0      584 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/asset/stock.py
+-rw-r--r--   0        0        0     2212 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/base.py
+-rw-r--r--   0        0        0     2606 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/model/search_result.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/py.typed
+-rw-r--r--   0        0        0      210 2024-04-26 08:10:13.266311 vistafetch-1.2.4/vistafetch/session.py
+-rw-r--r--   0        0        0     9384 1970-01-01 00:00:00.000000 vistafetch-1.2.4/PKG-INFO
```

### Comparing `vistafetch-1.2.3/LICENSE` & `vistafetch-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/README.md` & `vistafetch-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/pyproject.toml` & `vistafetch-1.2.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 in-place = true
 remove-all-unused-imports = true
 remove-duplicate-keys = true
 remove-unused-variables = true
 
 [tool.poetry]
 name = "vistafetch"
-version = "1.2.3"
+version = "1.2.4"
 description = "Small & simple library to fetch financial data for stocks, ETFs, funds, etc. from Onvista."
 authors = ["bossenti <bossenti@apache.org>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 repository = "https://github.com/bossenti/vistafetch"
 documentation = "https://github.com/bossenti/vistafetch#readme"
@@ -47,27 +47,27 @@
 requests = ">=2.31.0"
 rich = ">=13.0.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-autoflake = "2.2.1"
-mypy = "1.6.1"
+autoflake = "2.3.1"
+mypy = "1.10.0"
 pre-commit = "3.5.0"
-pytest = "7.4.3"
-pytest-cov = "4.1.0"
-ruff = "0.1.4"
-types-requests = "2.31.0.10"
+pytest = "8.1.1"
+pytest-cov = "5.0.0"
+ruff = "0.4.2"
+types-requests = "2.31.0.20240406"
 
 [tool.poetry.group.release]
 optional = true
 
 [tool.poetry.group.release.dependencies]
-twine = "4.0.2"
+twine = "5.0.0"
 
 [tool.ruff]
 select = ["C90", "D", "E", "F", "I", "ICN", "N", "PL", "UP"]
 ignore = [
     "D107",
     "D203", # ignore in favour of D211
     "D213", # ignore in favour of D212
```

### Comparing `vistafetch-1.2.3/vistafetch/client.py` & `vistafetch-1.2.4/vistafetch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class VistaFetchClient:
     """Client to fetch financial data from the Onvista API.
 
     Args:
     ----
         client_headers: additional headers to be sent with every request, optional
+
     """
 
     def __init__(
         self,
         client_headers: Optional[Dict[str, str]] = None,
         logging_level: Optional[int] = None,
     ):
```

### Comparing `vistafetch-1.2.3/vistafetch/logs.py` & `vistafetch-1.2.4/vistafetch/logs.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/__init__.py` & `vistafetch-1.2.4/vistafetch/model/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/bond.py` & `vistafetch-1.2.4/vistafetch/model/asset/bond.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/derivative.py` & `vistafetch-1.2.4/vistafetch/model/asset/derivative.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/financial_asset.py` & `vistafetch-1.2.4/vistafetch/model/asset/financial_asset.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/financial_asset_type.py` & `vistafetch-1.2.4/vistafetch/model/asset/financial_asset_type.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/financial_data.py` & `vistafetch-1.2.4/vistafetch/model/asset/financial_data.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/fund.py` & `vistafetch-1.2.4/vistafetch/model/asset/fund.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/index.py` & `vistafetch-1.2.4/vistafetch/model/asset/index.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/metal.py` & `vistafetch-1.2.4/vistafetch/model/asset/metal.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/asset/stock.py` & `vistafetch-1.2.4/vistafetch/model/asset/stock.py`

 * *Files identical despite different names*

### Comparing `vistafetch-1.2.3/vistafetch/model/base.py` & `vistafetch-1.2.4/vistafetch/model/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         This method returns the attributes of the entity data model as JSON string.
         It excludes additional parameters that are returned by the API but not modelled.
         Use `extra()` to get access to additional price-related data.
 
         Returns
         -------
             model_json: The model instance represented as JSON string
+
         """
         # By default, Pydantic includes additional parameters as well in the JSON dump
         # https://github.com/pydantic/pydantic/issues/6150
         # Therefore, we need to exclude them by hand
         return self.model_dump_json(
             exclude=set(self.model_extra.keys() if self.model_extra else [])
         )
@@ -69,9 +70,10 @@
 
         Extra data is exactly as returned by the API,
         no modifications are applied.
 
         Returns
         -------
             extra: dictionary containing additional data.
+
         """
         return self.model_extra if self.model_extra else {}
```

### Comparing `vistafetch-1.2.3/vistafetch/model/search_result.py` & `vistafetch-1.2.4/vistafetch/model/search_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
     def visualize(self) -> None:
         """Visualize the search result in the console.
 
         Returns
         -------
             None
+
         """
         console = Console()
 
         table = Table(title="Financial assets discovered")
 
         table.add_column("Index", justify="center")
         table.add_column("Name", justify="center")
```

### Comparing `vistafetch-1.2.3/PKG-INFO` & `vistafetch-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vistafetch
-Version: 1.2.3
+Version: 1.2.4
 Summary: Small & simple library to fetch financial data for stocks, ETFs, funds, etc. from Onvista.
 Home-page: https://github.com/bossenti/vistafetch
 License: Apache 2.0
 Keywords: etf,exchange,financial-data,funds,onvista,stocks
 Author: bossenti
 Author-email: bossenti@apache.org
 Requires-Python: >=3.8,<3.13
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vistafetch Version: 1.2.3 Summary: Small & simple
+Metadata-Version: 2.1 Name: vistafetch Version: 1.2.4 Summary: Small & simple
 library to fetch financial data for stocks, ETFs, funds, etc. from Onvista.
 Home-page: https://github.com/bossenti/vistafetch License: Apache 2.0 Keywords:
 etf,exchange,financial-data,funds,onvista,stocks Author: bossenti Author-email:
 bossenti@apache.org Requires-Python: >=3.8,<3.13 Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Console Classifier: Framework ::
 Pydantic :: 2 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Financial and Insurance Industry Classifier: Intended Audience ::
```


# Comparing `tmp/parcllabs-0.1.6.tar.gz` & `tmp/parcllabs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parcllabs-0.1.6.tar", last modified: Thu Apr 25 19:33:17 2024, max compression
+gzip compressed data, was "parcllabs-0.1.7.tar", last modified: Fri Apr 26 20:33:19 2024, max compression
```

## Comparing `parcllabs-0.1.6.tar` & `parcllabs-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:17.446097 parcllabs-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:32:36.000000 parcllabs-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 19:33:17.446097 parcllabs-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-25 19:32:36.000000 parcllabs-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:17.442097 parcllabs-0.1.6/parcllabs/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/plabs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:17.442097 parcllabs-0.1.6/parcllabs/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/search/metros.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/search/top_markets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:17.442097 parcllabs-0.1.6/parcllabs/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-25 19:33:13.000000 parcllabs-0.1.6/parcllabs/services/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/services/for_sale_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/services/investor_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/services/market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-25 19:32:36.000000 parcllabs-0.1.6/parcllabs/services/rental_market_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:17.442097 parcllabs-0.1.6/parcllabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 19:33:17.000000 parcllabs-0.1.6/parcllabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-25 19:33:17.000000 parcllabs-0.1.6/parcllabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:33:17.000000 parcllabs-0.1.6/parcllabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 19:33:17.000000 parcllabs-0.1.6/parcllabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 19:33:17.000000 parcllabs-0.1.6/parcllabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:33:17.446097 parcllabs-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-25 19:32:36.000000 parcllabs-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:17.442097 parcllabs-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-25 19:32:36.000000 parcllabs-0.1.6/tests/test_for_sale_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-25 19:32:36.000000 parcllabs-0.1.6/tests/test_parcl_labs_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-25 19:32:36.000000 parcllabs-0.1.6/tests/test_parcl_labs_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.440753 parcllabs-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 20:32:45.000000 parcllabs-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-26 20:33:19.436753 parcllabs-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-26 20:32:45.000000 parcllabs-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/parcllabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/plabs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/parcllabs/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/search/metros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/search/top_markets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/parcllabs/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-26 20:33:16.000000 parcllabs-0.1.7/parcllabs/services/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/for_sale_market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/investor_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/portfolio_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/rental_market_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/parcllabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:33:19.440753 parcllabs-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-26 20:32:45.000000 parcllabs-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-26 20:32:45.000000 parcllabs-0.1.7/tests/test_for_sale_market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-26 20:32:45.000000 parcllabs-0.1.7/tests/test_parcl_labs_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 20:32:45.000000 parcllabs-0.1.7/tests/test_parcl_labs_service.py
```

### Comparing `parcllabs-0.1.6/LICENSE` & `parcllabs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/PKG-INFO` & `parcllabs-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parcllabs
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python SDK for ParclLabs API
 Home-page: https://github.com/ParclLabs/parcllabs-python
 Author: ParclLabs
 Author-email: team@parcllabs.com
 Keywords: parcllabs api real estate analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `parcllabs-0.1.6/README.md` & `parcllabs-0.1.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 ![Logo](img/labs.jpg)
 # parcllabs-python
 
 ## Sign Up for an API Key
 
 To use the ParclLabs API, you need an API key. To get an API key, sign up at [ParclLabs](https://dashboard.parcllabs.com/signup).
 
-## Rental Market Metrics
+## Installation
 
-### Gross Yield
+You can install the package via pip:
+
+```bash
+pip install parcllabs
+```
+
+### Rental Market Metrics
+
+#### Gross Yield
 Gets the percent gross yield for a specified <parcl_id>. At the market level, identified by <parcl_id>, gross yield is calculated by dividing the annual median rental income—derived from multiplying the monthly median new rental listing price by 12—by its median new listings for sale price.
 
-### Rental Units Concentration
+#### Rental Units Concentration
 Gets the number of rental units, total units, and percent rental unit concentration for a specified <parcl_id>.
 
-#### Get all rental market metrics
+##### Get all rental market metrics
 ```python
 import os
 
 from parcllabs.search.top_markets import get_top_n_metros
 from parcllabs import ParclLabsClient
 
 api_key = os.getenv('PARCLLABS_API_KEY')
@@ -29,31 +37,33 @@
 
 start_date = '2020-01-01'
 end_date = '2024-04-01'
 
 results_rental_units_concentration = client.rental_market_metrics_rental_units_concentration.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
-    end_date=end_date
+    end_date=end_date,
+    as_dataframe=True
 )
 
 results_gross_yield = client.rental_market_metrics_gross_yield.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
-    end_date=end_date
+    end_date=end_date,
+    as_dataframe=True
 )
 ```
 
-## For Sale Market Metrics
+### For Sale Market Metrics
 
-### New Listings Rolling Counts
+#### New Listings Rolling Counts
 Gets weekly updated rolling counts of newly listed for sale properties, segmented into 7, 30, 60, and 90 day periods ending on a specified date, based on a given <parcl_id>.
 
 
-#### Get all for sale market metrics
+##### Get all for sale market metrics
 ```python
 import os
 
 from parcllabs.search.top_markets import get_top_n_metros
 from parcllabs import ParclLabsClient
 
 api_key = os.getenv('PARCLLABS_API_KEY')
@@ -66,31 +76,32 @@
 end_date = '2024-04-01'
 property_type = 'single_family'
 
 results_for_sale_new_listings = client.for_sale_market_metrics_new_listings_rolling_counts.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
     end_date=end_date,
-    property_type=property_type
+    property_type=property_type,
+    as_dataframe=True
 )
 ```
 
-## Market Metrics
+### Market Metrics
 
-### Housing Event Counts
+#### Housing Event Counts
 Gets monthly counts of housing events, including sales, new sale listings, and new rental listings, based on a specified <parcl_id>.
 
-### Housing Stock
+#### Housing Stock
 Gets housing stock for a specified <parcl_id>. Housing stock represents the total number of properties, broken out by single family homes, townhouses, and condos.
 
-### Housing Event Prices
+#### Housing Event Prices
 Gets monthly statistics on prices for housing events, including sales, new for-sale listings, and new rental listings, based on a specified <parcl_id>.
 
 
-#### Get all market metrics
+##### Get all market metrics
 ```python
 import os
 
 from parcllabs.search.top_markets import get_top_n_metros
 from parcllabs import ParclLabsClient
 
 
@@ -102,45 +113,48 @@
 
 start_date = '2020-01-01'
 end_date = '2024-04-01'
 
 results_housing_event_prices = client.market_metrics_housing_event_prices.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
-    end_date=end_date
+    end_date=end_date,
+    as_dataframe=True
 )
 
 results_housing_stock = client.market_metrics_housing_stock.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
-    end_date=end_date
+    end_date=end_date,
+    as_dataframe=True
 )
 
 results_housing_event_counts = client.market_metrics_housing_event_counts.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
-    end_date=end_date
+    end_date=end_date,
+    as_dataframe=True
 )
 ```
 
-## Investor Metrics
+### Investor Metrics
 
-### Housing Event Counts
+#### Housing Event Counts
 Gets monthly counts of investor housing events, including acquisitions, dispositions, new sale listings, and new rental listings, based on a specified <parcl_id>.
 
-### Purchase to Sale Ratio
+#### Purchase to Sale Ratio
 Gets the monthly investor purchase to sale ratio for a specified <parcl_id>.
 
-### New Listings for Sale Rolling Counts
+#### New Listings for Sale Rolling Counts
 Gets weekly updated rolling counts of investor-owned properties newly listed for sale, and their corresponding percentage share of the total for-sale listings market. These metrics are segmented into 7, 30, 60, and 90-day periods ending on a specified date, based on a given <parcl_id>
 
-### Housing Stock Ownership
+#### Housing Stock Ownership
 Gets counts of investor-owned properties and their corresponding percentage ownership share of the total housing stock, for a specified <parcl_id>.
 
-#### Get all investor metrics
+##### Get all investor metrics
 ```python
 import os
 
 from parcllabs.search.top_markets import get_top_n_metros
 from parcllabs import ParclLabsClient
 
 
@@ -152,28 +166,55 @@
 
 start_date = '2020-01-01'
 end_date = '2024-04-01'
 
 results_housing_stock_ownership = client.investor_metrics_housing_stock_ownership.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
-    end_date=end_date
+    end_date=end_date,
+    as_dataframe=True
 )
 
 results_new_listings_for_sale_rolling_counts = client.investor_metrics_new_listings_for_sale_rolling_counts.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
-    end_date=end_date
+    end_date=end_date,
+    as_dataframe=True
 )
 
 results_purchase_to_sale_ratio = client.investor_metrics_purchase_to_sale_ratio.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
-    end_date=end_date
+    end_date=end_date,
+    as_dataframe=True
 )
 
 results_housing_event_counts = client.investor_metrics_housing_event_counts.retrieve_many(
     parcl_ids=top_market_parcl_ids,
     start_date=start_date,
-    end_date=end_date
+    end_date=end_date,
+    as_dataframe=True
+)
+```
+
+#### Portfolio Metrics
+Gets counts of investor-owned single family properties and their corresponding percentage of the total single family housing stock, segmented by portfolio size, for a specified <parcl_id>. The data series for portfolio metrics begins on March 1, 2024 (2024-03-01).
+
+##### Single Family Home Portfolio Metrics
+```python
+import os
+
+from parcllabs.search.top_markets import get_top_n_metros
+from parcllabs import ParclLabsClient
+
+
+api_key = os.getenv('PARCLLABS_API_KEY')
+client = ParclLabsClient(api_key)
+
+top_markets = get_top_n_metros(n=10)
+top_market_parcl_ids = top_markets['parcl_id'].tolist()
+
+results_housing_stock_ownership = client.portfolio_metrics_sf_housing_stock_ownership.retrieve_many(
+    parcl_ids=top_market_parcl_ids,
+    as_dataframe=True
 )
 ```
```

### Comparing `parcllabs-0.1.6/parcllabs/__init__.py` & `parcllabs-0.1.7/parcllabs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,7 +28,9 @@
     ForSaleMarketMetricsNewListingsRollingCounts,
 )
 
 from parcllabs.services.rental_market_metrics import (
     RentalMarketMetricsRentalUnitsConcentration,
     RentalMarketMetricsGrossYield,
 )
+
+from parcllabs.services.portfolio_metrics import PortfolioMetricsSFHousingStockOwnership
```

### Comparing `parcllabs-0.1.6/parcllabs/plabs_client.py` & `parcllabs-0.1.7/parcllabs/plabs_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 )
 
 from parcllabs.services.rental_market_metrics import (
     RentalMarketMetricsRentalUnitsConcentration,
     RentalMarketMetricsGrossYield,
 )
 
+from parcllabs.services.portfolio_metrics import PortfolioMetricsSFHousingStockOwnership
+
 
 class ParclLabsClient:
     def __init__(self, api_key: str):
         if api_key is None:
             raise ValueError("api_key is required")
         self.api_key = api_key
         self.api_url = api_base
@@ -61,14 +63,17 @@
         )
         self.rental_market_metrics_rental_units_concentration = (
             RentalMarketMetricsRentalUnitsConcentration(client=self)
         )
         self.rental_market_metrics_gross_yield = RentalMarketMetricsGrossYield(
             client=self
         )
+        self.portfolio_metrics_sf_housing_stock_ownership = (
+            PortfolioMetricsSFHousingStockOwnership(client=self)
+        )
 
     def get(self, url: str, params: dict = None):
         """
         Send a GET request to the specified URL with the given parameters.
 
         Args:
             url (str): The URL endpoint to request.
```

### Comparing `parcllabs-0.1.6/parcllabs/search/metros.py` & `parcllabs-0.1.7/parcllabs/search/metros.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/parcllabs/services/base_service.py` & `parcllabs-0.1.7/parcllabs/services/base_service.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/parcllabs/services/for_sale_market_metrics.py` & `parcllabs-0.1.7/parcllabs/services/for_sale_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/parcllabs/services/investor_metrics.py` & `parcllabs-0.1.7/parcllabs/services/investor_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/parcllabs/services/market_metrics.py` & `parcllabs-0.1.7/parcllabs/services/market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/parcllabs/services/rental_market_metrics.py` & `parcllabs-0.1.7/parcllabs/services/rental_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/parcllabs.egg-info/PKG-INFO` & `parcllabs-0.1.7/parcllabs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parcllabs
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python SDK for ParclLabs API
 Home-page: https://github.com/ParclLabs/parcllabs-python
 Author: ParclLabs
 Author-email: team@parcllabs.com
 Keywords: parcllabs api real estate analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `parcllabs-0.1.6/parcllabs.egg-info/SOURCES.txt` & `parcllabs-0.1.7/parcllabs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 parcllabs/search/metros.py
 parcllabs/search/top_markets.py
 parcllabs/services/__init__.py
 parcllabs/services/base_service.py
 parcllabs/services/for_sale_market_metrics.py
 parcllabs/services/investor_metrics.py
 parcllabs/services/market_metrics.py
+parcllabs/services/portfolio_metrics.py
 parcllabs/services/rental_market_metrics.py
 tests/test_for_sale_market_metrics.py
 tests/test_parcl_labs_clients.py
 tests/test_parcl_labs_service.py
```

### Comparing `parcllabs-0.1.6/setup.py` & `parcllabs-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/tests/test_for_sale_market_metrics.py` & `parcllabs-0.1.7/tests/test_for_sale_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/tests/test_parcl_labs_clients.py` & `parcllabs-0.1.7/tests/test_parcl_labs_clients.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.6/tests/test_parcl_labs_service.py` & `parcllabs-0.1.7/tests/test_parcl_labs_service.py`

 * *Files identical despite different names*


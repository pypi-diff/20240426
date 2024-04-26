# Comparing `tmp/moneywiz_api-0.2.1.tar.gz` & `tmp/moneywiz_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneywiz_api-0.2.1.tar", last modified: Sun Apr 14 16:44:47 2024, max compression
+gzip compressed data, was "moneywiz_api-1.0.0.tar", last modified: Fri Apr 26 16:46:41 2024, max compression
```

## Comparing `moneywiz_api-0.2.1.tar` & `moneywiz_api-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.434098 moneywiz_api-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.434098 moneywiz_api-0.2.1/src/moneywiz_api/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/database_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/src/moneywiz_api/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/category_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/investment_holding_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/payee_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/record_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/tag_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/transaction_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/src/moneywiz_api/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/investment_holding.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/payee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/moneywiz_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-14 16:44:47.000000 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-14 16:44:47.000000 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:44:47.000000 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 16:44:47.000000 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.595223 moneywiz_api-1.0.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.595223 moneywiz_api-1.0.0/src/moneywiz_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.595223 moneywiz_api-1.0.0/src/moneywiz_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/database_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.595223 moneywiz_api-1.0.0/src/moneywiz_api/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/category_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/investment_holding_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/payee_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/record_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/tag_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/transaction_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/src/moneywiz_api/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/investment_holding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/payee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/raw_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/moneywiz_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/tests/test_config.py
```

### Comparing `moneywiz_api-0.2.1/LICENSE` & `moneywiz_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moneywiz_api-0.2.1/PKG-INFO` & `moneywiz_api-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 0.2.1
+Version: 1.0.0
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # MoneyWiz-API
 
 ![Static Badge](https://img.shields.io/badge/Python-3-blue?style=flat&logo=Python)
 ![PyPI](https://img.shields.io/pypi/v/moneywiz-api)
 
-
 <a href="https://www.buymeacoffee.com/Ileodo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
 
 A Python API to access MoneyWiz Sqlite database.
 
-
 ## Get Started
 
 ```bash
 pip install moneywiz-api
 ```
 
 ```python
@@ -52,10 +58,12 @@
 )
 
 record = accessor.get_record(record_id)
 print(record)
 
 ```
 
+It also offers a interactive shell `moneywiz-cli`.
+
 ## Contribution
 
 This project is in very early stage, all contributions are welcomed!
```

#### html2text {}

```diff
@@ -1,19 +1,23 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 0.2.1 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.0 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE # MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
-blue?style=flat&logo=Python) ![PyPI](https://img.shields.io/pypi/v/moneywiz-
-api) _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]A Python API to access MoneyWiz Sqlite database. ## Get
-Started ```bash pip install moneywiz-api ``` ```python from moneywiz_api import
-MoneywizApi moneywizApi = MoneywizApi("") ( accessor, account_manager,
-payee_manager, category_manager, transaction_manager,
-investment_holding_manager, ) = ( moneywizApi.accessor,
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: pandas Provides-Extra: dev Requires-Dist: pytest; extra
+== "dev" Requires-Dist: pylint; extra == "dev" Requires-Dist: mypy; extra ==
+"dev" Requires-Dist: black; extra == "dev" Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev" # MoneyWiz-API ![Static Badge](https://
+img.shields.io/badge/Python-3-blue?style=flat&logo=Python) ![PyPI](https://
+img.shields.io/pypi/v/moneywiz-api) _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]A Python API to access
+MoneyWiz Sqlite database. ## Get Started ```bash pip install moneywiz-api ```
+```python from moneywiz_api import MoneywizApi moneywizApi = MoneywizApi("")
+( accessor, account_manager, payee_manager, category_manager,
+transaction_manager, investment_holding_manager, ) = ( moneywizApi.accessor,
 moneywizApi.account_manager, moneywizApi.payee_manager,
 moneywizApi.category_manager, moneywizApi.transaction_manager,
 moneywizApi.investment_holding_manager, ) record = accessor.get_record
-(record_id) print(record) ``` ## Contribution This project is in very early
-stage, all contributions are welcomed!
+(record_id) print(record) ``` It also offers a interactive shell `moneywiz-
+cli`. ## Contribution This project is in very early stage, all contributions
+are welcomed!
```

### Comparing `moneywiz_api-0.2.1/README.md` & `moneywiz_api-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # MoneyWiz-API
 
 ![Static Badge](https://img.shields.io/badge/Python-3-blue?style=flat&logo=Python)
 ![PyPI](https://img.shields.io/pypi/v/moneywiz-api)
 
-
 <a href="https://www.buymeacoffee.com/Ileodo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
 
 A Python API to access MoneyWiz Sqlite database.
 
-
 ## Get Started
 
 ```bash
 pip install moneywiz-api
 ```
 
 ```python
@@ -38,10 +36,12 @@
 )
 
 record = accessor.get_record(record_id)
 print(record)
 
 ```
 
+It also offers a interactive shell `moneywiz-cli`.
+
 ## Contribution
 
 This project is in very early stage, all contributions are welcomed!
```

#### html2text {}

```diff
@@ -4,9 +4,10 @@
 Started ```bash pip install moneywiz-api ``` ```python from moneywiz_api import
 MoneywizApi moneywizApi = MoneywizApi("") ( accessor, account_manager,
 payee_manager, category_manager, transaction_manager,
 investment_holding_manager, ) = ( moneywizApi.accessor,
 moneywizApi.account_manager, moneywizApi.payee_manager,
 moneywizApi.category_manager, moneywizApi.transaction_manager,
 moneywizApi.investment_holding_manager, ) record = accessor.get_record
-(record_id) print(record) ``` ## Contribution This project is in very early
-stage, all contributions are welcomed!
+(record_id) print(record) ``` It also offers a interactive shell `moneywiz-
+cli`. ## Contribution This project is in very early stage, all contributions
+are welcomed!
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/database_accessor.py` & `moneywiz_api-1.0.0/src/moneywiz_api/database_accessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import sqlite3
 from collections import defaultdict
 from pathlib import Path
 from typing import Dict, List, Any, Callable, Tuple
+from decimal import Decimal
 
 from moneywiz_api.model.record import Record
-from moneywiz_api.types import ENT_ID, ID
+from moneywiz_api.model.raw_data_handler import RawDataHandler as RDH
+from moneywiz_api.types import ENT_ID, ID, GID
 
 
 class DatabaseAccessor:
     def __init__(self, db_path: Path):
         self._con = sqlite3.connect(db_path, uri=True)
 
         def dict_factory(cursor, row):
@@ -66,26 +68,38 @@
         
         """,
             [pk_id],
         )
 
         return constructor(res.fetchone())
 
-    def get_category_assignment(self) -> Dict[ID, List[Tuple[ID, float]]]:
-        transaction_map: Dict[ID, List[Tuple[ID, float]]] = defaultdict(list)
+    def get_record_by_gid(self, gid: GID, constructor: Callable = Record):
+        cur = self._con.cursor()
+        res = cur.execute(
+            """
+        SELECT * FROM ZSYNCOBJECT WHERE ZGID = ?
+        
+        """,
+            [gid],
+        )
+
+        return constructor(res.fetchone())
+
+    def get_category_assignment(self) -> Dict[ID, List[Tuple[ID, Decimal]]]:
+        transaction_map: Dict[ID, List[Tuple[ID, Decimal]]] = defaultdict(list)
         cur = self._con.cursor()
         res = cur.execute(
             """
         SELECT ZCATEGORY, ZTRANSACTION, ZAMOUNT  FROM ZCATEGORYASSIGMENT WHERE ZTRANSACTION IS NOT NULL
         
         """
         )
         for row in res.fetchall():
             transaction_map[row["ZTRANSACTION"]].append(
-                (row["ZCATEGORY"], row["ZAMOUNT"])
+                (row["ZCATEGORY"], RDH.get_decimal(row, "ZAMOUNT"))
             )
         return transaction_map
 
     def get_refund_maps(self) -> Dict[ID, ID]:
         refund_to_withdraw: Dict[ID, ID] = {}
         cur = self._con.cursor()
         res = cur.execute(
@@ -106,7 +120,20 @@
         SELECT Z_36TRANSACTIONS, Z_35TAGS FROM  Z_36TAGS
         
         """
         )
         for row in res.fetchall():
             transactions_to_tags[row["Z_36TRANSACTIONS"]].append(row["Z_35TAGS"])
         return transactions_to_tags
+
+    def get_users(self) -> Dict[ID, str]:
+        users_map: Dict[ID, str] = {}
+        cur = self._con.cursor()
+        res = cur.execute(
+            """
+        SELECT Z_PK, ZSYNCLOGIN FROM  "ZUSER"
+        
+        """
+        )
+        for row in res.fetchall():
+            users_map[row["Z_PK"]] = row["ZSYNCLOGIN"]
+        return users_map
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/managers/account_manager.py` & `moneywiz_api-1.0.0/src/moneywiz_api/managers/account_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,16 +28,14 @@
             "CreditCardAccount": CreditCardAccount,
             "LoanAccount": LoanAccount,
             "InvestmentAccount": InvestmentAccount,
             "ForexAccount": ForexAccount,
         }
 
     def records(self) -> Dict[ID, Account]:
-        return dict(
-            sorted(super().records().items(), key=lambda x: x[1]._display_order)
-        )
+        return dict(sorted(super().records().items(), key=lambda x: x[1].display_order))
 
     def get_accounts_for_user(self, user_id: ID) -> List[Account]:
         return sorted(
             [x for _, x in self.records().items() if x.user == user_id],
-            key=lambda x: (x._group_id, x._display_order),
+            key=lambda x: (x.group_id, x.display_order),
         )
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/managers/category_manager.py` & `moneywiz_api-1.0.0/src/moneywiz_api/managers/category_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         }
 
     def get_name_chain(self, category_id: ID) -> List[str]:
         ret: List[str] = []
         current = self.get(category_id)
         while current:
             ret.insert(0, current.name)
-            if not current.parentId:
+            if not current.parent_id:
                 break
             else:
-                current = self.get(current.parentId)
+                current = self.get(current.parent_id)
         return ret
 
     def get_name_chain_by_gid(self, category_gid: GID) -> List[str]:
         current = self.get_by_gid(category_gid)
         return self.get_name_chain(current.id)
 
     def get_categories_for_user(self, user_id: ID) -> List[Category]:
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/managers/investment_holding_manager.py` & `moneywiz_api-1.0.0/src/moneywiz_api/managers/investment_holding_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Dict, Callable, List
+from decimal import Decimal
 
 from moneywiz_api.model.investment_holding import InvestmentHolding
 from moneywiz_api.managers.record_manager import RecordManager
 from moneywiz_api.types import ID
 
 
 class InvestmentHoldingManager(RecordManager[InvestmentHolding]):
@@ -14,12 +15,12 @@
         return {
             "InvestmentHolding": InvestmentHolding,
         }
 
     def get_holdings_for_account(self, account_id: ID) -> List[InvestmentHolding]:
         return [x for _, x in self.records().items() if x.account == account_id]
 
-    def update_last_price(self, latest_price: float):
+    def update_last_price(self, latest_price: Decimal):
         raise NotImplementedError()
 
-    def update_price_table(self, latest_price: float):
+    def update_price_table(self, latest_price: Decimal):
         raise NotImplementedError()
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/managers/record_manager.py` & `moneywiz_api-1.0.0/src/moneywiz_api/managers/record_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             if typename in self.ents:
                 obj = self.ents[typename](record)
                 self.add(obj)
 
     def add(self, record: T) -> None:
         self._records[record.id] = record
         if record.gid in self._gid_to_id:
-            raise Exception(
+            raise RuntimeError(
                 f"Duplicate gid for {record}, existing record Id {self._gid_to_id[record.gid]}"
             )
 
         self._gid_to_id[record.gid] = record.id
 
     def get(self, record_id: ID) -> T | None:
         return self._records.get(record_id)
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/managers/transaction_manager.py` & `moneywiz_api-1.0.0/src/moneywiz_api/managers/transaction_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 from typing import Dict, Callable, List, Tuple
+from decimal import Decimal
 
-from moneywiz_api import utils
 from moneywiz_api.database_accessor import DatabaseAccessor
 from moneywiz_api.model.transaction import (
     Transaction,
     DepositTransaction,
     InvestmentExchangeTransaction,
     InvestmentBuyTransaction,
     InvestmentSellTransaction,
@@ -19,15 +19,15 @@
 from moneywiz_api.managers.record_manager import RecordManager
 from moneywiz_api.types import ID
 
 
 class TransactionManager(RecordManager[Transaction]):
     def __init__(self):
         super().__init__()
-        self.category_assignment: Dict[ID, List[Tuple[ID, float]]] = {}
+        self.category_assignment: Dict[ID, List[Tuple[ID, Decimal]]] = {}
         self.refund_maps: Dict[ID, ID] = {}
         self.tags_map: Dict[ID, ID] = {}
 
     @property
     def ents(self) -> Dict[str, Callable]:
         return {
             "DepositTransaction": DepositTransaction,
@@ -40,23 +40,23 @@
             "TransferDepositTransaction": TransferDepositTransaction,
             "TransferWithdrawTransaction": TransferWithdrawTransaction,
             "WithdrawTransaction": WithdrawTransaction,
         }
 
     def load(self, db_accessor: DatabaseAccessor) -> None:
         super().load(db_accessor)
-        self.category_assignment: Dict[ID, List[Tuple[ID, float]]] = (
+        self.category_assignment: Dict[ID, List[Tuple[ID, Decimal]]] = (
             db_accessor.get_category_assignment()
         )
         self.refund_maps: Dict[ID, ID] = db_accessor.get_refund_maps()
         self.tags_map: Dict[ID, ID] = db_accessor.get_tags_map()
 
     def category_for_transaction(
         self, transaction_id: ID
-    ) -> List[Tuple[ID, float]] | None:
+    ) -> List[Tuple[ID, Decimal]] | None:
         return self.category_assignment.get(transaction_id)
 
     def tags_for_transaction(self, transaction_id: ID) -> List[ID] | None:
         return self.tags_map.get(transaction_id)
 
     def original_transaction_for_refund_transaction(
         self, transaction_id: ID
@@ -74,22 +74,21 @@
         """
         return sorted(
             [
                 x
                 for _, x in self.records().items()
                 if not isinstance(x, TransferBudgetTransaction)
                 and x.account == account_id
-                and x.date <= utils.get_date(until)
+                and x.datetime <= until
             ],
-            key=lambda x: x.date,
+            key=lambda x: x.datetime,
         )
 
     def get_all(self, until: datetime = datetime.now()) -> List[Transaction]:
         return sorted(
             [
                 x
                 for _, x in self.records().items()
-                if not isinstance(x, TransferBudgetTransaction)
-                and x.date <= utils.get_date(until)
+                if not isinstance(x, TransferBudgetTransaction) and x.datetime <= until
             ],
-            key=lambda x: x.date,
+            key=lambda x: x.datetime,
         )
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/model/__init__.py` & `moneywiz_api-1.0.0/src/moneywiz_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/model/account.py` & `moneywiz_api-1.0.0/src/moneywiz_api/model/account.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 from abc import ABC
 from dataclasses import dataclass, field
+from decimal import Decimal
 
-from moneywiz_api.model.record import Record
 from moneywiz_api.types import ID
+from moneywiz_api.model.raw_data_handler import RawDataHandler as RDH
+from moneywiz_api.model.record import Record
 
 
 @dataclass
 class Account(Record, ABC):
     """
     ENT: 9
     """
 
-    _display_order: int = field(repr=False)
-    _group_id: int = field(repr=False)
+    display_order: int = field(repr=False)
+    group_id: int = field(repr=False)
 
     name: str
     currency: str
-    opening_balance: float
+    opening_balance: Decimal  # might be a tiny number
     info: str
     user: ID
 
     def __init__(self, row):
         super().__init__(row)
-        self._display_order = row["ZDISPLAYORDER"]
-        self._group_id = row["ZGROUPID"]
+        self.display_order = row["ZDISPLAYORDER"]
+        self.group_id = row["ZGROUPID"]
 
         self.name = row["ZNAME"]
         self.currency = row["ZCURRENCYNAME"]
-        self.opening_balance = row["ZOPENINGBALANCE"]
+        self.opening_balance = RDH.get_decimal(row, "ZOPENINGBALANCE")
         self.info = row["ZINFO"]
 
         self.user = row["ZUSER"]
 
+        # Fixes
+
         # Validate
-        assert self.name is not None
-        assert self.currency is not None
-        assert self.opening_balance is not None
-        assert self.info is not None
-        assert self.user is not None
+        assert self.display_order is not None, self.as_dict()
+        assert self.group_id is not None, self.as_dict()
+        assert self.name is not None, self.as_dict()
+        assert self.currency is not None, self.as_dict()
+        assert self.opening_balance is not None, self.as_dict()
+        assert self.info is not None, self.as_dict()
+        assert self.user is not None, self.as_dict()
 
 
 @dataclass
 class BankChequeAccount(Account):
     """
     ENT: 10
     """
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/model/category.py` & `moneywiz_api-1.0.0/src/moneywiz_api/model/category.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 @dataclass
 class Category(Record):
     """
     ENT: 19
     """
 
     name: str
-    parentId: Optional[int]
+    parent_id: Optional[int]
     type: CategoryType
     user: ID
 
     def __init__(self, row):
         super().__init__(row)
         self.name = row["ZNAME2"]
-        self.parentId = row["ZPARENTCATEGORY"]
+        self.parent_id = row["ZPARENTCATEGORY"]
         self.type = self._convert_type(row["ZTYPE2"])
         self.user = row["ZUSER3"]
 
+        # Fixes
+
         # Validate
-        assert self.name is not None
-        assert self.type is not None
-        assert self.user is not None
+        assert self.name is not None, self.as_dict()
+        assert self.type is not None, self.as_dict()
+        assert self.user is not None, self.as_dict()
 
     @staticmethod
     def _convert_type(type_: Optional[int]) -> CategoryType:
-        if not type_:
-            raise Exception("Invalid type")
-        if type_ not in [1, 2]:
-            raise Exception("Invalid type")
-        return "Expenses" if type_ == 1 else "Income"
+        if type_ and type_ in [1, 2]:
+            return "Expenses" if type_ == 1 else "Income"
+        raise RuntimeError(f"Invalid type {type_}")
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/model/investment_holding.py` & `moneywiz_api-1.0.0/src/moneywiz_api/model/investment_holding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from dataclasses import dataclass, field
 from typing import Dict, Any, Optional
+from decimal import Decimal
 
+from moneywiz_api.model.raw_data_handler import RawDataHandler as RDH
 from moneywiz_api.model.record import Record
 from moneywiz_api.types import ID
 
 
 @dataclass
 class InvestmentHolding(Record):
     """
     ENT: 24
     """
 
     account: ID
-    opening_number_of_shares: Optional[float]
+    opening_number_of_shares: Optional[Decimal]
 
-    number_of_shares: float
-    # price_per_share: float
+    number_of_shares: Decimal
+    # price_per_share: Decimal
     symbol: str
     holding_type: Optional[str]
     description: str
 
     price_per_share_available_online: bool
 
     """
@@ -33,43 +35,49 @@
     _investment_object_type: int = field(repr=False)
 
     """
     Unsure
     
     seems like the the cost for the shares which is not from transactions
     """
-    _cost_basis_of_missing_ob_shares: float = field(repr=False)
+    _cost_basis_of_missing_ob_shares: Decimal = field(repr=False)
 
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZINVESTMENTACCOUNT"]
-        self.opening_number_of_shares = row["ZOPENNINGNUMBEROFSHARES"]
-        self.number_of_shares = row["ZNUMBEROFSHARES"]
+        self.opening_number_of_shares = RDH.get_nullable_decimal(
+            row, "ZOPENNINGNUMBEROFSHARES"
+        )
+        self.number_of_shares = RDH.get_decimal(row, "ZNUMBEROFSHARES")
         # self.price_per_share = row["ZPRICEPERSHARE"]
         self.symbol = row["ZSYMBOL"]
         self.holding_type = row["ZHOLDINGTYPE"]
         self.description = row["ZDESC"]
         self.price_per_share_available_online = (
             row["ZISPRICEPERSHAREAVAILABLEONLINE"] == 1
         )
 
         self._investment_object_type = row["ZINVESTMENTOBJECTTYPE"]
-        self._cost_basis_of_missing_ob_shares = row["ZISFROMONLINEBANKING"]
+        self._cost_basis_of_missing_ob_shares = RDH.get_decimal(
+            row, "ZCOSTBASISOFMISSINGOBSHARES"
+        )
+
+        # Fixes
 
         # Validate
         self.validate()
 
     def validate(self):
-        assert self.account is not None
-        assert self.number_of_shares is not None
+        assert self.account is not None, self.as_dict()
+        assert self.number_of_shares is not None, self.as_dict()
         # assert self.price_per_share is not None
-        assert self.symbol is not None
-        assert self.description is not None
+        assert self.symbol is not None, self.as_dict()
+        assert self.description is not None, self.as_dict()
 
-        assert self._investment_object_type is not None
-        assert self._cost_basis_of_missing_ob_shares is not None
+        assert self._investment_object_type is not None, self.as_dict()
+        assert self._cost_basis_of_missing_ob_shares is not None, self.as_dict()
 
     def as_dict(self) -> Dict[str, Any]:
         original = super().as_dict()
         del original["_investment_object_type"]
         del original["_cost_basis_of_missing_ob_shares"]
         return original
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/model/transaction.py` & `moneywiz_api-1.0.0/src/moneywiz_api/model/transaction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,93 @@
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
+from datetime import datetime
+from decimal import Decimal
 
+from moneywiz_api.model.raw_data_handler import RawDataHandler as RDH
 from moneywiz_api.model.record import Record
 from moneywiz_api.types import ID
 
+
 import pytest
 
 
 @dataclass
 class Transaction(Record, ABC):
     """
     ENT: 36
     """
 
     reconciled: bool
 
-    amount: float
+    amount: Decimal
     description: str
-    date: float
+    datetime: datetime
     notes: Optional[str]
 
     def __init__(self, row):
         super().__init__(row)
         self.reconciled = row["ZRECONCILED"] == 1
-        self.amount = row["ZAMOUNT1"]
+        self.amount = RDH.get_decimal(row, "ZAMOUNT1")
         self.description = row["ZDESC2"]
-        self.date = row["ZDATE1"]
+        self.datetime = RDH.get_datetime(row, "ZDATE1")
         self.notes = row["ZNOTES1"]
 
+        # Fixes
+
         # Validate
-        assert self.reconciled is not None
-        assert self.amount is not None
-        assert self.description is not None
-        assert self.date is not None
+        assert self.reconciled is not None, self.as_dict()
+        assert self.amount is not None, self.as_dict()
+        assert self.description is not None, self.as_dict()
+        assert self.datetime is not None, self.as_dict()
         # self.notes can be None
 
 
 @dataclass
 class DepositTransaction(Transaction):
     """
     ENT: 37
     """
 
     account: ID
-    amount: float  # neg: expense, pos: income
+    amount: Decimal  # neg: expense, pos: income
     payee: Optional[ID]
 
     # FX
     original_currency: str
-    original_amount: float  # neg: expense, pos: income
-    original_exchange_rate: Optional[float]
+    original_amount: Decimal  # neg: expense, pos: income
+    original_exchange_rate: Optional[Decimal]
 
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZACCOUNT2"]
-        self.amount = row["ZAMOUNT1"]
+        self.amount = RDH.get_decimal(row, "ZAMOUNT1")
         self.payee = row["ZPAYEE2"]
         self.original_currency = row["ZORIGINALCURRENCY"]
-        self.original_amount = row["ZORIGINALAMOUNT"]
-        self.original_exchange_rate = row["ZORIGINALEXCHANGERATE"]
+        self.original_amount = RDH.get_decimal(row, "ZORIGINALAMOUNT")
+        self.original_exchange_rate = RDH.get_nullable_decimal(
+            row, "ZORIGINALEXCHANGERATE"
+        )
 
         # Validate
         self.validate()
 
     def validate(self):
-        assert self.account is not None
-        assert self.amount is not None
+        assert self.account is not None, self.as_dict()
+        assert self.amount is not None, self.as_dict()
         # self.payee can be None
-        assert self.original_currency is not None
-        assert self.original_amount is not None
+        assert self.original_currency is not None, self.as_dict()
+        assert self.original_amount is not None, self.as_dict()
 
-        assert self.amount * self.original_amount > 0  # Same sign
+        assert self.amount * self.original_amount > 0, self.as_dict()  # Same sign
         if self.original_exchange_rate is not None:
-            assert self.amount == self.original_amount * self.original_exchange_rate
+            assert (
+                self.amount == self.original_amount * self.original_exchange_rate
+            ), self.as_dict()
 
 
 @dataclass
 class InvestmentExchangeTransaction(Transaction):
     """
     ENT: 38
     """
@@ -100,32 +110,32 @@
 @dataclass
 class InvestmentBuyTransaction(InvestmentTransaction):
     """
     ENT: 40
     """
 
     account: ID
-    amount: float
+    amount: Decimal
 
-    fee: float
+    fee: Decimal
 
     investment_holding: ID
-    number_of_shares: float
-    price_per_share: float
+    number_of_shares: Decimal
+    price_per_share: Decimal
 
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZACCOUNT2"]
-        self.amount = row["ZAMOUNT1"]
+        self.amount = RDH.get_decimal(row, "ZAMOUNT1")
 
-        self.fee = row["ZFEE2"]
+        self.fee = RDH.get_decimal(row, "ZFEE2")
 
         self.investment_holding = row["ZINVESTMENTHOLDING"]
-        self.number_of_shares = row["ZNUMBEROFSHARES1"]
-        self.price_per_share = row["ZPRICEPERSHARE1"]
+        self.number_of_shares = RDH.get_decimal(row, "ZNUMBEROFSHARES1")
+        self.price_per_share = RDH.get_decimal(row, "ZPRICEPERSHARE1")
 
         # Fixes
         self.fee = max(self.fee, 0)
 
         # Validate
         self.validate()
 
@@ -150,32 +160,32 @@
 @dataclass
 class InvestmentSellTransaction(InvestmentTransaction):
     """
     ENT: 41
     """
 
     account: ID
-    amount: float  # neg: loss after fees, pos: income
+    amount: Decimal  # neg: loss after fees, pos: income
 
-    fee: float
+    fee: Decimal
 
     investment_holding: ID
-    number_of_shares: float
-    price_per_share: float
+    number_of_shares: Decimal
+    price_per_share: Decimal
 
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZACCOUNT2"]
-        self.amount = row["ZAMOUNT1"]
+        self.amount = RDH.get_decimal(row, "ZAMOUNT1")
 
-        self.fee = row["ZFEE2"]
+        self.fee = RDH.get_decimal(row, "ZFEE2")
 
         self.investment_holding = row["ZINVESTMENTHOLDING"]
-        self.number_of_shares = row["ZNUMBEROFSHARES1"]
-        self.price_per_share = row["ZPRICEPERSHARE1"]
+        self.number_of_shares = RDH.get_decimal(row, "ZNUMBEROFSHARES1")
+        self.price_per_share = RDH.get_decimal(row, "ZPRICEPERSHARE1")
 
         # Fixes
         self.fee = max(self.fee, 0)
 
         # Validate
         self.validate()
 
@@ -201,22 +211,22 @@
 @dataclass
 class ReconcileTransaction(Transaction):
     """
     ENT: 42
     """
 
     account: ID
-    amount: float  # neg: expense, pos: income
-    reconcile_amount: float  # new balance
+    amount: Decimal  # neg: expense, pos: income
+    reconcile_amount: Decimal  # new balance
 
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZACCOUNT2"]
-        self.amount = row["ZAMOUNT1"]
-        self.reconcile_amount = row["ZRECONCILEAMOUNT"]
+        self.amount = RDH.get_decimal(row, "ZAMOUNT1")
+        self.reconcile_amount = RDH.get_decimal(row, "ZRECONCILEAMOUNT")
 
         # Validate
         self.validate()
 
     def validate(self):
         assert self.account is not None
         assert self.amount is not None
@@ -226,31 +236,33 @@
 @dataclass
 class RefundTransaction(Transaction):
     """
     ENT: 43
     """
 
     account: ID
-    amount: float
+    amount: Decimal
     payee: Optional[ID]
 
     # FX
     original_currency: str
-    original_amount: float
-    original_exchange_rate: Optional[float]
+    original_amount: Decimal
+    original_exchange_rate: Optional[Decimal]
 
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZACCOUNT2"]
-        self.amount = row["ZAMOUNT1"]
+        self.amount = RDH.get_decimal(row, "ZAMOUNT1")
         self.payee = row["ZPAYEE2"]
 
         self.original_currency = row["ZORIGINALCURRENCY"]
-        self.original_amount = row["ZORIGINALAMOUNT"]
-        self.original_exchange_rate = row["ZORIGINALEXCHANGERATE"]
+        self.original_amount = RDH.get_decimal(row, "ZORIGINALAMOUNT")
+        self.original_exchange_rate = RDH.get_nullable_decimal(
+            row, "ZORIGINALEXCHANGERATE"
+        )
 
         # Validate
         self.validate()
 
     def validate(self):
         assert self.account is not None
         assert self.amount is not None
@@ -280,47 +292,47 @@
 @dataclass
 class TransferDepositTransaction(Transaction):
     """
     ENT: 45
     """
 
     account: ID
-    amount: float  # pos: in
+    amount: Decimal  # pos: in
 
     sender_account: ID
     sender_transaction: ID
 
-    original_amount: float  # ATTENTION: sign got fixed
+    original_amount: Decimal  # ATTENTION: sign got fixed
     original_currency: str
 
-    sender_amount: float
+    sender_amount: Decimal
     sender_currency: str
 
-    original_fee: Optional[float]
+    original_fee: Optional[Decimal]
     original_fee_currency: Optional[str]
 
-    original_exchange_rate: float
+    original_exchange_rate: Decimal
 
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZACCOUNT2"]
-        self.amount = row["ZAMOUNT1"]
+        self.amount = RDH.get_decimal(row, "ZAMOUNT1")
 
         self.sender_account = row["ZSENDERACCOUNT"]
         self.sender_transaction = row["ZSENDERTRANSACTION"]
 
-        self.original_amount = row["ZORIGINALAMOUNT"]
+        self.original_amount = RDH.get_decimal(row, "ZORIGINALAMOUNT")
         self.original_currency = row["ZORIGINALCURRENCY"]
-        self.sender_amount = row["ZORIGINALSENDERAMOUNT"]
+        self.sender_amount = RDH.get_decimal(row, "ZORIGINALSENDERAMOUNT")
         self.sender_currency = row["ZORIGINALSENDERCURRENCY"]
 
-        self.original_fee = row["ZORIGINALFEE"]
+        self.original_fee = RDH.get_nullable_decimal(row, "ZORIGINALFEE")
         self.original_fee_currency = row["ZORIGINALFEECURRENCY"]
 
-        self.original_exchange_rate = row["ZORIGINALEXCHANGERATE"]
+        self.original_exchange_rate = RDH.get_decimal(row, "ZORIGINALEXCHANGERATE")
 
         # Fixes
         self.original_amount = abs(self.original_amount)
 
         # Validate
         self.validate()
 
@@ -353,47 +365,47 @@
 @dataclass
 class TransferWithdrawTransaction(Transaction):
     """
     ENT: 46
     """
 
     account: ID
-    amount: float  # neg: out
+    amount: Decimal  # neg: out
 
     recipient_account: ID
     recipient_transaction: ID
 
-    original_amount: float  # always neg
+    original_amount: Decimal  # always neg
     original_currency: str
 
-    recipient_amount: float  # ATTENTION: sign got fixed
+    recipient_amount: Decimal  # ATTENTION: sign got fixed
     recipient_currency: str
 
-    original_fee: Optional[float]
+    original_fee: Optional[Decimal]
     original_fee_currency: Optional[str]
 
-    original_exchange_rate: float
+    original_exchange_rate: Decimal
 
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZACCOUNT2"]
-        self.amount = row["ZAMOUNT1"]
+        self.amount = RDH.get_decimal(row, "ZAMOUNT1")
 
         self.recipient_account = row["ZRECIPIENTACCOUNT1"]
         self.recipient_transaction = row["ZRECIPIENTTRANSACTION"]
 
-        self.original_amount = row["ZORIGINALAMOUNT"]
+        self.original_amount = RDH.get_decimal(row, "ZORIGINALAMOUNT")
         self.original_currency = row["ZORIGINALCURRENCY"]
-        self.recipient_amount = row["ZORIGINALRECIPIENTAMOUNT"]
+        self.recipient_amount = RDH.get_decimal(row, "ZORIGINALRECIPIENTAMOUNT")
         self.recipient_currency = row["ZORIGINALRECIPIENTCURRENCY"]
 
-        self.original_fee = row["ZORIGINALFEE"]
+        self.original_fee = RDH.get_nullable_decimal(row, "ZORIGINALFEE")
         self.original_fee_currency = row["ZORIGINALFEECURRENCY"]
 
-        self.original_exchange_rate = row["ZORIGINALEXCHANGERATE"]
+        self.original_exchange_rate = RDH.get_decimal(row, "ZORIGINALEXCHANGERATE")
 
         # Fixes
         self.recipient_amount = abs(self.recipient_amount)
 
         # Validate
         self.validate()
 
@@ -425,31 +437,33 @@
 @dataclass
 class WithdrawTransaction(Transaction):
     """
     ENT: 47
     """
 
     account: ID
-    amount: float  # neg: expense, pos: income
+    amount: Decimal  # neg: expense, pos: income
     payee: Optional[ID]
 
     # FX
     original_currency: str
-    original_amount: float  # neg: expense, pos: income ATTENTION: sign got fixed
-    original_exchange_rate: Optional[float]
+    original_amount: Decimal  # neg: expense, pos: income ATTENTION: sign got fixed
+    original_exchange_rate: Optional[Decimal]
 
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZACCOUNT2"]
-        self.amount = row["ZAMOUNT1"]
+        self.amount = RDH.get_decimal(row, "ZAMOUNT1")
         self.payee = row["ZPAYEE2"]
 
         self.original_currency = row["ZORIGINALCURRENCY"]
-        self.original_amount = row["ZORIGINALAMOUNT"]
-        self.original_exchange_rate = row["ZORIGINALEXCHANGERATE"]
+        self.original_amount = RDH.get_decimal(row, "ZORIGINALAMOUNT")
+        self.original_exchange_rate = RDH.get_nullable_decimal(
+            row, "ZORIGINALEXCHANGERATE"
+        )
 
         # Fixes
         if self.amount * self.original_amount < 0:
             self.original_amount = -self.original_amount
 
         # Validate
         self.validate()
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api/moneywiz_api.py` & `moneywiz_api-1.0.0/src/moneywiz_api/moneywiz_api.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api.egg-info/PKG-INFO` & `moneywiz_api-1.0.0/src/moneywiz_api.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 0.2.1
+Version: 1.0.0
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # MoneyWiz-API
 
 ![Static Badge](https://img.shields.io/badge/Python-3-blue?style=flat&logo=Python)
 ![PyPI](https://img.shields.io/pypi/v/moneywiz-api)
 
-
 <a href="https://www.buymeacoffee.com/Ileodo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
 
 A Python API to access MoneyWiz Sqlite database.
 
-
 ## Get Started
 
 ```bash
 pip install moneywiz-api
 ```
 
 ```python
@@ -52,10 +58,12 @@
 )
 
 record = accessor.get_record(record_id)
 print(record)
 
 ```
 
+It also offers a interactive shell `moneywiz-cli`.
+
 ## Contribution
 
 This project is in very early stage, all contributions are welcomed!
```

#### html2text {}

```diff
@@ -1,19 +1,23 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 0.2.1 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.0 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE # MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
-blue?style=flat&logo=Python) ![PyPI](https://img.shields.io/pypi/v/moneywiz-
-api) _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]A Python API to access MoneyWiz Sqlite database. ## Get
-Started ```bash pip install moneywiz-api ``` ```python from moneywiz_api import
-MoneywizApi moneywizApi = MoneywizApi("") ( accessor, account_manager,
-payee_manager, category_manager, transaction_manager,
-investment_holding_manager, ) = ( moneywizApi.accessor,
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: pandas Provides-Extra: dev Requires-Dist: pytest; extra
+== "dev" Requires-Dist: pylint; extra == "dev" Requires-Dist: mypy; extra ==
+"dev" Requires-Dist: black; extra == "dev" Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev" # MoneyWiz-API ![Static Badge](https://
+img.shields.io/badge/Python-3-blue?style=flat&logo=Python) ![PyPI](https://
+img.shields.io/pypi/v/moneywiz-api) _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]A Python API to access
+MoneyWiz Sqlite database. ## Get Started ```bash pip install moneywiz-api ```
+```python from moneywiz_api import MoneywizApi moneywizApi = MoneywizApi("")
+( accessor, account_manager, payee_manager, category_manager,
+transaction_manager, investment_holding_manager, ) = ( moneywizApi.accessor,
 moneywizApi.account_manager, moneywizApi.payee_manager,
 moneywizApi.category_manager, moneywizApi.transaction_manager,
 moneywizApi.investment_holding_manager, ) record = accessor.get_record
-(record_id) print(record) ``` ## Contribution This project is in very early
-stage, all contributions are welcomed!
+(record_id) print(record) ``` It also offers a interactive shell `moneywiz-
+cli`. ## Contribution This project is in very early stage, all contributions
+are welcomed!
```

### Comparing `moneywiz_api-0.2.1/src/moneywiz_api.egg-info/SOURCES.txt` & `moneywiz_api-1.0.0/src/moneywiz_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 LICENSE
 README.md
 pyproject.toml
+requirements-dev.txt
+requirements.txt
 src/__init__.py
-src/shell.py
 src/moneywiz_api/__init__.py
 src/moneywiz_api/database_accessor.py
 src/moneywiz_api/moneywiz_api.py
 src/moneywiz_api/types.py
 src/moneywiz_api/utils.py
 src/moneywiz_api.egg-info/PKG-INFO
 src/moneywiz_api.egg-info/SOURCES.txt
 src/moneywiz_api.egg-info/dependency_links.txt
+src/moneywiz_api.egg-info/entry_points.txt
+src/moneywiz_api.egg-info/requires.txt
 src/moneywiz_api.egg-info/top_level.txt
+src/moneywiz_api/cli/cli.py
+src/moneywiz_api/cli/helpers.py
 src/moneywiz_api/managers/__init__.py
 src/moneywiz_api/managers/account_manager.py
 src/moneywiz_api/managers/category_manager.py
 src/moneywiz_api/managers/investment_holding_manager.py
 src/moneywiz_api/managers/payee_manager.py
 src/moneywiz_api/managers/record_manager.py
 src/moneywiz_api/managers/tag_manager.py
 src/moneywiz_api/managers/transaction_manager.py
 src/moneywiz_api/model/__init__.py
 src/moneywiz_api/model/account.py
 src/moneywiz_api/model/category.py
 src/moneywiz_api/model/investment_holding.py
 src/moneywiz_api/model/payee.py
+src/moneywiz_api/model/raw_data_handler.py
 src/moneywiz_api/model/record.py
 src/moneywiz_api/model/tag.py
 src/moneywiz_api/model/transaction.py
 tests/test_config.py
```


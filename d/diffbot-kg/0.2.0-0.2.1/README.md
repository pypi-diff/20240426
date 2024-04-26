# Comparing `tmp/diffbot_kg-0.2.0.tar.gz` & `tmp/diffbot_kg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffbot_kg-0.2.0.tar", max compression
+gzip compressed data, was "diffbot_kg-0.2.1.tar", max compression
```

## Comparing `diffbot_kg-0.2.0.tar` & `diffbot_kg-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1074 2024-04-10 21:01:10.627504 diffbot_kg-0.2.0/LICENSE
--rw-r--r--   0        0        0     1311 2024-04-10 21:01:10.627504 diffbot_kg-0.2.0/README.md
--rw-r--r--   0        0        0      648 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/__init__.py
--rw-r--r--   0        0        0     3819 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/clients/base.py
--rw-r--r--   0        0        0     5850 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/clients/enhance.py
--rw-r--r--   0        0        0     2050 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/clients/search.py
--rw-r--r--   0        0        0     3224 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/clients/session.py
--rw-r--r--   0        0        0      644 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/__init__.py
--rw-r--r--   0        0        0     1767 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/base.py
--rw-r--r--   0        0        0      573 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_create.py
--rw-r--r--   0        0        0      471 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_list.py
--rw-r--r--   0        0        0     1011 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_results.py
--rw-r--r--   0        0        0      786 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_status.py
--rw-r--r--   0        0        0      141 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/coverage_report.py
--rw-r--r--   0        0        0      865 2024-04-10 21:01:10.631504 diffbot_kg-0.2.0/src/diffbot_kg/models/response/entities.py
--rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 diffbot_kg-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1272 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/README.md
+-rw-r--r--   0        0        0      648 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/clients/__init__.py
+-rw-r--r--   0        0        0     3930 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/clients/base.py
+-rw-r--r--   0        0        0     5851 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/clients/enhance.py
+-rw-r--r--   0        0        0     2050 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/clients/search.py
+-rw-r--r--   0        0        0     3636 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/clients/session.py
+-rw-r--r--   0        0        0      644 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/models/response/__init__.py
+-rw-r--r--   0        0        0     1767 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/models/response/base.py
+-rw-r--r--   0        0        0      573 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/models/response/bulkjob_create.py
+-rw-r--r--   0        0        0      471 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/models/response/bulkjob_list.py
+-rw-r--r--   0        0        0     1011 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/models/response/bulkjob_results.py
+-rw-r--r--   0        0        0      786 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/models/response/bulkjob_status.py
+-rw-r--r--   0        0        0      141 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/models/response/coverage_report.py
+-rw-r--r--   0        0        0      865 2024-04-26 05:15:07.256533 diffbot_kg-0.2.1/src/diffbot_kg/models/response/entities.py
+-rw-r--r--   0        0        0     1857 1970-01-01 00:00:00.000000 diffbot_kg-0.2.1/PKG-INFO
```

### Comparing `diffbot_kg-0.2.0/LICENSE` & `diffbot_kg-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diffbot_kg-0.2.0/README.md` & `diffbot_kg-0.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,41 @@
-Diffbot Knowledge Graph Client
-=============
-
-![](https://www.diffbot.com/assets/img/diffbot-logo-darkbg.svg)
+# Diffbot Knowledge Graph Client
 
+![Diffbot Logo](https://www.diffbot.com/assets/img/diffbot-logo-darkbg.svg)
 
 [![CodeFactor](https://www.codefactor.io/repository/github/brendancsmith/diffbot-kg/badge)](https://www.codefactor.io/repository/github/brendancsmith/diffbot-kg)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/brendancsmith/diffbot-kg/python-package.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/diffbot-kg)
 ![GitHub License](https://img.shields.io/github/license/brendancsmith/diffbot-kg)
 
-
-Description
------------
+## Description
 
 Python client for the Diffbot Knowledge Graph API.
 
-Installation
-------------
+## Installation
 
 ```sh
 pip install diffbot-kg
 ```
 
-Usage
------
+## Usage
 
 ```python
 from diffbot_kg import DiffbotSearchClient, DiffbotEnhanceClient
 
 search_client = DiffbotSearchClient('your_api_key')
 enhance_client = DiffbotEnhanceClient('your_api_key')
 
 # Search for entities
 search_results = search_client.search({query='type:Organization name:Diffbot'})
 
 # Enhance an entity
 enhanced_entity = enhance_client.enhance({query='type:Organization name:Diffbot'})
 ```
 
-Contributing
-------------
+## Contributing
 
 Contributions to this project are welcome. - see the CONTRIBUTING.md file for details.
 
-License
--------
+## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `diffbot_kg-0.2.0/pyproject.toml` & `diffbot_kg-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "diffbot-kg"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python client for the Diffbot Knowledge Graph API."
 authors = ["Brendan C. Smith"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `diffbot_kg-0.2.0/src/diffbot_kg/clients/base.py` & `diffbot_kg-0.2.1/src/diffbot_kg/clients/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any
 
-from diffbot_kg.clients.session import BaseDiffbotResponse, DiffbotSession
 from yarl import URL
 
+from diffbot_kg.clients.session import BaseDiffbotResponse, DiffbotSession
+
 
 class BaseDiffbotKGClient:
     """
     Base class for Diffbot Knowledge Graph API clients.
     """
 
     url = URL("https://kg.diffbot.com/kg/v3/")
@@ -36,14 +37,16 @@
 
         Returns:
             dict: The merged parameters.
         """
 
         params = params or {}
         params = {**self.default_params, **params}
+
+        # sourcery skip: inline-immediately-returned-variable
         params = {k: v for k, v in params.items() if v is not None}
         return params
 
     async def _get(
         self, url: str | URL, params=None, headers=None
     ) -> BaseDiffbotResponse:
         """
@@ -54,17 +57,19 @@
             params (dict, optional): The query parameters for the request. Defaults to None.
             headers (dict, optional): The headers for the request. Defaults to None.
 
         Returns:
             BaseDiffbotResponse: The response from the API.
         """
 
-        headers = {"accept": "application/json", **(headers or {})}
+        headers = headers or {}
 
         params = self._merge_params(params)
+
+        # sourcery skip: inline-immediately-returned-variable
         resp = await self.s.get(url, params=params, headers=headers)
         return resp
 
     async def _post(
         self,
         url: str | URL,
         params: dict | None = None,
@@ -83,18 +88,18 @@
             BaseDiffbotResponse: The response from the API.
         """
 
         params = self._merge_params(params)
 
         headers = {
             "content-type": "application/json",
-            "accept": "application/json",
             **(headers or {}),
         }
 
+        # sourcery skip: inline-immediately-returned-variable
         resp = await self.s.post(url, params=params, headers=headers, json=json)
         return resp
 
     async def _get_or_post(
         self, url: str | URL, params: dict | None = None
     ) -> BaseDiffbotResponse:
         """
```

### Comparing `diffbot_kg-0.2.0/src/diffbot_kg/clients/enhance.py` & `diffbot_kg-0.2.1/src/diffbot_kg/clients/enhance.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,15 @@
         Returns:
             DiffbotResponse: The response from the Diffbot API.
         """
 
         url = self.bulk_job_coverage_report_url.human_repr().format(
             bulkjobId=bulkjobId, reportId=reportId
         )
+
         resp = await self._get(url)
         resp.__class__ = DiffbotCoverageReportResponse
         return cast(DiffbotCoverageReportResponse, resp)
 
     async def single_bulkjob_result(
         self,
         bulkjobId: str,
```

### Comparing `diffbot_kg-0.2.0/src/diffbot_kg/clients/search.py` & `diffbot_kg-0.2.1/src/diffbot_kg/clients/search.py`

 * *Files identical despite different names*

### Comparing `diffbot_kg-0.2.0/src/diffbot_kg/models/response/__init__.py` & `diffbot_kg-0.2.1/src/diffbot_kg/models/response/__init__.py`

 * *Files identical despite different names*

### Comparing `diffbot_kg-0.2.0/src/diffbot_kg/models/response/base.py` & `diffbot_kg-0.2.1/src/diffbot_kg/models/response/base.py`

 * *Files identical despite different names*

### Comparing `diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_create.py` & `diffbot_kg-0.2.1/src/diffbot_kg/models/response/bulkjob_create.py`

 * *Files identical despite different names*

### Comparing `diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_results.py` & `diffbot_kg-0.2.1/src/diffbot_kg/models/response/bulkjob_results.py`

 * *Files identical despite different names*

### Comparing `diffbot_kg-0.2.0/src/diffbot_kg/models/response/bulkjob_status.py` & `diffbot_kg-0.2.1/src/diffbot_kg/models/response/bulkjob_status.py`

 * *Files identical despite different names*

### Comparing `diffbot_kg-0.2.0/src/diffbot_kg/models/response/entities.py` & `diffbot_kg-0.2.1/src/diffbot_kg/models/response/entities.py`

 * *Files identical despite different names*

### Comparing `diffbot_kg-0.2.0/PKG-INFO` & `diffbot_kg-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,59 @@
 Metadata-Version: 2.1
 Name: diffbot-kg
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client for the Diffbot Knowledge Graph API.
 License: MIT
 Author: Brendan C. Smith
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: yarl (>=1.9.4,<2.0.0)
 Description-Content-Type: text/markdown
 
-Diffbot Knowledge Graph Client
-=============
-
-![](https://www.diffbot.com/assets/img/diffbot-logo-darkbg.svg)
+# Diffbot Knowledge Graph Client
 
+![Diffbot Logo](https://www.diffbot.com/assets/img/diffbot-logo-darkbg.svg)
 
 [![CodeFactor](https://www.codefactor.io/repository/github/brendancsmith/diffbot-kg/badge)](https://www.codefactor.io/repository/github/brendancsmith/diffbot-kg)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/brendancsmith/diffbot-kg/python-package.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/diffbot-kg)
 ![GitHub License](https://img.shields.io/github/license/brendancsmith/diffbot-kg)
 
-
-Description
------------
+## Description
 
 Python client for the Diffbot Knowledge Graph API.
 
-Installation
-------------
+## Installation
 
 ```sh
 pip install diffbot-kg
 ```
 
-Usage
------
+## Usage
 
 ```python
 from diffbot_kg import DiffbotSearchClient, DiffbotEnhanceClient
 
 search_client = DiffbotSearchClient('your_api_key')
 enhance_client = DiffbotEnhanceClient('your_api_key')
 
 # Search for entities
 search_results = search_client.search({query='type:Organization name:Diffbot'})
 
 # Enhance an entity
 enhanced_entity = enhance_client.enhance({query='type:Organization name:Diffbot'})
 ```
 
-Contributing
-------------
+## Contributing
 
 Contributions to this project are welcome. - see the CONTRIBUTING.md file for details.
 
-License
--------
+## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```


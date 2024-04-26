# Comparing `tmp/myelectricaldatapy-2.1.7.tar.gz` & `tmp/myelectricaldatapy-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-2.1.7.tar", last modified: Thu Apr 25 06:57:29 2024, max compression
+gzip compressed data, was "myelectricaldatapy-2.1.8.tar", last modified: Fri Apr 26 15:34:46 2024, max compression
```

## Comparing `myelectricaldatapy-2.1.7.tar` & `myelectricaldatapy-2.1.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:57:29.257364 myelectricaldatapy-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:57:29.253364 myelectricaldatapy-2.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:57:29.253364 myelectricaldatapy-2.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/.github/workflows/dependbot-auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:57:29.253364 myelectricaldatapy-2.1.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-25 06:57:29.257364 myelectricaldatapy-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:57:29.257364 myelectricaldatapy-2.1.7/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/myelectricaldatapy/mypdl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/myelectricaldatapy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:57:29.257364 myelectricaldatapy-2.1.7/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-25 06:57:29.000000 myelectricaldatapy-2.1.7/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 06:57:29.000000 myelectricaldatapy-2.1.7/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:57:29.000000 myelectricaldatapy-2.1.7/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 06:57:29.000000 myelectricaldatapy-2.1.7/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 06:57:29.000000 myelectricaldatapy-2.1.7/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:57:29.257364 myelectricaldatapy-2.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:57:29.257364 myelectricaldatapy-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-25 06:57:16.000000 myelectricaldatapy-2.1.7/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:34:46.650039 myelectricaldatapy-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:34:46.646039 myelectricaldatapy-2.1.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:34:46.646039 myelectricaldatapy-2.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/.github/workflows/dependbot-auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:34:46.646039 myelectricaldatapy-2.1.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-26 15:34:46.650039 myelectricaldatapy-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:34:46.650039 myelectricaldatapy-2.1.8/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/myelectricaldatapy/mypdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/myelectricaldatapy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:34:46.650039 myelectricaldatapy-2.1.8/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-26 15:34:46.000000 myelectricaldatapy-2.1.8/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-26 15:34:46.000000 myelectricaldatapy-2.1.8/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:34:46.000000 myelectricaldatapy-2.1.8/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 15:34:46.000000 myelectricaldatapy-2.1.8/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:34:46.000000 myelectricaldatapy-2.1.8/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:34:46.650039 myelectricaldatapy-2.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:34:46.650039 myelectricaldatapy-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11461 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-26 15:34:36.000000 myelectricaldatapy-2.1.8/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-2.1.7/.github/dependabot.yml` & `myelectricaldatapy-2.1.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/.github/workflows/dependbot-auto-approve.yml` & `myelectricaldatapy-2.1.8/.github/workflows/dependbot-auto-approve.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/.github/workflows/lint.yml` & `myelectricaldatapy-2.1.8/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/.github/workflows/pythonpublish.yml` & `myelectricaldatapy-2.1.8/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/.github/workflows/release.yml` & `myelectricaldatapy-2.1.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/.gitignore` & `myelectricaldatapy-2.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/.pre-commit-config.yaml` & `myelectricaldatapy-2.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/LICENSE` & `myelectricaldatapy-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/PKG-INFO` & `myelectricaldatapy-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.7
+Version: 2.1.8
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.7/README.md` & `myelectricaldatapy-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/example.py` & `myelectricaldatapy-2.1.8/example.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/myelectricaldatapy/analytics.py` & `myelectricaldatapy-2.1.8/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/myelectricaldatapy/auth.py` & `myelectricaldatapy-2.1.8/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-2.1.8/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-2.1.8/myelectricaldatapy/mypdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,15 @@
                 try:
                     dataset = await func(self.pdl, start, end)
                     if dataset is None or dataset.get("meter_reading") is None:
                         raise EnedisException("Data collect is empty")
                 except EnedisException as error:
                     checked = False
                     _LOGGER.error(error.args[1]["detail"])
-                data = dataset.get("meter_reading", {}).get("interval_reading", {})
-                if len(data) != 0:
-                    checked = checked and len(data) != 0
+                data = dataset.get("meter_reading", {}).get("interval_reading", [])
+                if len(data) > 0:
+                    checked = checked and len(data) > 0
                     self._params[mode].update({"data": data})
                 if mode == CONSUMPTION and self._tempo_subs:
                     self.tempo = await self._api.async_get_tempo(start, end)
 
         self.has_collected = checked
```

### Comparing `myelectricaldatapy-2.1.7/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-2.1.8/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.7
+Version: 2.1.8
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.7/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-2.1.8/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/pyproject.toml` & `myelectricaldatapy-2.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/tests/conftest.py` & `myelectricaldatapy-2.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/tests/consts.py` & `myelectricaldatapy-2.1.8/tests/consts.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.7/tests/test_analytics.py` & `myelectricaldatapy-2.1.8/tests/test_analytics.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from __future__ import annotations
 
 from datetime import datetime as dt
 from typing import Any
 from unittest.mock import Mock, patch
 
-import pytest
 from freezegun import freeze_time
+import pytest
 
 import myelectricaldatapy
 from myelectricaldatapy import EnedisByPDL
 
 from .consts import DATASET_DAILY_COMPARE, PDL, TOKEN
 
 
@@ -201,14 +201,36 @@
     assert resultat[0]["sum_value"] == resultat[0]["value"] + 1000
     assert resultat[0]["sum_price"] == resultat[0]["price"] + 75
     # standard
     assert resultat[27]["sum_value"] == resultat[27]["value"] + 100
     assert resultat[27]["sum_price"] == resultat[27]["price"] + 50
 
 
+@freeze_time("2023-03-01")
+@pytest.mark.asyncio
+async def test_extra_date(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
+    """Test cumulative summary."""
+    prices: dict[str, Any] = {"standard": {"price": 0.17}, "offpeak": {"price": 0.18}}
+    intervals = [("01:30:00", "08:00:00"), ("12:30:00", "14:00:00")]
+    api = EnedisByPDL(pdl=PDL, token=TOKEN)
+    api.set_collects(
+        "consumption_load_curve",
+        start=dt.strptime("2023-03-01", "%Y-%m-%d"),
+        end=dt.strptime("2023-03-28", "%Y-%m-%d"),
+        prices=prices,
+        intervals=intervals,
+    )
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
+    # offpeak
+    assert resultat[0]["sum_value"] is not None
+    # standard
+    assert resultat[27]["sum_value"] is not None
+
+
 @freeze_time("2023-3-1")
 @pytest.mark.asyncio
 async def test_tempo(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test tempo pricings."""
     prices: dict[str, Any] = {
         "standard": {
             "blue": 0.2,
```

### Comparing `myelectricaldatapy-2.1.7/tests/test_load_data.py` & `myelectricaldatapy-2.1.8/tests/test_load_data.py`

 * *Files identical despite different names*


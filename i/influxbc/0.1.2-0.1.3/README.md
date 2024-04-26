# Comparing `tmp/influxbc-0.1.2.tar.gz` & `tmp/influxbc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxbc-0.1.2.tar", max compression
+gzip compressed data, was "influxbc-0.1.3.tar", max compression
```

## Comparing `influxbc-0.1.2.tar` & `influxbc-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-10-20 14:43:27.670092 influxbc-0.1.2/LICENSE
--rw-r--r--   0        0        0     9056 2024-03-08 17:29:50.369350 influxbc-0.1.2/README.md
--rw-r--r--   0        0        0     1078 2024-03-08 17:47:34.960743 influxbc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      109 2023-12-07 10:46:45.783716 influxbc-0.1.2/src/influxbc/__init__.py
--rw-r--r--   0        0        0    15836 2024-03-08 17:32:04.497539 influxbc-0.1.2/src/influxbc/_base.py
--rw-r--r--   0        0        0    15734 2024-03-08 15:05:13.654770 influxbc-0.1.2/src/influxbc/client_v1.py
--rw-r--r--   0        0        0    21084 2024-03-08 15:05:13.654770 influxbc-0.1.2/src/influxbc/client_v2.py
--rw-r--r--   0        0        0      520 2023-12-07 10:46:45.787716 influxbc-0.1.2/src/influxbc/const.py
--rw-r--r--   0        0        0      612 2024-02-23 14:12:25.019421 influxbc-0.1.2/src/influxbc/errors.py
--rw-r--r--   0        0        0      304 2023-12-07 10:46:45.787716 influxbc-0.1.2/src/influxbc/logging.py
--rw-r--r--   0        0        0      127 2023-12-01 17:11:20.008363 influxbc-0.1.2/src/influxbc/typing.py
--rw-r--r--   0        0        0    10102 1970-01-01 00:00:00.000000 influxbc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-10-20 14:43:27.670092 influxbc-0.1.3/LICENSE
+-rw-r--r--   0        0        0    11002 2024-04-26 09:39:20.403367 influxbc-0.1.3/README.md
+-rw-r--r--   0        0        0     1078 2024-04-26 09:43:52.423514 influxbc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-12-07 10:46:45.783716 influxbc-0.1.3/src/influxbc/__init__.py
+-rw-r--r--   0        0        0    15836 2024-03-08 17:32:04.497539 influxbc-0.1.3/src/influxbc/_base.py
+-rw-r--r--   0        0        0    16601 2024-04-26 09:39:20.695367 influxbc-0.1.3/src/influxbc/client_v1.py
+-rw-r--r--   0        0        0    21079 2024-04-26 08:02:18.659692 influxbc-0.1.3/src/influxbc/client_v2.py
+-rw-r--r--   0        0        0      549 2024-04-26 09:28:41.723992 influxbc-0.1.3/src/influxbc/const.py
+-rw-r--r--   0        0        0      612 2024-02-23 14:12:25.019421 influxbc-0.1.3/src/influxbc/errors.py
+-rw-r--r--   0        0        0      307 2024-04-26 08:25:15.771029 influxbc-0.1.3/src/influxbc/logging.py
+-rw-r--r--   0        0        0      127 2023-12-01 17:11:20.008363 influxbc-0.1.3/src/influxbc/typing.py
+-rw-r--r--   0        0        0    12048 1970-01-01 00:00:00.000000 influxbc-0.1.3/PKG-INFO
```

### Comparing `influxbc-0.1.2/LICENSE` & `influxbc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `influxbc-0.1.2/pyproject.toml` & `influxbc-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "influxbc"
-version = "0.1.2"
+version = "0.1.3"
 description = "A universal Python client for InfluxDB"
 authors = [  # In alphabetical order of last names
     "Paul Kernstock <paul.kernstock@posteo.de>",
     "Philip Tillmann <philip.tillmann@haw-hamburg.de>",
     "Jan Trosdorff <jan.trosdorff@haw-hamburg.de>"
 ]
 maintainers = [  # In alphabetical order of last names
```

### Comparing `influxbc-0.1.2/src/influxbc/_base.py` & `influxbc-0.1.3/src/influxbc/_base.py`

 * *Files identical despite different names*

### Comparing `influxbc-0.1.2/src/influxbc/client_v1.py` & `influxbc-0.1.3/src/influxbc/client_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 from typing import Optional, Dict, Union, List
 
 import influxdb.exceptions
 import pandas as pd
 import requests
 
-from . import errors
+from . import errors, logging
 from .const import (
     INFLUX_DEFAULT_BATCH_SIZE,
 )
 from ._base import BaseClient, WriteMode, FirstLast
 
 
 class InfluxDBV1Client(influxdb.DataFrameClient, BaseClient):
@@ -362,15 +362,16 @@
         :param stop: Stop date-time to read.
             If omitted, the first point between start and InfluxDB's internal
             `now()` is returned.
         :return: First point of the specified field
             or an empty series, if none was found
         """
         select_query = (
-            f'SELECT {first_or_last.value.upper()}({field}) FROM "{measurement}"'
+            f'SELECT {first_or_last.value.upper()}("{field}") FROM'
+            f' "{measurement}"'
         )
 
         # Range
         where_query = " WHERE"
         start = self._cast_validate_date_time_string(start)
         if stop is not None:
             stop = self._cast_validate_date_time_string(stop)
@@ -384,14 +385,43 @@
                 first_or_last.value.lower()
             ]
         except KeyError:
             result = pd.Series()
 
         return result
 
+    def request(
+        self,
+        url,
+        method="GET",
+        params=None,
+        data=None,
+        stream=False,
+        expected_response_code=200,
+        headers=None,
+    ):
+        """
+        Override of influxdb.InfluxDBClient.request with extended functionality
+        - Logging of sent requests on the DEBUG level
+        For original parameters, see influxdb.InfluxDBClient.request
+        """
+        kwargs = dict(
+            url=url,
+            method=method,
+            params=params,
+            data=data,
+            stream=stream,
+            expected_response_code=expected_response_code,
+            headers=headers,
+        )
+        logging.logger.debug(
+            f"Requesting {url} with method {method} with params {params} with data {data} "
+        )
+        return super().request(**kwargs)
+
     # endregion
 
     # region Write Data
     def write_data_frame(
         self,
         data_frame: pd.DataFrame,
         measurement: str,
```

### Comparing `influxbc-0.1.2/src/influxbc/client_v2.py` & `influxbc-0.1.3/src/influxbc/client_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     # endregion
 
     # region Schema & Management
     def get_databases(self) -> List[str]:
         """
         List of all buckets of the organisation
         """
-        query = f"""    
+        query = f"""
         buckets()
         """
         tables = self.queryAPI.query(query=query, org=self.org)
 
         # Flatten output tables into list of measurements
         buckets_lst = [row.values["name"] for table in tables for row in table]
 
@@ -223,15 +223,15 @@
             if tag_key not in self.get_tag_keys():
                 msg = f'Given tag key "{tag_key}" does not exist.'
                 warnings.warn(msg)
             query = f"""
             import \"influxdata/influxdb/schema\"
 
             schema.tagValues(
-                bucket:  \"{self.bucketName}\", 
+                bucket:  \"{self.bucketName}\",
                 tag: \"{tag_key}\",
                 start: {INFLUX_EPOCH}
             )
             """
         else:
             self._warn_measurement_does_not_exist(measurement)
             if tag_key not in self.get_tag_keys(measurement=measurement):
```

### Comparing `influxbc-0.1.2/src/influxbc/const.py` & `influxbc-0.1.3/src/influxbc/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pandas as pd
 
+# region Polling
 # Default milliseconds to sleep between polls
 DEFAULT_POLL_SLEEP_MS = 60_000
 # Default time delta for how much older a point can be to be taken by a poll
 DEFAULT_POLL_VALIDITY_PERIOD = pd.Timedelta("0s")
+# endregion
 
 # region InfluxDBs internal constants
 # InfluxDB's internal Epoch
 INFLUX_EPOCH = "1970-01-01T00:00:00Z"
 # InfluxDB's internal databases/buckets
 INFLUX_V1_INT_DB = "_internal"
 INFLUX_V2_INT_DB_MONIT = "_monitoring"
```

### Comparing `influxbc-0.1.2/src/influxbc/errors.py` & `influxbc-0.1.3/src/influxbc/errors.py`

 * *Files identical despite different names*

### Comparing `influxbc-0.1.2/PKG-INFO` & `influxbc-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: influxbc
-Version: 0.1.2
-Summary: A universal Python client for InfluxDB
-Home-page: https://gitlab.com/waermewerk/influxbc
-License: MIT
-Author: Paul Kernstock
-Author-email: paul.kernstock@posteo.de
-Maintainer: Paul Kernstock
-Maintainer-email: paul.kernstock@posteo.de
-Requires-Python: >=3.8,<3.13
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: influxdb (>=5,<6)
-Requires-Dist: influxdb-client[extra] (>=1,<2)
-Requires-Dist: pandas (>=2,<3)
-Project-URL: Changelog, https://gitlab.com/waermewerk/influxbc/blob/main/CHANGELOG.md
-Project-URL: Issues, https://gitlab.com/waermewerk/influxbc/issues
-Project-URL: Repository, https://gitlab.com/waermewerk/influxbc
-Description-Content-Type: text/markdown
-
 # InfluxBC
 
 [InfluxBC as in Influx Buzz Compensator]
 
 A universal Python client for InfluxDB.
 
 This project aims to provide a higher level API and compatibility layer to InfluxData's official Python [V1](https://github.com/influxdata/influxdb-python), [V2](https://github.com/influxdata/influxdb-client-python) (and eventually [V3](https://github.com/InfluxCommunity/influxdb3-python)) client libraries.
@@ -230,23 +204,45 @@
 data = pd.DataFrame({
     "time": pd.to_datetime(["2023-02-23T15:00:00Z"]),
     "value": [10.5],
 })
 client.write_data_frame(data, measurement="my_measurement", tags={"sensor_id": "123"})
 ```
 
+### Logging
+
+InfluxBC registers a logger with the ID `influxbc` with the Python Standard Library `logging` facility.
+
+As a default, the logger is set to the `WARNING` logging level. You can set the level in your code like so:
+
+```python
+import logging
+
+from influxbc.logging import logger as influxbc_logger
+
+influxbc_logger.setLevel(logging.DEBUG)
+```
+
+Alternatively, you can set the `IBC_LOG_LEVEL` environment variable to control InfluxBC's logging level.
+
+#### Getting the Messages
+
+While the official V1 client library does not seem to provide any logging interface at all, messages from InfluxBC's logger is all you can expect.
+
+However, being a lot more complex, the official V2 client library provides [several logger instances](https://github.com/influxdata/influxdb-client-python?tab=readme-ov-file#logging) which can be used to see what's going on inside the client. To see the HTTP requests sent to the InfluxDB V2 instance for example, you can get the logger with ID `influxdb_client.client.http` and set it to the `DEBUG` level.
+
 ## Concepts
 
 - Missing data as a result of missing resources (e.g. a missing measurement, a failing filter criterion, etc.) will not raise an error but return empty data instead. This goes along best practices for HTTP APIs, which is the interface form of InfluxDB instances.
 - A client instance is always bound and connected to a database/bucket which has to be given upon client initialization (this is considered common sense in database clients).
 
 ## Rationale
 
 The core structural concept of InfluxDB has been more or less the same acros all major InfluxDB versions.
-However unfortunately, implementations such as query language, client libraries as well as concept nomenclature have not. 
+However unfortunately, implementations such as query language, client libraries as well as concept nomenclature have not.
 
 Following is an overview of consistencies and inconsistencies among InfluxDB major version.
 Please note that we're completely ignoring potential benefits which come from using or upgrading to a higher major version of InfluxDB, such as say performance aspects.
 
 |                            | V1                                  | V2                              | V3                        |
 |----------------------------|-------------------------------------|---------------------------------|---------------------------|
 | Database                   | Database                            | Bucket                          | Database                  |
@@ -263,17 +259,51 @@
 | Inclusive Range            | Arbitrary (InfluxQL)                | Flux' `range` is half-open      | Arbitrary (InfluxQL, SQL) |
 | Continuous Processing      | Continuous Queries                  | Tasks                           | (tba)                     |
 | Frontend                   | Chronograf[^chronograf]             | Built-in                        | (tba)                     |
 | Python Client              | `influxdb-python`[^v1] (archived)   | `influxdb-client-python`[^v2]   | `influxdb3-python`[^v3]   |
 | State of development[^sod] | Maintenance                         | Active                          | Prototype development     |
 
 [^v1]: https://github.com/influxdata/influxdb-python
-[^v2]: https://github.com/influxdata/influxdb-client-python 
+[^v2]: https://github.com/influxdata/influxdb-client-python
 [^v3]: https://github.com/InfluxCommunity/influxdb3-python
 [^chronograf]: https://www.influxdata.com/time-series-platform/chronograf
 [^dbrp]: https://docs.influxdata.com/influxdb/v2/reference/api/influxdb-1x/dbrp/
 [^sod]: March 2024 (https://github.com/influxdata/influxdb)
 
+## Development
+
+To set up a development environment you need a virtual environment and [Poetry](https://python-poetry.org/docs/#installation), for example:
+
+```shell
+POETRY_VIRTUALENVS_IN_PROJECT=1 poetry install
+```
+
+### Testing
+
+Tests for `influxbc` are written with `pytest`. You can run the test suite with
+
+```shell
+pytest tests
+```
+
+### Formatting
+
+We use [Black](https://black.readthedocs.io/en/stable/) as our code formatter.
+
+```shell
+black --preview .
+```
+
+## Contributing
+
+Before requesting your contribution to be merged, please make sure that
+all tests check out and that your code is properly formatted.
+
+### pre-commit
+
+Please install and use [pre-commit](https://pre-commit.com) in your development environment to simple issues up-front before committing your contribution.
+
+Going through the "Quick start" guide will install pre-commit git hooks that run automatically when you commit.
+
 ## License
 
 This project is licensed under the terms of the [MIT](https://en.wikipedia.org/wiki/MIT_License#License_terms) license.
-
```


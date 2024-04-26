# Comparing `tmp/ssb_datadoc_model-5.2.0.tar.gz` & `tmp/ssb_datadoc_model-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_datadoc_model-5.2.0.tar", max compression
+gzip compressed data, was "ssb_datadoc_model-5.3.0.tar", max compression
```

## Comparing `ssb_datadoc_model-5.2.0.tar` & `ssb_datadoc_model-5.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      628 2024-04-23 13:37:10.483633 ssb_datadoc_model-5.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-23 13:37:10.483633 ssb_datadoc_model-5.2.0/datadoc_model/__init__.py
--rw-r--r--   0        0        0      266 2024-04-23 13:37:10.483633 ssb_datadoc_model-5.2.0/datadoc_model/datadoc_base_model.py
--rw-r--r--   0        0        0    17751 2024-04-23 13:37:20.371514 ssb_datadoc_model-5.2.0/datadoc_model/model.py
--rw-r--r--   0        0        0        0 2024-04-23 13:37:10.483633 ssb_datadoc_model-5.2.0/datadoc_model/py.typed
--rw-r--r--   0        0        0      613 2024-04-23 13:37:20.371514 ssb_datadoc_model-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 ssb_datadoc_model-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0      628 2024-04-26 06:56:43.684111 ssb_datadoc_model-5.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 06:56:43.684111 ssb_datadoc_model-5.3.0/datadoc_model/__init__.py
+-rw-r--r--   0        0        0      266 2024-04-26 06:56:43.684111 ssb_datadoc_model-5.3.0/datadoc_model/datadoc_base_model.py
+-rw-r--r--   0        0        0    17761 2024-04-26 06:56:53.916288 ssb_datadoc_model-5.3.0/datadoc_model/model.py
+-rw-r--r--   0        0        0        0 2024-04-26 06:56:43.684111 ssb_datadoc_model-5.3.0/datadoc_model/py.typed
+-rw-r--r--   0        0        0      613 2024-04-26 06:56:53.916288 ssb_datadoc_model-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 ssb_datadoc_model-5.3.0/PKG-INFO
```

### Comparing `ssb_datadoc_model-5.2.0/README.md` & `ssb_datadoc_model-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ssb_datadoc_model-5.2.0/datadoc_model/model.py` & `ssb_datadoc_model-5.3.0/datadoc_model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # generated by datamodel-codegen:
 #   filename:  metadata-container-json-schema.json
-#   timestamp: 2024-04-23T13:18:29+00:00
+#   timestamp: 2024-04-25T13:29:06+00:00
 
 from __future__ import annotations
 
+from datetime import date
 from enum import Enum
 from typing import Any, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import AnyUrl, AwareDatetime, Field, RootModel
 
 from datadoc_model.datadoc_base_model import DatadocBaseModel
@@ -296,20 +297,20 @@
         title="Metadata last updated date",
     )
     metadata_last_updated_by: Optional[str] = Field(
         None,
         description="Last change made by identifiable person. ",
         title="Metadata last updated by",
     )
-    contains_data_from: Optional[str] = Field(
+    contains_data_from: Optional[date] = Field(
         None,
         description="The data set contains data from date/time",
         title="Contains data from",
     )
-    contains_data_until: Optional[str] = Field(
+    contains_data_until: Optional[date] = Field(
         None,
         description="The data set contains data up until date/time",
         title="Contains data up until",
     )
 
 
 class OtherSpecialValue(DatadocBaseModel):
@@ -418,32 +419,32 @@
         title="Custom type for variable metadata",
     )
     id: Optional[UUID] = Field(
         None,
         description="Unique SSB identifier for the instance variable in the data set",
         title="Identifier",
     )
-    contains_data_from: Optional[AwareDatetime] = Field(
+    contains_data_from: Optional[date] = Field(
         None,
         description="The instance variable in the data set contains data from and including this date. This can be useful information for data sets that contain many instance variables in addition to data for many periods/years. In many cases, it will then be the case that some variables only contain data for the most recent periods/years, e.g. if the entire data set contains data from 1970 to 2020, while some instance variables only contain data from 1998 onwards.",
         title="Contains data from",
     )
-    contains_data_until: Optional[AwareDatetime] = Field(
+    contains_data_until: Optional[date] = Field(
         None,
         description="The instance variable in the data set contains data up to and including this date. This can be useful information for data sets that contain many instance variables in addition to data for many periods/years. In many cases, it will then be the case that some of the instance variables in the data set are terminated (no longer updated) after a given point in time.",
         title="Contains data up until",
     )
 
 
 class DatadocMetadata(DatadocBaseModel):
     percentage_complete: Optional[int] = Field(
         None, description="Percentage of obligatory metadata fields populated."
     )
-    document_version: Literal["3.2.0"] = Field(
-        "3.2.0", description="Version of this model"
+    document_version: Literal["3.3.0"] = Field(
+        "3.3.0", description="Version of this model"
     )
     dataset: Optional[Dataset] = None
     variables: Optional[list[Variable]] = None
 
 
 class MetadataContainer(DatadocBaseModel):
     document_version: Literal["0.0.1"] = "0.0.1"
```

### Comparing `ssb_datadoc_model-5.2.0/pyproject.toml` & `ssb_datadoc_model-5.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-datadoc-model"
-version = "5.2.0"
+version = "5.3.0"
 description = "Data Model for use in Statistics Norway's Metadata system"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/statisticsnorway/ssb-datadoc-model"
 
 packages = [{ include = "datadoc_model" }]
```

### Comparing `ssb_datadoc_model-5.2.0/PKG-INFO` & `ssb_datadoc_model-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-datadoc-model
-Version: 5.2.0
+Version: 5.3.0
 Summary: Data Model for use in Statistics Norway's Metadata system
 Home-page: https://github.com/statisticsnorway/ssb-datadoc-model
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
```

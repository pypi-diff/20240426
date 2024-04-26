# Comparing `tmp/buildarr_prowlarr-0.5.1.tar.gz` & `tmp/buildarr_prowlarr-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr_prowlarr-0.5.1.tar", max compression
+gzip compressed data, was "buildarr_prowlarr-0.5.2.tar", max compression
```

## Comparing `buildarr_prowlarr-0.5.1.tar` & `buildarr_prowlarr-0.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/LICENSE
--rw-r--r--   0        0        0    11891 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/README.md
--rw-r--r--   0        0        0      975 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/__init__.py
--rw-r--r--   0        0        0     7086 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/api.py
--rw-r--r--   0        0        0     2881 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/cli.py
--rw-r--r--   0        0        0     5660 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/__init__.py
--rw-r--r--   0        0        0     4912 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/__init__.py
--rw-r--r--   0        0        0     1055 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/apps/__init__.py
--rw-r--r--   0        0        0    27178 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/apps/applications.py
--rw-r--r--   0        0        0     8813 2023-12-01 23:34:12.213329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/apps/sync_profiles.py
--rw-r--r--   0        0        0    10899 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/download_clients/__init__.py
--rw-r--r--   0        0        0     8509 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/download_clients/base.py
--rw-r--r--   0        0        0    32312 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/download_clients/torrent.py
--rw-r--r--   0        0        0    14395 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/download_clients/usenet.py
--rw-r--r--   0        0        0    19724 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/general.py
--rw-r--r--   0        0        0     2318 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/indexers/__init__.py
--rw-r--r--   0        0        0    31264 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/indexers/indexers.py
--rw-r--r--   0        0        0    16453 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/indexers/proxies.py
--rw-r--r--   0        0        0    43595 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/notifications.py
--rw-r--r--   0        0        0     2931 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/tags.py
--rw-r--r--   0        0        0     7227 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/ui.py
--rw-r--r--   0        0        0     1034 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/types.py
--rw-r--r--   0        0        0     1396 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/exceptions.py
--rw-r--r--   0        0        0      950 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/manager.py
--rw-r--r--   0        0        0     1189 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/plugin.py
--rw-r--r--   0        0        0        0 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/py.typed
--rw-r--r--   0        0        0     5970 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/secrets.py
--rw-r--r--   0        0        0      997 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/types.py
--rw-r--r--   0        0        0     1465 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/buildarr_prowlarr/util.py
--rw-r--r--   0        0        0     2595 2023-12-01 23:34:12.217329 buildarr_prowlarr-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    13569 1970-01-01 00:00:00.000000 buildarr_prowlarr-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/LICENSE
+-rw-r--r--   0        0        0    11891 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/README.md
+-rw-r--r--   0        0        0      975 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/__init__.py
+-rw-r--r--   0        0        0     7086 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/api.py
+-rw-r--r--   0        0        0     2881 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/cli.py
+-rw-r--r--   0        0        0     5660 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/__init__.py
+-rw-r--r--   0        0        0     4912 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/__init__.py
+-rw-r--r--   0        0        0     1055 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/__init__.py
+-rw-r--r--   0        0        0    27143 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/applications.py
+-rw-r--r--   0        0        0     8813 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/sync_profiles.py
+-rw-r--r--   0        0        0    10899 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/__init__.py
+-rw-r--r--   0        0        0     8509 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/base.py
+-rw-r--r--   0        0        0    32324 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/torrent.py
+-rw-r--r--   0        0        0    14395 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/usenet.py
+-rw-r--r--   0        0        0    19716 2024-04-26 11:13:22.945076 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/general.py
+-rw-r--r--   0        0        0     2318 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/__init__.py
+-rw-r--r--   0        0        0    31264 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/indexers.py
+-rw-r--r--   0        0        0    16453 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/proxies.py
+-rw-r--r--   0        0        0    43595 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/notifications.py
+-rw-r--r--   0        0        0     2931 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/tags.py
+-rw-r--r--   0        0        0     7227 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/ui.py
+-rw-r--r--   0        0        0     1034 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/types.py
+-rw-r--r--   0        0        0     1396 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/exceptions.py
+-rw-r--r--   0        0        0      950 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/manager.py
+-rw-r--r--   0        0        0     1189 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/py.typed
+-rw-r--r--   0        0        0     5970 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/secrets.py
+-rw-r--r--   0        0        0      997 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/types.py
+-rw-r--r--   0        0        0     1465 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/buildarr_prowlarr/util.py
+-rw-r--r--   0        0        0     2595 2024-04-26 11:13:22.949077 buildarr_prowlarr-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    13569 1970-01-01 00:00:00.000000 buildarr_prowlarr-0.5.2/PKG-INFO
```

### Comparing `buildarr_prowlarr-0.5.1/LICENSE` & `buildarr_prowlarr-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/README.md` & `buildarr_prowlarr-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/__init__.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/api.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/api.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/cli.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/cli.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/__init__.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/__init__.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/apps/__init__.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/apps/applications.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from buildarr.state import state
 from buildarr.types import BaseEnum, InstanceName, LowerCaseNonEmptyStr, NonEmptyStr, Password
 from pydantic import AnyHttpUrl, Field, SecretStr, validator
 from typing_extensions import Annotated, Self
 
 from ....api import prowlarr_api_client
 from ....secrets import ProwlarrSecrets
-from ....types import ArrApiKey
 from ...types import ProwlarrConfigBase
 
 logger = getLogger(__name__)
 
 
 class SyncLevel(BaseEnum):
     disabled = "disabled"
@@ -285,15 +284,15 @@
     """
 
     type: Literal["lidarr"] = "lidarr"
     """
     Type value associated with this kind of application.
     """
 
-    api_key: ArrApiKey
+    api_key: Password
     """
     API key used to access the target instance.
     """
 
     sync_categories: Set[LowerCaseNonEmptyStr] = {
         "Audio/MP3",  # type: ignore[arg-type]
         "Audio/Audiobook",  # type: ignore[arg-type]
@@ -351,15 +350,15 @@
 
     instance_name: Optional[InstanceName] = Field(None, plugin="radarr")
     """
     The name of the Radarr instance within Buildarr, if adding
     a Buildarr-defined Radarr instance to this Prowlarr instance.
     """
 
-    api_key: Optional[ArrApiKey] = None
+    api_key: Optional[SecretStr] = None
     """
     API key used to access the target Radarr instance.
 
     If a Radarr instance managed by Buildarr is not referenced using `instance_name`,
     this attribute is required.
     """
 
@@ -407,15 +406,15 @@
     """
 
     type: Literal["readarr"] = "readarr"
     """
     Type value associated with this kind of application.
     """
 
-    api_key: ArrApiKey
+    api_key: Password
     """
     API key used to access the target instance.
     """
 
     sync_categories: Set[LowerCaseNonEmptyStr] = {
         "Audio/Audiobook",  # type: ignore[arg-type]
         "Books/Mags",  # type: ignore[arg-type]
@@ -451,15 +450,15 @@
 
     instance_name: Optional[InstanceName] = Field(None, plugin="sonarr")
     """
     The name of the Sonarr instance within Buildarr, if adding
     a Buildarr-defined Sonarr instance to this Prowlarr instance.
     """
 
-    api_key: Optional[ArrApiKey] = None
+    api_key: Optional[SecretStr] = None
     """
     API key used to access the target Sonarr instance.
 
     If a Sonarr instance managed by Buildarr is not referenced using `instance_name`,
     this attribute is required.
     """
 
@@ -542,15 +541,15 @@
     """
 
     type: Literal["whisparr"] = "whisparr"
     """
     Type value associated with this kind of application.
     """
 
-    api_key: ArrApiKey
+    api_key: Password
     """
     API key used to access the target instance.
     """
 
     sync_categories: Set[LowerCaseNonEmptyStr] = {
         "XXX/DVD",  # type: ignore[arg-type]
         "XXX/WMV",  # type: ignore[arg-type]
```

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/apps/sync_profiles.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/apps/sync_profiles.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/download_clients/__init__.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/download_clients/base.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/download_clients/torrent.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/torrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from __future__ import annotations
 
 from logging import getLogger
 from typing import Any, Dict, List, Literal, Mapping, Optional, Set
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum, LowerCaseNonEmptyStr, NonEmptyStr, Password, Port
-from pydantic import validator
+from pydantic import SecretStr, validator
 
 from .base import DownloadClient
 
 logger = getLogger(__name__)
 
 
 class DelugePriority(BaseEnum):
@@ -998,15 +998,15 @@
     """
 
     username: Optional[str] = None
     """
     User name to use when authenticating with the download client, if required.
     """
 
-    password: Optional[Password] = None
+    password: Optional[SecretStr] = None
     """
     Password to use to authenticate the download client user, if required.
     """
 
     category: Optional[str] = None
     """
     Associate media from Prowlarr with a category.
```

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/download_clients/usenet.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/download_clients/usenet.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/general.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from ipaddress import IPv4Address
 from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Tuple, Union
 
 import prowlarr
 
 from buildarr.config import RemoteMapEntry
-from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
+from buildarr.types import BaseEnum, NonEmptyStr, Port
 from pydantic import Field, SecretStr
 from typing_extensions import Self
 
 from ...api import prowlarr_api_client
 from ...secrets import ProwlarrSecrets
 from ..types import ProwlarrConfigBase
 
@@ -260,15 +260,15 @@
     username: Optional[str] = None
     """
     Username for the administrator user. Required if authentication is enabled.
 
     Requires a restart of Prowlarr to take effect.
     """
 
-    password: Optional[Password] = None
+    password: Optional[SecretStr] = None
     """
     Password for the administrator user. Required if authentication is enabled.
 
     Requires a restart of Prowlarr to take effect.
     """
 
     certificate_validation: CertificateValidation = CertificateValidation.enabled
@@ -352,15 +352,15 @@
 
     username: Optional[str] = None
     """
     Username to authenticate with.
     Only enter if authentication is required by the proxy.
     """
 
-    password: Optional[Password] = None
+    password: Optional[SecretStr] = None
     """
     Password for the proxy user.
     Only enter if authentication is required by the proxy.
     """
 
     ignored_addresses: Set[NonEmptyStr] = set()
     """
```

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/indexers/__init__.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/indexers/indexers.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/indexers.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/indexers/proxies.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/indexers/proxies.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/notifications.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/notifications.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/tags.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/tags.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/settings/ui.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/settings/ui.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/config/types.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/exceptions.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/manager.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/manager.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/plugin.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/plugin.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/secrets.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/secrets.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/types.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/buildarr_prowlarr/util.py` & `buildarr_prowlarr-0.5.2/buildarr_prowlarr/util.py`

 * *Files identical despite different names*

### Comparing `buildarr_prowlarr-0.5.1/pyproject.toml` & `buildarr_prowlarr-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "buildarr-prowlarr"
-version = "0.5.1"
+version = "0.5.2"
 description = "Prowlarr indexer manager plugin for Buildarr"
 authors = ["Callum Dickinson <callum.dickinson.nz@gmail.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://buildarr.github.io"
 repository = "https://github.com/buildarr/buildarr-prowlarr"
 documentation = "https://buildarr.github.io/plugins/prowlarr"
 keywords = [
```

### Comparing `buildarr_prowlarr-0.5.1/PKG-INFO` & `buildarr_prowlarr-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildarr-prowlarr
-Version: 0.5.1
+Version: 0.5.2
 Summary: Prowlarr indexer manager plugin for Buildarr
 Home-page: https://buildarr.github.io
 License: GPL-3.0-or-later
 Keywords: buildarr,prowlarr,lazylibrarian,lidarr,mylar,radarr,readarr,sonarr,whisparr
 Author: Callum Dickinson
 Author-email: callum.dickinson.nz@gmail.com
 Requires-Python: >=3.8,<4.0
```


# Comparing `tmp/getstream-1.0.2rc1.tar.gz` & `tmp/getstream-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getstream-1.0.2rc1.tar", max compression
+gzip compressed data, was "getstream-1.1.0rc1.tar", max compression
```

## Comparing `getstream-1.0.2rc1.tar` & `getstream-1.1.0rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    14205 2024-04-25 17:21:06.048129 getstream-1.0.2rc1/LICENSE.md
--rw-r--r--   0        0        0     3160 2024-04-25 17:21:06.048129 getstream-1.0.2rc1/README.md
--rw-r--r--   0        0        0       50 2024-04-25 17:21:06.048129 getstream-1.0.2rc1/getstream/__init__.py
--rw-r--r--   0        0        0     6264 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/base.py
--rw-r--r--   0        0        0        0 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/chat/__init__.py
--rw-r--r--   0        0        0       24 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/chat/channel.py
--rw-r--r--   0        0        0      267 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/chat/client.py
--rw-r--r--   0        0        0    48042 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/chat/rest_client.py
--rw-r--r--   0        0        0        0 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/common/__init__.py
--rw-r--r--   0        0        0      275 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/common/client.py
--rw-r--r--   0        0        0    16606 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/common/rest_client.py
--rw-r--r--   0        0        0      925 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/config.py
--rw-r--r--   0        0        0       46 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/generic.py
--rw-r--r--   0        0        0      497 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/meta.py
--rw-r--r--   0        0        0   297290 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/models/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/rate_limit.py
--rw-r--r--   0        0        0     4061 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/stream.py
--rw-r--r--   0        0        0     1024 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/stream_response.py
--rw-r--r--   0        0        0     4057 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/utils.py
--rw-r--r--   0        0        0       22 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/version.py
--rw-r--r--   0        0        0        0 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/video/__init__.py
--rw-r--r--   0        0        0     9639 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/video/call.py
--rw-r--r--   0        0        0      817 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/video/client.py
--rw-r--r--   0        0        0    20224 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/getstream/video/rest_client.py
--rw-r--r--   0        0        0      724 2024-04-25 17:21:06.052129 getstream-1.0.2rc1/pyproject.toml
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 getstream-1.0.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    14205 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/LICENSE.md
+-rw-r--r--   0        0        0     3032 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/README.md
+-rw-r--r--   0        0        0       50 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/__init__.py
+-rw-r--r--   0        0        0     6264 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/base.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/chat/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/chat/channel.py
+-rw-r--r--   0        0        0      267 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/chat/client.py
+-rw-r--r--   0        0        0    48906 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/chat/rest_client.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/common/__init__.py
+-rw-r--r--   0        0        0      275 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/common/client.py
+-rw-r--r--   0        0        0    16606 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/common/rest_client.py
+-rw-r--r--   0        0        0      925 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/config.py
+-rw-r--r--   0        0        0       46 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/generic.py
+-rw-r--r--   0        0        0      497 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/meta.py
+-rw-r--r--   0        0        0   295611 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/models/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/rate_limit.py
+-rw-r--r--   0        0        0     4489 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/stream.py
+-rw-r--r--   0        0        0     1024 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/stream_response.py
+-rw-r--r--   0        0        0     4057 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/utils.py
+-rw-r--r--   0        0        0       22 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/version.py
+-rw-r--r--   0        0        0        0 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/video/__init__.py
+-rw-r--r--   0        0        0     9667 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/video/call.py
+-rw-r--r--   0        0        0      817 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/video/client.py
+-rw-r--r--   0        0        0    19960 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/getstream/video/rest_client.py
+-rw-r--r--   0        0        0      724 2024-04-26 08:37:44.106664 getstream-1.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3742 1970-01-01 00:00:00.000000 getstream-1.1.0rc1/PKG-INFO
```

### Comparing `getstream-1.0.2rc1/LICENSE.md` & `getstream-1.1.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `getstream-1.0.2rc1/README.md` & `getstream-1.1.0rc1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -28,32 +28,22 @@
 
 ### Users and Authentication
 
 ```python
 from getstream.models import UserRequest
 
 # sync two users using the update_users method, both users will get insert or updated
-client.update_users(users={
-    "tommaso-id": UserRequest(
-        id="tommaso-id",
-        name="tommaso",
-        role="admin",
-        custom={
-            "country": "NL"
-        }
+client.upsert_users(
+    UserRequest(
+        id="tommaso-id", name="tommaso", role="admin", custom={"country": "NL"}
     ),
-    "thierry-id": UserRequest(
-        id="thierry-id",
-        name="thierry",
-        role="admin",
-        custom={
-            "country": "US"
-        }
+    UserRequest(
+        id="thierry-id", name="thierry", role="admin", custom={"country": "US"}
     ),
-})
+)
 
 # Create a JWT token for the user to connect client-side (e.g. browser/mobile app)
 token = client.create_token("tommaso-id")
 ```
 
 ### Video API - Calls
```

### Comparing `getstream-1.0.2rc1/getstream/base.py` & `getstream-1.1.0rc1/getstream/base.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.2rc1/getstream/chat/rest_client.py` & `getstream-1.1.0rc1/getstream/chat/rest_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -919,14 +919,45 @@
         return self.get(
             "/api/v2/chat/messages/{id}/reactions",
             GetReactionsResponse,
             query_params=query_params,
             path_params=path_params,
         )
 
+    def query_reactions(
+        self,
+        id: str,
+        limit: Optional[int] = None,
+        next: Optional[str] = None,
+        prev: Optional[str] = None,
+        user_id: Optional[str] = None,
+        sort: Optional[List[Optional[SortParam]]] = None,
+        filter: Optional[Dict[str, object]] = None,
+        user: Optional[UserRequest] = None,
+    ) -> StreamResponse[QueryReactionsResponse]:
+        path_params = {
+            "id": id,
+        }
+        json = build_body_dict(
+            limit=limit,
+            next=next,
+            prev=prev,
+            user_id=user_id,
+            sort=sort,
+            filter=filter,
+            user=user,
+        )
+
+        return self.post(
+            "/api/v2/chat/messages/{id}/reactions",
+            QueryReactionsResponse,
+            path_params=path_params,
+            json=json,
+        )
+
     def translate_message(
         self, id: str, language: str
     ) -> StreamResponse[MessageResponse]:
         path_params = {
             "id": id,
         }
         json = build_body_dict(language=language)
```

### Comparing `getstream-1.0.2rc1/getstream/common/rest_client.py` & `getstream-1.1.0rc1/getstream/common/rest_client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.2rc1/getstream/config.py` & `getstream-1.1.0rc1/getstream/config.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.2rc1/getstream/models/__init__.py` & `getstream-1.1.0rc1/getstream/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2824,18 +2824,22 @@
 class GeofenceSettingsResponse(DataClassJsonMixin):
     names: List[str] = dc_field(metadata=dc_config(field_name="names"))
 
 
 @dataclass
 class GeolocationResult(DataClassJsonMixin):
     accuracy_radius: int = dc_field(metadata=dc_config(field_name="accuracy_radius"))
+    city: str = dc_field(metadata=dc_config(field_name="city"))
+    continent: str = dc_field(metadata=dc_config(field_name="continent"))
     continent_code: str = dc_field(metadata=dc_config(field_name="continent_code"))
+    country: str = dc_field(metadata=dc_config(field_name="country"))
     country_iso_code: str = dc_field(metadata=dc_config(field_name="country_iso_code"))
     latitude: float = dc_field(metadata=dc_config(field_name="latitude"))
     longitude: float = dc_field(metadata=dc_config(field_name="longitude"))
+    subdivision: str = dc_field(metadata=dc_config(field_name="subdivision"))
     subdivision_iso_code: str = dc_field(
         metadata=dc_config(field_name="subdivision_iso_code")
     )
 
 
 @dataclass
 class GetApplicationResponse(DataClassJsonMixin):
@@ -3555,14 +3559,24 @@
     country_iso_code: str = dc_field(metadata=dc_config(field_name="country_iso_code"))
     subdivision_iso_code: str = dc_field(
         metadata=dc_config(field_name="subdivision_iso_code")
     )
 
 
 @dataclass
+class MOSStats(DataClassJsonMixin):
+    average_score: float = dc_field(metadata=dc_config(field_name="average_score"))
+    max_score: float = dc_field(metadata=dc_config(field_name="max_score"))
+    min_score: float = dc_field(metadata=dc_config(field_name="min_score"))
+    hist_og_ram_duration_seconds: "List[float]" = dc_field(
+        metadata=dc_config(field_name="histogram_duration_seconds")
+    )
+
+
+@dataclass
 class MarkChannelsReadRequest(DataClassJsonMixin):
     user_id: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="user_id")
     )
     read_by_channel: "Optional[Dict[str, str]]" = dc_field(
         default=None, metadata=dc_config(field_name="read_by_channel")
     )
@@ -3674,15 +3688,14 @@
     )
     deleted_reply_count: int = dc_field(
         metadata=dc_config(field_name="deleted_reply_count")
     )
     html: str = dc_field(metadata=dc_config(field_name="html"))
     id: str = dc_field(metadata=dc_config(field_name="id"))
     pinned: bool = dc_field(metadata=dc_config(field_name="pinned"))
-    poll_id: str = dc_field(metadata=dc_config(field_name="poll_id"))
     reply_count: int = dc_field(metadata=dc_config(field_name="reply_count"))
     shadowed: bool = dc_field(metadata=dc_config(field_name="shadowed"))
     silent: bool = dc_field(metadata=dc_config(field_name="silent"))
     text: str = dc_field(metadata=dc_config(field_name="text"))
     type: str = dc_field(metadata=dc_config(field_name="type"))
     updated_at: datetime = dc_field(
         metadata=dc_config(
@@ -3704,14 +3717,17 @@
     own_reactions: "List[Optional[Reaction]]" = dc_field(
         metadata=dc_config(field_name="own_reactions")
     )
     custom: Dict[str, object] = dc_field(metadata=dc_config(field_name="custom"))
     reaction_counts: "Dict[str, int]" = dc_field(
         metadata=dc_config(field_name="reaction_counts")
     )
+    reaction_groups: "Dict[str, Optional[ReactionGroupResponse]]" = dc_field(
+        metadata=dc_config(field_name="reaction_groups")
+    )
     reaction_scores: "Dict[str, int]" = dc_field(
         metadata=dc_config(field_name="reaction_scores")
     )
     before_message_send_failed: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="before_message_send_failed")
     )
     command: Optional[str] = dc_field(
@@ -3753,14 +3769,17 @@
         metadata=dc_config(
             field_name="pinned_at",
             encoder=encode_datetime,
             decoder=datetime_from_unix_ns,
             mm_field=fields.DateTime(format="iso"),
         ),
     )
+    poll_id: Optional[str] = dc_field(
+        default=None, metadata=dc_config(field_name="poll_id")
+    )
     quoted_message_id: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="quoted_message_id")
     )
     show_in_channel: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="show_in_channel")
     )
     thread_participants: "Optional[List[UserObject]]" = dc_field(
@@ -3925,74 +3944,14 @@
     moderation_thresholds: "Optional[Thresholds]" = dc_field(
         default=None, metadata=dc_config(field_name="moderation_thresholds")
     )
 
 
 @dataclass
 class MessagePaginationParams(DataClassJsonMixin):
-    created_at_after: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_after",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_after_or_equal: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_after_or_equal",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_around: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_around",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_before: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_before",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_before_or_equal: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_before_or_equal",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    id_around: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="id_around")
-    )
-    id_gt: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="id_gt")
-    )
-    id_gte: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="id_gte")
-    )
-    id_lt: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="id_lt")
-    )
-    id_lte: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="id_lte")
-    )
     limit: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="limit")
     )
     offset: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="offset")
     )
 
@@ -4096,15 +4055,14 @@
     )
     deleted_reply_count: int = dc_field(
         metadata=dc_config(field_name="deleted_reply_count")
     )
     html: str = dc_field(metadata=dc_config(field_name="html"))
     id: str = dc_field(metadata=dc_config(field_name="id"))
     pinned: bool = dc_field(metadata=dc_config(field_name="pinned"))
-    poll_id: str = dc_field(metadata=dc_config(field_name="poll_id"))
     reply_count: int = dc_field(metadata=dc_config(field_name="reply_count"))
     shadowed: bool = dc_field(metadata=dc_config(field_name="shadowed"))
     silent: bool = dc_field(metadata=dc_config(field_name="silent"))
     text: str = dc_field(metadata=dc_config(field_name="text"))
     type: str = dc_field(metadata=dc_config(field_name="type"))
     updated_at: datetime = dc_field(
         metadata=dc_config(
@@ -4173,14 +4131,17 @@
         metadata=dc_config(
             field_name="pinned_at",
             encoder=encode_datetime,
             decoder=datetime_from_unix_ns,
             mm_field=fields.DateTime(format="iso"),
         ),
     )
+    poll_id: Optional[str] = dc_field(
+        default=None, metadata=dc_config(field_name="poll_id")
+    )
     quoted_message_id: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="quoted_message_id")
     )
     show_in_channel: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="show_in_channel")
     )
     thread_participants: "Optional[List[UserResponse]]" = dc_field(
@@ -4197,14 +4158,17 @@
     )
     poll: "Optional[Poll]" = dc_field(
         default=None, metadata=dc_config(field_name="poll")
     )
     quoted_message: "Optional[Message]" = dc_field(
         default=None, metadata=dc_config(field_name="quoted_message")
     )
+    reaction_groups: "Optional[Dict[str, Optional[ReactionGroupResponse]]]" = dc_field(
+        default=None, metadata=dc_config(field_name="reaction_groups")
+    )
 
 
 @dataclass
 class MessageUpdate(DataClassJsonMixin):
     old_text: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="old_text")
     )
@@ -4226,15 +4190,14 @@
     )
     deleted_reply_count: int = dc_field(
         metadata=dc_config(field_name="deleted_reply_count")
     )
     html: str = dc_field(metadata=dc_config(field_name="html"))
     id: str = dc_field(metadata=dc_config(field_name="id"))
     pinned: bool = dc_field(metadata=dc_config(field_name="pinned"))
-    poll_id: str = dc_field(metadata=dc_config(field_name="poll_id"))
     reply_count: int = dc_field(metadata=dc_config(field_name="reply_count"))
     shadowed: bool = dc_field(metadata=dc_config(field_name="shadowed"))
     silent: bool = dc_field(metadata=dc_config(field_name="silent"))
     text: str = dc_field(metadata=dc_config(field_name="text"))
     type: str = dc_field(metadata=dc_config(field_name="type"))
     updated_at: datetime = dc_field(
         metadata=dc_config(
@@ -4304,14 +4267,17 @@
         metadata=dc_config(
             field_name="pinned_at",
             encoder=encode_datetime,
             decoder=datetime_from_unix_ns,
             mm_field=fields.DateTime(format="iso"),
         ),
     )
+    poll_id: Optional[str] = dc_field(
+        default=None, metadata=dc_config(field_name="poll_id")
+    )
     quoted_message_id: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="quoted_message_id")
     )
     show_in_channel: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="show_in_channel")
     )
     thread_participants: "Optional[List[UserResponse]]" = dc_field(
@@ -4328,14 +4294,17 @@
     )
     poll: "Optional[Poll]" = dc_field(
         default=None, metadata=dc_config(field_name="poll")
     )
     quoted_message: "Optional[Message]" = dc_field(
         default=None, metadata=dc_config(field_name="quoted_message")
     )
+    reaction_groups: "Optional[Dict[str, Optional[ReactionGroupResponse]]]" = dc_field(
+        default=None, metadata=dc_config(field_name="reaction_groups")
+    )
 
 
 @dataclass
 class ModerationResponse(DataClassJsonMixin):
     action: str = dc_field(metadata=dc_config(field_name="action"))
     explicit: float = dc_field(metadata=dc_config(field_name="explicit"))
     spam: float = dc_field(metadata=dc_config(field_name="spam"))
@@ -4590,26 +4559,14 @@
     push_notifications: "Optional[PushNotificationSettings]" = dc_field(
         default=None, metadata=dc_config(field_name="push_notifications")
     )
 
 
 @dataclass
 class PaginationParams(DataClassJsonMixin):
-    id_gt: Optional[int] = dc_field(
-        default=None, metadata=dc_config(field_name="id_gt")
-    )
-    id_gte: Optional[int] = dc_field(
-        default=None, metadata=dc_config(field_name="id_gte")
-    )
-    id_lt: Optional[int] = dc_field(
-        default=None, metadata=dc_config(field_name="id_lt")
-    )
-    id_lte: Optional[int] = dc_field(
-        default=None, metadata=dc_config(field_name="id_lte")
-    )
     limit: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="limit")
     )
     offset: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="offset")
     )
 
@@ -5180,50 +5137,14 @@
 
 
 @dataclass
 class QueryBannedUsersRequest(DataClassJsonMixin):
     filter_conditions: Dict[str, object] = dc_field(
         metadata=dc_config(field_name="filter_conditions")
     )
-    created_at_after: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_after",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_after_or_equal: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_after_or_equal",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_before: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_before",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_before_or_equal: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_before_or_equal",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
     exclude_expired_bans: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="exclude_expired_bans")
     )
     limit: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="limit")
     )
     offset: Optional[int] = dc_field(
@@ -5301,17 +5222,14 @@
 @dataclass
 class QueryCallsRequest(DataClassJsonMixin):
     limit: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="limit")
     )
     next: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="next"))
     prev: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="prev"))
-    watch: Optional[bool] = dc_field(
-        default=None, metadata=dc_config(field_name="watch")
-    )
     sort: "Optional[List[Optional[SortParam]]]" = dc_field(
         default=None, metadata=dc_config(field_name="sort")
     )
     filter_conditions: Optional[Dict[str, object]] = dc_field(
         default=None, metadata=dc_config(field_name="filter_conditions")
     )
 
@@ -5367,72 +5285,24 @@
 
 @dataclass
 class QueryMembersRequest(DataClassJsonMixin):
     type: str = dc_field(metadata=dc_config(field_name="type"))
     filter_conditions: Dict[str, object] = dc_field(
         metadata=dc_config(field_name="filter_conditions")
     )
-    created_at_after: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_after",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_after_or_equal: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_after_or_equal",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_before: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_before",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
-    created_at_before_or_equal: Optional[datetime] = dc_field(
-        default=None,
-        metadata=dc_config(
-            field_name="created_at_before_or_equal",
-            encoder=encode_datetime,
-            decoder=datetime_from_unix_ns,
-            mm_field=fields.DateTime(format="iso"),
-        ),
-    )
     id: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="id"))
     limit: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="limit")
     )
     offset: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="offset")
     )
     user_id: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="user_id")
     )
-    user_id_gt: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="user_id_gt")
-    )
-    user_id_gte: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="user_id_gte")
-    )
-    user_id_lt: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="user_id_lt")
-    )
-    user_id_lte: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="user_id_lte")
-    )
     members: "Optional[List[Optional[ChannelMember]]]" = dc_field(
         default=None, metadata=dc_config(field_name="members")
     )
     sort: "Optional[List[Optional[SortParam]]]" = dc_field(
         default=None, metadata=dc_config(field_name="sort")
     )
     user: "Optional[UserRequest]" = dc_field(
@@ -5508,14 +5378,45 @@
     duration: str = dc_field(metadata=dc_config(field_name="duration"))
     polls: "List[PollResponseData]" = dc_field(metadata=dc_config(field_name="polls"))
     next: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="next"))
     prev: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="prev"))
 
 
 @dataclass
+class QueryReactionsRequest(DataClassJsonMixin):
+    limit: Optional[int] = dc_field(
+        default=None, metadata=dc_config(field_name="limit")
+    )
+    next: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="next"))
+    prev: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="prev"))
+    user_id: Optional[str] = dc_field(
+        default=None, metadata=dc_config(field_name="user_id")
+    )
+    sort: "Optional[List[Optional[SortParam]]]" = dc_field(
+        default=None, metadata=dc_config(field_name="sort")
+    )
+    filter: Optional[Dict[str, object]] = dc_field(
+        default=None, metadata=dc_config(field_name="filter")
+    )
+    user: "Optional[UserRequest]" = dc_field(
+        default=None, metadata=dc_config(field_name="user")
+    )
+
+
+@dataclass
+class QueryReactionsResponse(DataClassJsonMixin):
+    duration: str = dc_field(metadata=dc_config(field_name="duration"))
+    reactions: "List[ReactionResponse]" = dc_field(
+        metadata=dc_config(field_name="reactions")
+    )
+    next: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="next"))
+    prev: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="prev"))
+
+
+@dataclass
 class QueryThreadsRequest(DataClassJsonMixin):
     limit: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="limit")
     )
     next: Optional[str] = dc_field(default=None, metadata=dc_config(field_name="next"))
     participant_limit: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="participant_limit")
@@ -5543,26 +5444,14 @@
 
 
 @dataclass
 class QueryUsersPayload(DataClassJsonMixin):
     filter_conditions: Dict[str, object] = dc_field(
         metadata=dc_config(field_name="filter_conditions")
     )
-    id_gt: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="id_gt")
-    )
-    id_gte: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="id_gte")
-    )
-    id_lt: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="id_lt")
-    )
-    id_lte: Optional[str] = dc_field(
-        default=None, metadata=dc_config(field_name="id_lte")
-    )
     include_deactivated_users: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="include_deactivated_users")
     )
     limit: Optional[int] = dc_field(
         default=None, metadata=dc_config(field_name="limit")
     )
     offset: Optional[int] = dc_field(
@@ -5620,14 +5509,36 @@
     )
     user: "Optional[UserObject]" = dc_field(
         default=None, metadata=dc_config(field_name="user")
     )
 
 
 @dataclass
+class ReactionGroupResponse(DataClassJsonMixin):
+    count: int = dc_field(metadata=dc_config(field_name="count"))
+    first_reaction_at: datetime = dc_field(
+        metadata=dc_config(
+            field_name="first_reaction_at",
+            encoder=encode_datetime,
+            decoder=datetime_from_unix_ns,
+            mm_field=fields.DateTime(format="iso"),
+        )
+    )
+    last_reaction_at: datetime = dc_field(
+        metadata=dc_config(
+            field_name="last_reaction_at",
+            encoder=encode_datetime,
+            decoder=datetime_from_unix_ns,
+            mm_field=fields.DateTime(format="iso"),
+        )
+    )
+    sum_scores: int = dc_field(metadata=dc_config(field_name="sum_scores"))
+
+
+@dataclass
 class ReactionRemovalResponse(DataClassJsonMixin):
     duration: str = dc_field(metadata=dc_config(field_name="duration"))
     message: "Optional[Message]" = dc_field(
         default=None, metadata=dc_config(field_name="message")
     )
     reaction: "Optional[Reaction]" = dc_field(
         default=None, metadata=dc_config(field_name="reaction")
@@ -5975,15 +5886,14 @@
     )
     deleted_reply_count: int = dc_field(
         metadata=dc_config(field_name="deleted_reply_count")
     )
     html: str = dc_field(metadata=dc_config(field_name="html"))
     id: str = dc_field(metadata=dc_config(field_name="id"))
     pinned: bool = dc_field(metadata=dc_config(field_name="pinned"))
-    poll_id: str = dc_field(metadata=dc_config(field_name="poll_id"))
     reply_count: int = dc_field(metadata=dc_config(field_name="reply_count"))
     shadowed: bool = dc_field(metadata=dc_config(field_name="shadowed"))
     silent: bool = dc_field(metadata=dc_config(field_name="silent"))
     text: str = dc_field(metadata=dc_config(field_name="text"))
     type: str = dc_field(metadata=dc_config(field_name="type"))
     updated_at: datetime = dc_field(
         metadata=dc_config(
@@ -6005,14 +5915,17 @@
     own_reactions: "List[Optional[Reaction]]" = dc_field(
         metadata=dc_config(field_name="own_reactions")
     )
     custom: Dict[str, object] = dc_field(metadata=dc_config(field_name="custom"))
     reaction_counts: "Dict[str, int]" = dc_field(
         metadata=dc_config(field_name="reaction_counts")
     )
+    reaction_groups: "Dict[str, Optional[ReactionGroupResponse]]" = dc_field(
+        metadata=dc_config(field_name="reaction_groups")
+    )
     reaction_scores: "Dict[str, int]" = dc_field(
         metadata=dc_config(field_name="reaction_scores")
     )
     before_message_send_failed: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="before_message_send_failed")
     )
     command: Optional[str] = dc_field(
@@ -6054,14 +5967,17 @@
         metadata=dc_config(
             field_name="pinned_at",
             encoder=encode_datetime,
             decoder=datetime_from_unix_ns,
             mm_field=fields.DateTime(format="iso"),
         ),
     )
+    poll_id: Optional[str] = dc_field(
+        default=None, metadata=dc_config(field_name="poll_id")
+    )
     quoted_message_id: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="quoted_message_id")
     )
     show_in_channel: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="show_in_channel")
     )
     thread_participants: "Optional[List[UserObject]]" = dc_field(
@@ -7515,14 +7431,17 @@
 class UpdateUsersRequest(DataClassJsonMixin):
     users: "Dict[str, UserRequest]" = dc_field(metadata=dc_config(field_name="users"))
 
 
 @dataclass
 class UpdateUsersResponse(DataClassJsonMixin):
     duration: str = dc_field(metadata=dc_config(field_name="duration"))
+    membership_deletion_task_id: str = dc_field(
+        metadata=dc_config(field_name="membership_deletion_task_id")
+    )
     users: "Dict[str, FullUserResponse]" = dc_field(
         metadata=dc_config(field_name="users")
     )
 
 
 @dataclass
 class UpsertPushProviderRequest(DataClassJsonMixin):
@@ -7777,14 +7696,20 @@
 
 
 @dataclass
 class UserSessionStats(DataClassJsonMixin):
     freeze_duration_seconds: int = dc_field(
         metadata=dc_config(field_name="freeze_duration_seconds")
     )
+    max_freeze_fraction: float = dc_field(
+        metadata=dc_config(field_name="max_freeze_fraction")
+    )
+    max_freezes_duration_seconds: int = dc_field(
+        metadata=dc_config(field_name="max_freezes_duration_seconds")
+    )
     packet_loss_fraction: float = dc_field(
         metadata=dc_config(field_name="packet_loss_fraction")
     )
     publishing_duration_seconds: int = dc_field(
         metadata=dc_config(field_name="publishing_duration_seconds")
     )
     quality_score: float = dc_field(metadata=dc_config(field_name="quality_score"))
@@ -7808,14 +7733,17 @@
     )
     device_model: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="device_model")
     )
     device_version: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="device_version")
     )
+    distance_to_sfu_kilometers: Optional[float] = dc_field(
+        default=None, metadata=dc_config(field_name="distance_to_sfu_kilometers")
+    )
     max_fir_per_second: Optional[float] = dc_field(
         default=None, metadata=dc_config(field_name="max_fir_per_second")
     )
     max_freezes_per_second: Optional[float] = dc_field(
         default=None, metadata=dc_config(field_name="max_freezes_per_second")
     )
     max_nack_per_second: Optional[float] = dc_field(
@@ -7855,14 +7783,20 @@
     )
     max_publishing_video_quality: "Optional[VideoQuality]" = dc_field(
         default=None, metadata=dc_config(field_name="max_publishing_video_quality")
     )
     max_receiving_video_quality: "Optional[VideoQuality]" = dc_field(
         default=None, metadata=dc_config(field_name="max_receiving_video_quality")
     )
+    publisher_audio_mos: "Optional[MOSStats]" = dc_field(
+        default=None, metadata=dc_config(field_name="publisher_audio_mos")
+    )
+    subscriber_audio_mos: "Optional[MOSStats]" = dc_field(
+        default=None, metadata=dc_config(field_name="subscriber_audio_mos")
+    )
     timeline: "Optional[CallTimeline]" = dc_field(
         default=None, metadata=dc_config(field_name="timeline")
     )
 
 
 @dataclass
 class UserStats(DataClassJsonMixin):
```

### Comparing `getstream-1.0.2rc1/getstream/rate_limit.py` & `getstream-1.1.0rc1/getstream/rate_limit.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.2rc1/getstream/stream.py` & `getstream-1.1.0rc1/getstream/stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 import jwt
 from functools import cached_property
 from typing import List
 
 from getstream.chat.client import ChatClient
 from getstream.common.client import CommonClient
+from getstream.models import UserRequest
 from getstream.utils import validate_and_clean_url
 from getstream.video.client import VideoClient
 
 BASE_URL = "https://chat.stream-io-api.com/"
 
 
 class Stream(CommonClient):
@@ -63,14 +64,23 @@
         return ChatClient(
             api_key=self.api_key,
             base_url=self.base_url,
             token=self.token,
             timeout=self.timeout,
         )
 
+    def upsert_users(self, *users: UserRequest):
+        """
+        Creates or updates users. This method performs an "upsert" operation,
+        where it checks if each user already exists and updates their information
+        if they do, or creates a new user entry if they do not.
+        """
+        users_map = {u.id: u for u in users}
+        return self.update_users(users_map)
+
     def create_token(
         self,
         user_id: str,
         expiration: int = None,
     ):
         """
             Generates a token for a given user, with an optional expiration time.
```

### Comparing `getstream-1.0.2rc1/getstream/stream_response.py` & `getstream-1.1.0rc1/getstream/stream_response.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.2rc1/getstream/utils.py` & `getstream-1.1.0rc1/getstream/utils.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.2rc1/getstream/video/call.py` & `getstream-1.1.0rc1/getstream/video/call.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,7 +262,9 @@
             id=self.id,
             user_id=user_id,
             grant_permissions=grant_permissions,
             revoke_permissions=revoke_permissions,
         )
         self._sync_from_response(response.data)
         return response
+
+    create = get_or_create
```

### Comparing `getstream-1.0.2rc1/getstream/video/client.py` & `getstream-1.1.0rc1/getstream/video/client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.2rc1/getstream/video/rest_client.py` & `getstream-1.1.0rc1/getstream/video/rest_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,38 +507,29 @@
             UpdateUserPermissionsResponse,
             path_params=path_params,
             json=json,
         )
 
     def query_calls(
         self,
-        connection_id: Optional[str] = None,
         limit: Optional[int] = None,
         next: Optional[str] = None,
         prev: Optional[str] = None,
-        watch: Optional[bool] = None,
         sort: Optional[List[Optional[SortParam]]] = None,
         filter_conditions: Optional[Dict[str, object]] = None,
     ) -> StreamResponse[QueryCallsResponse]:
-        query_params = build_query_param(connection_id=connection_id)
         json = build_body_dict(
             limit=limit,
             next=next,
             prev=prev,
-            watch=watch,
             sort=sort,
             filter_conditions=filter_conditions,
         )
 
-        return self.post(
-            "/api/v2/video/calls",
-            QueryCallsResponse,
-            query_params=query_params,
-            json=json,
-        )
+        return self.post("/api/v2/video/calls", QueryCallsResponse, json=json)
 
     def list_call_types(self) -> StreamResponse[ListCallTypeResponse]:
         return self.get("/api/v2/video/calltypes", ListCallTypeResponse)
 
     def create_call_type(
         self,
         name: str,
```

### Comparing `getstream-1.0.2rc1/pyproject.toml` & `getstream-1.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getstream"
-version = "1.0.2-rc1"
+version = "1.1.0-rc1"
 description = ""
 authors = [
     "sachaarbonel <sacha.arbonel@hotmail.fr>",
     "tbarbugli <tbarbugli@gmail.com>"
 ]
 readme = "README.md"
```

### Comparing `getstream-1.0.2rc1/PKG-INFO` & `getstream-1.1.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getstream
-Version: 1.0.2rc1
+Version: 1.1.0rc1
 Summary: 
 Author: sachaarbonel
 Author-email: sacha.arbonel@hotmail.fr
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -48,32 +48,22 @@
 
 ### Users and Authentication
 
 ```python
 from getstream.models import UserRequest
 
 # sync two users using the update_users method, both users will get insert or updated
-client.update_users(users={
-    "tommaso-id": UserRequest(
-        id="tommaso-id",
-        name="tommaso",
-        role="admin",
-        custom={
-            "country": "NL"
-        }
+client.upsert_users(
+    UserRequest(
+        id="tommaso-id", name="tommaso", role="admin", custom={"country": "NL"}
     ),
-    "thierry-id": UserRequest(
-        id="thierry-id",
-        name="thierry",
-        role="admin",
-        custom={
-            "country": "US"
-        }
+    UserRequest(
+        id="thierry-id", name="thierry", role="admin", custom={"country": "US"}
     ),
-})
+)
 
 # Create a JWT token for the user to connect client-side (e.g. browser/mobile app)
 token = client.create_token("tommaso-id")
 ```
 
 ### Video API - Calls
```


# Comparing `tmp/nonebot_adapter_feishu-2.5.0.tar.gz` & `tmp/nonebot_adapter_feishu-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_feishu-2.5.0.tar", max compression
+gzip compressed data, was "nonebot_adapter_feishu-2.6.0.tar", max compression
```

## Comparing `nonebot_adapter_feishu-2.5.0.tar` & `nonebot_adapter_feishu-2.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1064 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/LICENSE
--rw-r--r--   0        0        0     2459 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/README.md
--rw-r--r--   0        0        0      863 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/__init__.py
--rw-r--r--   0        0        0    11552 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/adapter.py
--rw-r--r--   0        0        0    10938 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/bot.py
--rw-r--r--   0        0        0     1366 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/config.py
--rw-r--r--   0        0        0    12019 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/event.py
--rw-r--r--   0        0        0     1348 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/exception.py
--rw-r--r--   0        0        0    16590 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/message.py
--rw-r--r--   0        0        0       69 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/__init__.py
--rw-r--r--   0        0        0      725 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/api.py
--rw-r--r--   0        0        0    12854 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/common.py
--rw-r--r--   0        0        0      911 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/utils.py
--rw-r--r--   0        0        0     2386 2024-04-13 03:06:29.510895 nonebot_adapter_feishu-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/LICENSE
+-rw-r--r--   0        0        0     2459 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/README.md
+-rw-r--r--   0        0        0      863 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/__init__.py
+-rw-r--r--   0        0        0    11669 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/adapter.py
+-rw-r--r--   0        0        0    10926 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/bot.py
+-rw-r--r--   0        0        0     1360 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/config.py
+-rw-r--r--   0        0        0    12013 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/event.py
+-rw-r--r--   0        0        0     1348 2024-04-26 02:38:59.055566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/exception.py
+-rw-r--r--   0        0        0    16543 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/message.py
+-rw-r--r--   0        0        0       69 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/__init__.py
+-rw-r--r--   0        0        0      700 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/api.py
+-rw-r--r--   0        0        0    12848 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/common.py
+-rw-r--r--   0        0        0      911 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/utils.py
+-rw-r--r--   0        0        0     2387 2024-04-26 02:38:59.059566 nonebot_adapter_feishu-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 nonebot_adapter_feishu-2.6.0/PKG-INFO
```

### Comparing `nonebot_adapter_feishu-2.5.0/LICENSE` & `nonebot_adapter_feishu-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.5.0/README.md` & `nonebot_adapter_feishu-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 <p align="center">
   <a href="https://raw.githubusercontent.com/nonebot/adapter-feishu/master/LICENSE">
     <img src="https://img.shields.io/github/license/nonebot/adapter-feishu" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-adapter-feishu">
     <img src="https://img.shields.io/pypi/v/nonebot-adapter-feishu" alt="pypi">
   </a>
-  <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python">
+  <img src="https://img.shields.io/badge/python-3.9+-blue" alt="python">
   <a href="https://codecov.io/gh/nonebot/adapter-feishu">
     <img src="https://codecov.io/gh/nonebot/adapter-feishu/branch/master/graph/badge.svg?token=45OH1IVM9C"/>
   </a>
   <a href="https://github.com/nonebot/adapter-feishu/actions/workflows/website-deploy.yml">
     <img src="https://github.com/nonebot/adapter-feishu/actions/workflows/website-deploy.yml/badge.svg?branch=master&event=push" alt="site"/>
   </a>
   <a href="https://results.pre-commit.ci/latest/github/nonebot/adapter-feishu/master">
```

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/__init__.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/adapter.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import asyncio
 import inspect
 from typing_extensions import override
-from typing import Any, Dict, List, Type, Union, Callable, Optional, cast
+from typing import Any, Union, Callable, Optional, cast
 
 from pygtrie import StringTrie
 from nonebot.utils import escape_tag
 from nonebot.compat import type_validate_python
 from nonebot.drivers import (
     URL,
     Driver,
@@ -42,15 +42,15 @@
         event_models["." + model.__event__] = model
 
     @override
     def __init__(self, driver: Driver, **kwargs: Any):
         super().__init__(driver, **kwargs)
         """飞书适配器配置"""
         self.feishu_config: Config = get_plugin_config(Config)
-        self.bot_apps: Dict[str, BotConfig] = {}
+        self.bot_apps: dict[str, BotConfig] = {}
         self.setup()
 
     @classmethod
     @override
     def get_name(cls) -> str:
         """适配器名称: `Feishu`"""
         return "Feishu"
@@ -158,27 +158,31 @@
             expire -= 30 * 60
 
         await cache.set(key, result.tenant_access_token, expire)
 
         return result.tenant_access_token
 
     async def send_request(self, request: Request, **data: Any):
+        return_response = data.get("_return_response", False)
         timeout: float = data.get("_timeout", self.config.api_timeout)
         request.timeout = timeout
 
         if not isinstance(self.driver, HTTPClientMixin):
             raise ApiNotAvailable
 
         try:
             response = await self.driver.request(request)
 
             if 200 <= response.status_code < 300:
                 if not response.content:
                     raise ValueError("Empty response")
 
+                if return_response:
+                    return response
+
                 if response.headers["Content-Type"].find("application/json") != -1:
                     result = json.loads(response.content)
                     return result
                 else:
                     return response.content
 
             raise NetworkError(
@@ -308,27 +312,27 @@
                 "ERROR",
                 "<r><bg #f8bbd0>Failed to parse event. "
                 f"Raw: {escape_tag(str(json_data))}</bg #f8bbd0></r>",
                 e,
             )
 
     @classmethod
-    def add_custom_model(cls, model: Type[Event]) -> None:
+    def add_custom_model(cls, model: type[Event]) -> None:
         """插入或覆盖一个自定义的 Event 类型。
         需提供 `__event__` 属性，进行事件模型索引，
         格式为 `{post_type}[.{sub_type}]`，如: `message.private`。
         参数:
             model: 自定义的 Event 类型
         """
         if not hasattr(model, "__event__"):
             raise ValueError("Event model's `__event__` attribute must be set")
         cls.event_models["." + model.__event__] = model
 
     @classmethod
-    def get_event_model(cls, event_name: str) -> List[Type[Event]]:
+    def get_event_model(cls, event_name: str) -> list[type[Event]]:
         """根据事件名获取对应 `Event Model` 及 `FallBack Event Model` 列表，
         不包括基类 `Event`。
         """
         return [model.value for model in cls.event_models.prefixes("." + event_name)][
             ::-1
         ]
```

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/bot.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from typing_extensions import override
-from typing import TYPE_CHECKING, Any, Dict, List, Union, Literal, Callable, Optional
+from typing import TYPE_CHECKING, Any, Union, Literal, Callable, Optional
 
 from nonebot.message import handle_event
 from nonebot.compat import type_validate_python
 
 from nonebot.adapters import Bot as BaseBot
 
 from .utils import log
@@ -226,30 +226,30 @@
     async def get_msg_read_users(
         self,
         message_id: str,
         user_id_type: str,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
     ):
-        params: Dict[str, Any] = {"user_id_type": user_id_type}
+        params: dict[str, Any] = {"user_id_type": user_id_type}
         if page_size:
             params.update({"page_size": page_size})
 
         if page_token:
             params.update({"page_token": page_token})
 
         return await self.call_api(
             f"im/v1/messages/{message_id}/read_users", method="GET", params=params
         )
 
     async def merge_forward_msg(
         self,
         receive_id_type: str,
         receive_id: str,
-        message_id_list: List[str],
+        message_id_list: list[str],
         uuid: Optional[str] = None,
     ):
         params = {"receive_id_type": receive_id_type}
         if uuid:
             params.update({"uuid": uuid})
 
         return await self.call_api(
```

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/config.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import Optional
 
 from pydantic import Field, HttpUrl, BaseModel
 
 
 class BotConfig(BaseModel):
     """
     飞书适配器机器人配置类
@@ -35,8 +35,8 @@
       - ``feishu_lark_api_base``: 飞书海外版（lark）开放平台 API Endpoint
       - ``feishu_bots``: 飞书适配器 Bot 配置列表，具体配置项参阅 BotConfig 类
 
     """
 
     feishu_api_base: HttpUrl = Field("https://open.feishu.cn")
     feishu_lark_api_base: HttpUrl = Field("https://open.larksuite.com")
-    feishu_bots: List[BotConfig] = Field(default_factory=list)
+    feishu_bots: list[BotConfig] = Field(default_factory=list)
```

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/event.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import deepcopy
 from datetime import datetime
 from typing_extensions import override
-from typing import TYPE_CHECKING, Any, Dict, Literal, Optional
+from typing import TYPE_CHECKING, Any, Literal, Optional
 
 from pydantic import Field
 from nonebot.utils import escape_tag
 from nonebot.compat import model_dump
 
 from nonebot.adapters import Event as BaseEvent
 
@@ -199,15 +199,15 @@
 
 class PrivateMessageEvent(MessageEvent):
     __event__ = "im.message.receive_v1.p2p"
     event: PrivateMessageEventDetail
 
 
 class NoticeEvent(Event):
-    event: Dict[str, Any]
+    event: dict[str, Any]
 
     @override
     def get_type(self) -> Literal["notice"]:
         return "notice"
 
     @override
     def get_event_name(self) -> str:
```

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/exception.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/message.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,28 @@
 import re
 import json
 from dataclasses import dataclass
+from collections.abc import Iterable
 from typing_extensions import override
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    List,
-    Type,
-    Tuple,
-    Union,
-    Literal,
-    Iterable,
-    Optional,
-    TypedDict,
-)
+from typing import TYPE_CHECKING, Any, Union, Literal, Optional, TypedDict
 
 from nonebot.adapters import Message as BaseMessage
 from nonebot.adapters import MessageSegment as BaseMessageSegment
 
 from .models import Mention
 
 
 class MessageSegment(BaseMessageSegment["Message"]):
     """
     飞书 协议 MessageSegment 适配。具体方法参考协议消息段类型或源码。
     """
 
     @classmethod
     @override
-    def get_message_class(cls) -> Type["Message"]:
+    def get_message_class(cls) -> type["Message"]:
         return Message
 
     @override
     def is_text(self) -> bool:
         return self.type == "text" or self.type == "post"
 
     @override
@@ -64,27 +53,27 @@
         return Text("text", {"text": str(text)})
 
     @staticmethod
     def at(user_id: str):
         return At("at", {"user_id": user_id})
 
     @staticmethod
-    def post(title: str, content: List[List[Dict[str, Any]]]) -> "Post":
+    def post(title: str, content: list[list[dict[str, Any]]]) -> "Post":
         return Post("post", data={"title": title, "content": content})
 
     @staticmethod
     def image(image_key: str) -> "Image":
         return Image("image", {"image_key": image_key})
 
     @staticmethod
     def interactive(
         header: "InteractiveHeader",
         config: "InteractiveConfig",
-        elements: Optional[List[Dict[str, Any]]] = None,
-        i18n_elements: Optional[List[Dict[str, Any]]] = None,
+        elements: Optional[list[dict[str, Any]]] = None,
+        i18n_elements: Optional[list[dict[str, Any]]] = None,
     ):
         elements_key = "elements" if elements else "i18n_elements"
         elements_value = elements or i18n_elements
 
         return Interactive(
             "interactive",
             {
@@ -92,15 +81,15 @@
                 elements_key: elements_value,
                 "config": config,
             },
         )
 
     @staticmethod
     def interactive_template(
-        template_id: str, template_variable: Dict[str, Any]
+        template_id: str, template_variable: dict[str, Any]
     ) -> "InteractiveTemplate":
         return InteractiveTemplate(
             "interactive",
             {
                 "template_id": template_id,
                 "template_variable": template_variable,
             },
@@ -113,15 +102,15 @@
         )
 
     @staticmethod
     def hongbao(text: str) -> "Hongbao":
         return Hongbao("hongbao", {"text": text})
 
     @staticmethod
-    def system(template: str, from_user: List[str], to_chatters: List[str]) -> "System":
+    def system(template: str, from_user: list[str], to_chatters: list[str]) -> "System":
         return System(
             "system",
             {"template": template, "from_user": from_user, "to_chatters": to_chatters},
         )
 
     @staticmethod
     def location(name: str, longitude: str, latitude: str) -> "Location":
@@ -224,46 +213,46 @@
     def __str__(self) -> str:
         return f"[image:{self.data['image_key']!r}]"
 
 
 class InteractiveHeaderTitle(TypedDict):
     tag: Literal["plain_text"]
     content: Optional[str]
-    i18n: Optional[Dict[str, str]]
+    i18n: Optional[dict[str, str]]
     template: Optional[str]
 
 
 class InteractiveHeader(TypedDict):
     title: InteractiveHeaderTitle
 
 
 class InteractiveConfig(TypedDict):
     enable_forward: Optional[bool]
     update_multi: Optional[bool]
 
 
 class _InteractiveData(TypedDict):
     header: InteractiveHeader
-    elements: Optional[List[Dict[str, Any]]]
-    i18n_elements: Optional[List[Dict[str, Any]]]
+    elements: Optional[list[dict[str, Any]]]
+    i18n_elements: Optional[list[dict[str, Any]]]
     config: InteractiveConfig
 
 
 class Interactive(MessageSegment):
     if TYPE_CHECKING:
         data: _InteractiveData
 
     @override
     def __str__(self) -> str:
         return f"[interactive:{self.data!r}]"
 
 
 class _InteractiveTemplateData(TypedDict):
     template_id: str
-    template_variable: Dict[str, Any]
+    template_variable: dict[str, Any]
 
 
 @dataclass
 class InteractiveTemplate(MessageSegment):
     if TYPE_CHECKING:
         data: _InteractiveTemplateData
 
@@ -377,15 +366,15 @@
 
 
 class PostMessageNode(TypedDict):
     tag: str
 
 
 class PostMessageNodeStylable(TypedDict):
-    style: Optional[List[Literal["bold", "underline", "lineThrough", "italic"]]]
+    style: Optional[list[Literal["bold", "underline", "lineThrough", "italic"]]]
 
 
 class PostText(PostMessageNode, PostMessageNodeStylable):
     text: str
     un_escape: Optional[bool]
 
 
@@ -410,15 +399,15 @@
 
 class PostEmotion(PostMessageNode):
     emoji_type: str
 
 
 class _PostData(TypedDict):
     title: str
-    content: List[List[Dict[str, Any]]]
+    content: list[list[dict[str, Any]]]
 
 
 @dataclass
 class Post(MessageSegment):
     if TYPE_CHECKING:
         data: _PostData
 
@@ -454,16 +443,16 @@
         content_string = content_string.strip()
 
         return content_string
 
 
 class _SystemData(TypedDict):
     template: str
-    from_user: List[str]
-    to_chatters: List[str]
+    from_user: list[str]
+    to_chatters: list[str]
 
 
 @dataclass
 class System(MessageSegment):
     if TYPE_CHECKING:
         data: _SystemData
 
@@ -517,15 +506,15 @@
     @override
     def __str__(self) -> str:
         return f"[todo:{self.data!r}]"
 
 
 class _VoteData(TypedDict):
     topic: str
-    options: List[str]
+    options: list[str]
 
 
 @dataclass
 class Vote(MessageSegment):
     if TYPE_CHECKING:
         data: _VoteData
 
@@ -585,15 +574,15 @@
 class Message(BaseMessage[MessageSegment]):
     """
     飞书 协议 Message 适配。
     """
 
     @classmethod
     @override
-    def get_segment_class(cls) -> Type[MessageSegment]:
+    def get_segment_class(cls) -> type[MessageSegment]:
         return MessageSegment
 
     @override
     def __add__(
         self, other: Union[str, "MessageSegment", Iterable["MessageSegment"]]
     ) -> "Message":
         return super().__add__(
@@ -609,15 +598,15 @@
         )
 
     @staticmethod
     @override
     def _construct(msg: str) -> Iterable[MessageSegment]:
         yield Text("text", {"text": msg})
 
-    def serialize(self) -> Tuple[str, str]:
+    def serialize(self) -> tuple[str, str]:
         combined = {"zh_cn": {"title": "", "content": [[]]}}
 
         if len(self) >= 2:
             for seg in self:
                 if isinstance(seg, Post):
                     combined["zh_cn"]["title"] = seg.data["title"]
                     combined["zh_cn"]["content"] = [
@@ -639,15 +628,15 @@
 
             return self[0].type, json.dumps(self[0].data, ensure_ascii=False)
         else:
             raise ValueError("Cannot serialize empty message")
 
     @staticmethod
     def deserialize(
-        content: str, mentions: Optional[List[Mention]], message_type: str
+        content: str, mentions: Optional[list[Mention]], message_type: str
     ) -> "Message":
         msg = Message()
         parsed_content = json.loads(content)
         at_key_to_id = {
             # wipeout @ at the start of key
             mention.key[1:]: mention.id.open_id
             for mention in (mentions or [])
@@ -690,13 +679,13 @@
             else:
                 msg.append(MessageSegment(message_type, parsed_content))
 
         return msg
 
     @override
     def extract_plain_text(self) -> str:
-        text_list: List[str] = []
+        text_list: list[str] = []
         for seg in self:
             if seg.is_text():
                 text_list.append(str(seg))
 
         return "".join(text_list)
```

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/api.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 from pydantic import HttpUrl, BaseModel
 
 from .common import Reply
 
 
 class BaseResponse(BaseModel):
     code: int
@@ -15,24 +13,24 @@
     expire: int
 
 
 class BotInfo(BaseModel):
     activate_status: int
     app_name: str
     avatar_url: HttpUrl
-    ip_white_list: List[str]
+    ip_white_list: list[str]
     open_id: str
 
 
 class BotInfoResponse(BaseResponse):
     bot: BotInfo
 
 
 class ReplyResponseItems(BaseModel):
-    items: List[Reply]
+    items: list[Reply]
 
 
 class ReplyResponse(BaseResponse):
     data: ReplyResponseItems
 
 
 __all__ = [
```

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/models/common.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/models/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import List, Literal, Optional
+from typing import Literal, Optional
 
 from pydantic import BaseModel
 from nonebot.compat import PYDANTIC_V2, ConfigDict
 
 
 class EventHeader(BaseModel):
     event_id: str
     event_type: str
     create_time: str
     token: str
     app_id: str
     tenant_key: str
     resource_id: Optional[str] = None
-    user_list: Optional[List[dict]] = None
+    user_list: Optional[list[dict]] = None
 
     if PYDANTIC_V2:
         model_config = ConfigDict(extra="allow")
     else:
 
         class Config(ConfigDict):
             extra = "allow"
@@ -116,15 +116,15 @@
     create_time: str
     update_time: str
     deleted: bool
     updated: bool
     chat_id: str
     sender: ReplySender
     body: MessageBody
-    mentions: List[ReplyMention]
+    mentions: list[ReplyMention]
     upper_message_id: Optional[str] = None
 
     if PYDANTIC_V2:
         model_config = ConfigDict(extra="allow")
     else:
 
         class Config(ConfigDict):
@@ -136,15 +136,15 @@
     root_id: Optional[str] = None
     parent_id: Optional[str] = None
     create_time: str
     chat_id: str
     chat_type: str
     message_type: str
     content: str
-    mentions: Optional[List[Mention]] = None
+    mentions: Optional[list[Mention]] = None
 
     if PYDANTIC_V2:
         model_config = ConfigDict(extra="allow")
     else:
 
         class Config(ConfigDict):
             extra = "allow"
@@ -188,15 +188,15 @@
     employee_id: str
     employee_no: str
     is_field: bool
     is_wifi: bool
     latitude: float
     location_name: str
     longitude: float
-    photo_urls: Optional[List[str]] = None
+    photo_urls: Optional[list[str]] = None
     record_id: str
     ssid: str
     type: int
 
 
 class AttendanceUserTaskStatusDiff(BaseModel):
     before_status: str
@@ -209,15 +209,15 @@
 
 class AttendanceUserTaskUpdatedEventDetail(BaseModel):
     date: int
     employee_id: str
     employee_no: str
     group_id: str
     shift_id: str
-    status_changes: List[AttendanceUserTaskStatusDiff]
+    status_changes: list[AttendanceUserTaskStatusDiff]
     task_id: str
     time_zone: str
 
 
 class VCMeetingStartedEventDetail(BaseModel):
     meeting: Meeting
     operator: MeetingUser
@@ -242,16 +242,16 @@
     room_id: str
     room_name: str
 
 
 class DriveFileEditedEventDetail(BaseModel):
     file_token: str
     file_type: str
-    operator_id_list: List[UserId]
-    subscriber_id_list: List[UserId]
+    operator_id_list: list[UserId]
+    subscriber_id_list: list[UserId]
 
 
 class DriveFileDeletedEventDetail(BaseModel):
     file_token: str
     file_type: str
     operator_id: UserId
 
@@ -259,39 +259,39 @@
 class DriveFileTrashedEventDetail(BaseModel):
     file_token: str
     file_type: str
     operator_id: UserId
 
 
 class DriveFilePermissionMemberRemovedEventDetail(BaseModel):
-    chat_list: List[str]
+    chat_list: list[str]
     file_token: str
     file_type: str
     operator_id: UserId
-    user_list: List[UserId]
+    user_list: list[UserId]
 
 
 class DriveFilePermissionMemberAddedEventDetail(BaseModel):
-    chat_list: List[str]
+    chat_list: list[str]
     file_token: str
     file_type: str
     operator_id: UserId
-    user_list: List[UserId]
+    user_list: list[UserId]
 
 
 class DriveFileTitleUpdatedEventDetail(BaseModel):
     file_token: str
     file_type: str
     operator_id: UserId
 
 
 class DriveFileReadEventDetail(BaseModel):
     file_token: str
     file_type: str
-    operator_id_list: List[UserId]
+    operator_id_list: list[UserId]
 
 
 class CalendarEventChangedEventDetail(BaseModel):
     calendar_id: str
 
 
 class CalendarAclScope(BaseModel):
@@ -382,28 +382,28 @@
     name: str
     en_name: str
     email: str
     mobile: str
     gender: int
     avatar: AvatarInfo
     status: UserStatus
-    department_ids: Optional[List[str]] = None
+    department_ids: Optional[list[str]] = None
     leader_user_id: str
     city: str
     country: str
     work_station: str
     join_time: int
     employee_no: str
     employee_type: int
-    orders: Optional[List[UserOrder]] = None
-    custom_attrs: List[UserCustomAttr]
+    orders: Optional[list[UserOrder]] = None
+    custom_attrs: list[UserCustomAttr]
 
 
 class OldContactUser(BaseModel):
-    department_ids: List[str]
+    department_ids: list[str]
     open_id: str
 
 
 class ContactUserCreatedEventDetail(BaseModel):
     object: ContactUser
 
 
@@ -424,31 +424,31 @@
 
 
 class GroupMemberUserDeletedEventDetail(BaseModel):
     chat_id: str
     operator_id: UserId
     external: bool
     operator_tenant_key: str
-    users: List[ChatMemberUser]
+    users: list[ChatMemberUser]
 
 
 class GroupMemberUserWithdrawnEventDetail(BaseModel):
     chat_id: str
     operator_id: UserId
     external: bool
     operator_tenant_key: str
-    users: List[ChatMemberUser]
+    users: list[ChatMemberUser]
 
 
 class GroupMemberUserAddedEventDetail(BaseModel):
     chat_id: str
     operator_id: UserId
     external: bool
     operator_tenant_key: str
-    users: List[ChatMemberUser]
+    users: list[ChatMemberUser]
 
 
 class GroupMemberBotDeletedEventDetail(BaseModel):
     chat_id: str
     operator_id: UserId
     external: bool
     operator_tenant_key: str
@@ -534,15 +534,15 @@
     reader_id: UserId
     read_time: str
     tenant_key: str
 
 
 class MessageReadEventDetail(BaseModel):
     reader: MessageReader
-    message_id_list: List[str]
+    message_id_list: list[str]
 
 
 __all__ = [
     "EventHeader",
     "UserId",
     "MeetingUser",
     "Meeting",
```

### Comparing `nonebot_adapter_feishu-2.5.0/nonebot/adapters/feishu/utils.py` & `nonebot_adapter_feishu-2.6.0/nonebot/adapters/feishu/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_feishu-2.5.0/pyproject.toml` & `nonebot_adapter_feishu-2.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-feishu"
-version = "2.5.0"
+version = "2.6.0"
 description = "feishu(larksuite) adapter for nonebot2"
 authors = ["StarHeartHunt <starheart233@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://feishu.adapters.nonebot.dev/"
 repository = "https://github.com/nonebot/adapter-feishu"
 documentation = "https://feishu.adapters.nonebot.dev/"
@@ -15,46 +15,46 @@
   "Framework :: Robot Framework :: Library",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
 ]
 packages = [{ include = "nonebot" }]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 nonebot2 = "^2.2.0"
 cashews = "^7.0.0"
 pycryptodome = ">=3.18.0, <4.0.0"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.3.0"
+ruff = "^0.4.0"
 isort = "^5.10.1"
 black = "^24.0.0"
 nonemoji = "^0.1.2"
 pre-commit = "^3.2.0"
 nonebot2 = { git = "https://github.com/nonebot/nonebot2.git", branch = "master", extras = [
   "fastapi",
   "httpx",
 ] }
 
 [tool.poetry.group.test.dependencies]
 nonebug = "^0.3.0"
 wsproto = "^1.2.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.23.0"
 werkzeug = ">=2.3.6,<4.0.0"
 
 [tool.poetry.group.docs.dependencies]
 nb-autodoc = { git = "https://github.com/nonebot/nb-autodoc.git" }
 
 [tool.pytest.ini_options]
 addopts = "--cov=nonebot/adapters/feishu --cov-report term-missing"
 
 [tool.black]
 line-length = 88
-target-version = ["py38", "py39", "py310", "py311"]
+target-version = ["py39", "py310", "py311", "py312"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
 
 [tool.isort]
 profile = "black"
 line_length = 88
@@ -62,26 +62,26 @@
 skip_gitignore = true
 force_sort_within_sections = true
 src_paths = ["nonebot", "tests"]
 extra_standard_library = ["typing_extensions"]
 
 [tool.ruff]
 line-length = 88
-target-version = "py38"
+target-version = "py39"
 
 [tool.ruff.lint]
 select = ["E", "W", "F", "UP", "C", "T", "PYI", "PT", "Q"]
 ignore = ["E402", "C901", "UP037", "PYI021"]
 
 [tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 
 [tool.pyright]
-pythonVersion = "3.8"
+pythonVersion = "3.9"
 pythonPlatform = "All"
 defineConstant = { PYDANTIC_V2 = true }
 executionEnvironments = [
   { root = "./tests", extraPaths = [
     "./",
   ] },
   { root = "./" },
```

### Comparing `nonebot_adapter_feishu-2.5.0/PKG-INFO` & `nonebot_adapter_feishu-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-feishu
-Version: 2.5.0
+Version: 2.6.0
 Summary: feishu(larksuite) adapter for nonebot2
 Home-page: https://feishu.adapters.nonebot.dev/
 License: MIT
 Keywords: bot,feishu,larksuite
 Author: StarHeartHunt
 Author-email: starheart233@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cashews (>=7.0.0,<8.0.0)
 Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
@@ -46,15 +45,15 @@
 <p align="center">
   <a href="https://raw.githubusercontent.com/nonebot/adapter-feishu/master/LICENSE">
     <img src="https://img.shields.io/github/license/nonebot/adapter-feishu" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-adapter-feishu">
     <img src="https://img.shields.io/pypi/v/nonebot-adapter-feishu" alt="pypi">
   </a>
-  <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python">
+  <img src="https://img.shields.io/badge/python-3.9+-blue" alt="python">
   <a href="https://codecov.io/gh/nonebot/adapter-feishu">
     <img src="https://codecov.io/gh/nonebot/adapter-feishu/branch/master/graph/badge.svg?token=45OH1IVM9C"/>
   </a>
   <a href="https://github.com/nonebot/adapter-feishu/actions/workflows/website-deploy.yml">
     <img src="https://github.com/nonebot/adapter-feishu/actions/workflows/website-deploy.yml/badge.svg?branch=master&event=push" alt="site"/>
   </a>
   <a href="https://results.pre-commit.ci/latest/github/nonebot/adapter-feishu/master">
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.5.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-feishu Version: 2.6.0 Summary:
 feishu(larksuite) adapter for nonebot2 Home-page: https://
 feishu.adapters.nonebot.dev/ License: MIT Keywords: bot,feishu,larksuite
 Author: StarHeartHunt Author-email: starheart233@gmail.com Requires-Python:
->=3.8,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
+>=3.9,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Framework :: Robot Framework Classifier: Framework :: Robot Framework ::
 Library Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: cashews (>=7.0.0,<8.0.0) Requires-
-Dist: nonebot2 (>=2.2.0,<3.0.0) Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
-Project-URL: Documentation, https://feishu.adapters.nonebot.dev/ Project-URL:
-Repository, https://github.com/nonebot/adapter-feishu Description-Content-Type:
-text/markdown
+:: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Requires-Dist: cashews
+(>=7.0.0,<8.0.0) Requires-Dist: nonebot2 (>=2.2.0,<3.0.0) Requires-Dist:
+pycryptodome (>=3.18.0,<4.0.0) Project-URL: Documentation, https://
+feishu.adapters.nonebot.dev/ Project-URL: Repository, https://github.com/
+nonebot/adapter-feishu Description-Content-Type: text/markdown
                            _[_n_o_n_e_b_o_t_-_a_d_a_p_t_e_r_-_f_e_i_s_h_u_]
              # NoneBot-Adapter-Feishu _â¨ é£ä¹¦åè®®éé â¨_
  _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_n_o_n_e_b_o_t_/_a_d_a_p_t_e_r_-_f_e_i_s_h_u_/_b_r_a_n_c_h_/
  _m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_4_5_O_H_1_I_V_M_9_C_]_[_s_i_t_e_]_[_h_t_t_p_s_:_/_/_r_e_s_u_l_t_s_._p_r_e_-_c_o_m_m_i_t_._c_i_/
                 _b_a_d_g_e_/_g_i_t_h_u_b_/_n_o_n_e_b_o_t_/_a_d_a_p_t_e_r_-_f_e_i_s_h_u_/_m_a_s_t_e_r_._s_v_g_]
          _[_Q_Q_ _C_h_a_t_ _G_r_o_u_p_]_[_Q_Q_ _C_h_a_n_n_e_l_]_[_T_e_l_e_g_r_a_m_ _C_h_a_n_n_e_l_]_[_D_i_s_c_o_r_d_ _S_e_r_v_e_r_]
                        _æ___æ_¡_£ Â· _å_®__è_£_ Â· _å_¼__å_§__ä_½_¿_ç__¨
```


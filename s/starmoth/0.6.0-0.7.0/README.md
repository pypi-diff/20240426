# Comparing `tmp/starmoth-0.6.0.tar.gz` & `tmp/starmoth-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmoth-0.6.0.tar", last modified: Wed Oct  4 21:37:06 2023, max compression
+gzip compressed data, was "starmoth-0.7.0.tar", last modified: Fri Apr 26 17:12:38 2024, max compression
```

## Comparing `starmoth-0.6.0.tar` & `starmoth-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 21:37:06.162110 starmoth-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     2635 2023-10-04 21:37:06.162110 starmoth-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2263 2023-10-04 21:26:33.000000 starmoth-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 21:37:06.154109 starmoth-0.6.0/moth/
--rw-rw-rw-   0 root         (0) root         (0)     4587 2023-07-20 18:39:06.000000 starmoth-0.6.0/moth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 21:37:06.158110 starmoth-0.6.0/moth/cli/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.6.0/moth/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 21:37:06.158110 starmoth-0.6.0/moth/driver/
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-30 20:12:28.000000 starmoth-0.6.0/moth/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 21:37:06.158110 starmoth-0.6.0/moth/message/
--rw-rw-rw-   0 root         (0) root         (0)     7574 2023-09-27 22:08:34.000000 starmoth-0.6.0/moth/message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.6.0/moth/message/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 21:37:06.158110 starmoth-0.6.0/moth/server/
--rw-rw-rw-   0 root         (0) root         (0)     6040 2023-06-15 20:13:10.000000 starmoth-0.6.0/moth/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-04 21:37:06.162110 starmoth-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-04 21:37:06.162110 starmoth-0.6.0/starmoth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2635 2023-10-04 21:37:06.000000 starmoth-0.6.0/starmoth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-10-04 21:37:06.000000 starmoth-0.6.0/starmoth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-04 21:37:06.000000 starmoth-0.6.0/starmoth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-04 21:37:06.000000 starmoth-0.6.0/starmoth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-10-04 21:37:06.000000 starmoth-0.6.0/starmoth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-10-04 21:37:06.000000 starmoth-0.6.0/starmoth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.998340 starmoth-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-04-26 17:12:37.998340 starmoth-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3549 2024-04-23 20:53:43.000000 starmoth-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/
+-rw-rw-rw-   0 root         (0) root         (0)     4670 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/driver/
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/message/
+-rw-rw-rw-   0 root         (0) root         (0)     9396 2024-04-26 17:11:22.000000 starmoth-0.7.0/moth/message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/message/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.994340 starmoth-0.7.0/moth/server/
+-rw-rw-rw-   0 root         (0) root         (0)     5976 2024-04-23 20:53:43.000000 starmoth-0.7.0/moth/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 17:12:37.998340 starmoth-0.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-04-23 20:53:43.000000 starmoth-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:12:37.998340 starmoth-0.7.0/starmoth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-26 17:12:37.000000 starmoth-0.7.0/starmoth.egg-info/top_level.txt
```

### Comparing `starmoth-0.6.0/PKG-INFO` & `starmoth-0.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.6.0
+Version: 0.7.0
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pyzmq>=25.0.0
@@ -20,17 +20,15 @@
 
 `moth server <folder path>`
 
 `moth client`
 
 # Client
 
-
-
-Simplest possible classification model client.
+Simple classification model client.
 ``` python
 from moth import Moth
 from moth.message import ImagePromptMsg, ClassificationResultMsg, HandshakeTaskTypes
 
 moth = Moth("my-ai", task_type=HandshakeTaskTypes.CLASSIFICATION)
 
 @moth.prompt
@@ -43,42 +41,111 @@
 
 ClassificationResultMsg can optionally include a confidence value
 
 ``` python
 ClassificationResultMsg(prompt_id=prompt.id, class_name="cat", confidence=0.9)
 ```
 
-Simplest possible object detection model client.
+Simple object detection model client.
 ``` python
 from moth import Moth
-from moth.message import ImagePromptMsg, ObjectDetectionResultMsg, ObjectDetectionResult, HandshakeTaskTypes
+from moth.message import (
+    ImagePromptMsg,
+    ObjectDetectionResultMsg,
+    ObjectDetectionResult,
+    HandshakeTaskTypes,
+)
 
 moth = Moth("my-ai", task_type=HandshakeTaskTypes.OBJECT_DETECTION)
 
+
 @moth.prompt
 def on_prompt(prompt: ImagePromptMsg):
     # TODO: Do smart AI here
     # Make a list of ObjectDetectionResults
-    l = []
-    l.append(ObjectDetectionResult(0, 0, 50, 50, class_name="cat", class_index=0, confidence=0.9))
-    l.append(ObjectDetectionResult(10, 10, 50, 35, class_name="dog", class_index=1, confidence=0.1))
-    return ObjectDetectionResultMsg(prompt_id=prompt.id, object_detection_results=l)
- 
+    results = []
+    results.append(
+        ObjectDetectionResult(
+            0,
+            0,
+            50,
+            50,
+            class_name="cat",
+            class_index=0,
+            confidence=0.9,  # Optional confidence
+        )
+    )
+    results.append(
+        ObjectDetectionResult(
+            10,
+            10,
+            50,
+            35,
+            class_name="dog",
+            class_index=1,
+            confidence=0.1,  # Optional confidence
+        )
+    )
+    return ObjectDetectionResultMsg(
+        prompt_id=prompt.id, object_detection_results=results
+    )
+
+
+moth.run()
+
+```
+
+Simple segmentation model client.
+``` python
+from moth import Moth
+from moth.message import (
+    ImagePromptMsg,
+    SegmentationResultMsg,
+    SegmentationResult,
+    HandshakeTaskTypes,
+)
+
+moth = Moth("my-ai", task_type=HandshakeTaskTypes.SEGMENTATION)
+
+
+@moth.prompt
+def on_prompt(prompt: ImagePromptMsg):
+    # TODO: Do smart AI here
+    # Make a list of ObjectDetectionResults
+    results = []
+    results.append(
+        SegmentationResult(
+            [0, 0, 50, 50, 20, 20, 0, 0],  # The predicted polygon
+            class_name="cat",
+            class_index=0,
+            confidence=0.9,  # Optional confidence
+        )
+    )
+    results.append(
+        SegmentationResult(
+            [0, 0, 50, 50, 13, 20, 0, 0],  # The predicted polygon
+            class_name="dog",
+            class_index=1,
+            confidence=0.1,  # Optional confidence
+        )
+    )
+    return SegmentationResultMsg(prompt_id=prompt.id, results=results)
+
 
 moth.run()
 ```
 
-You can also define a set of client output classes that get handed over to the server.
+You can also define a set of client output classes that get sent to the server. We recommend you do this.
 ``` python
 moth = Moth("my-ai", task_type=HandshakeTaskTypes.CLASSIFICATION, output_classes=["cat", "dog"])
 ```
 
 # Server
 
-Simplest possible server.
+Simple server.
 ``` python
 from moth.server import Server
 from moth.message import HandshakeMsg
 
 class ModelDriverImpl(ModelDriver):
     # TODO: Implement your model driver here
     pass
@@ -86,15 +153,15 @@
 server = Server(7171)
 
 @server.driver_factory
 def handle_handshake(handshake: HandshakeMsg) -> ModelDriver
     return ModelDriverImpl()
 ```
 
-You can also register to keep an up to date list of connected models.
+You can also subscribe to track changes to the current list of connected models.
 ``` python
 from moth.server import Model
 
 @server.on_model_change
 def handle_model_change(model_list: List[Model]):
     print(f"Connected models: {model_list}")
 ```
```

### Comparing `starmoth-0.6.0/README.md` & `starmoth-0.7.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 `moth server <folder path>`
 
 `moth client`
 
 # Client
 
-
-
-Simplest possible classification model client.
+Simple classification model client.
 ``` python
 from moth import Moth
 from moth.message import ImagePromptMsg, ClassificationResultMsg, HandshakeTaskTypes
 
 moth = Moth("my-ai", task_type=HandshakeTaskTypes.CLASSIFICATION)
 
 @moth.prompt
@@ -30,42 +28,111 @@
 
 ClassificationResultMsg can optionally include a confidence value
 
 ``` python
 ClassificationResultMsg(prompt_id=prompt.id, class_name="cat", confidence=0.9)
 ```
 
-Simplest possible object detection model client.
+Simple object detection model client.
 ``` python
 from moth import Moth
-from moth.message import ImagePromptMsg, ObjectDetectionResultMsg, ObjectDetectionResult, HandshakeTaskTypes
+from moth.message import (
+    ImagePromptMsg,
+    ObjectDetectionResultMsg,
+    ObjectDetectionResult,
+    HandshakeTaskTypes,
+)
 
 moth = Moth("my-ai", task_type=HandshakeTaskTypes.OBJECT_DETECTION)
 
+
 @moth.prompt
 def on_prompt(prompt: ImagePromptMsg):
     # TODO: Do smart AI here
     # Make a list of ObjectDetectionResults
-    l = []
-    l.append(ObjectDetectionResult(0, 0, 50, 50, class_name="cat", class_index=0, confidence=0.9))
-    l.append(ObjectDetectionResult(10, 10, 50, 35, class_name="dog", class_index=1, confidence=0.1))
-    return ObjectDetectionResultMsg(prompt_id=prompt.id, object_detection_results=l)
- 
+    results = []
+    results.append(
+        ObjectDetectionResult(
+            0,
+            0,
+            50,
+            50,
+            class_name="cat",
+            class_index=0,
+            confidence=0.9,  # Optional confidence
+        )
+    )
+    results.append(
+        ObjectDetectionResult(
+            10,
+            10,
+            50,
+            35,
+            class_name="dog",
+            class_index=1,
+            confidence=0.1,  # Optional confidence
+        )
+    )
+    return ObjectDetectionResultMsg(
+        prompt_id=prompt.id, object_detection_results=results
+    )
+
+
+moth.run()
+
+```
+
+Simple segmentation model client.
+``` python
+from moth import Moth
+from moth.message import (
+    ImagePromptMsg,
+    SegmentationResultMsg,
+    SegmentationResult,
+    HandshakeTaskTypes,
+)
+
+moth = Moth("my-ai", task_type=HandshakeTaskTypes.SEGMENTATION)
+
+
+@moth.prompt
+def on_prompt(prompt: ImagePromptMsg):
+    # TODO: Do smart AI here
+    # Make a list of ObjectDetectionResults
+    results = []
+    results.append(
+        SegmentationResult(
+            [0, 0, 50, 50, 20, 20, 0, 0],  # The predicted polygon
+            class_name="cat",
+            class_index=0,
+            confidence=0.9,  # Optional confidence
+        )
+    )
+    results.append(
+        SegmentationResult(
+            [0, 0, 50, 50, 13, 20, 0, 0],  # The predicted polygon
+            class_name="dog",
+            class_index=1,
+            confidence=0.1,  # Optional confidence
+        )
+    )
+    return SegmentationResultMsg(prompt_id=prompt.id, results=results)
+
 
 moth.run()
 ```
 
-You can also define a set of client output classes that get handed over to the server.
+You can also define a set of client output classes that get sent to the server. We recommend you do this.
 ``` python
 moth = Moth("my-ai", task_type=HandshakeTaskTypes.CLASSIFICATION, output_classes=["cat", "dog"])
 ```
 
 # Server
 
-Simplest possible server.
+Simple server.
 ``` python
 from moth.server import Server
 from moth.message import HandshakeMsg
 
 class ModelDriverImpl(ModelDriver):
     # TODO: Implement your model driver here
     pass
@@ -73,15 +140,15 @@
 server = Server(7171)
 
 @server.driver_factory
 def handle_handshake(handshake: HandshakeMsg) -> ModelDriver
     return ModelDriverImpl()
 ```
 
-You can also register to keep an up to date list of connected models.
+You can also subscribe to track changes to the current list of connected models.
 ``` python
 from moth.server import Model
 
 @server.on_model_change
 def handle_model_change(model_list: List[Model]):
     print(f"Connected models: {model_list}")
 ```
```

### Comparing `starmoth-0.6.0/moth/__init__.py` & `starmoth-0.7.0/moth/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,15 +39,17 @@
         context = zmq.Context()
         socket = context.socket(zmq.DEALER)
         socket.setsockopt_string(zmq.IDENTITY, self.name)
 
         try:
             socket.connect(url)
             # This is a handshake call to prove our identity
-            handshake = HandshakeMsg(self.name, self._token, "v0.0.0", self.task_type, self.output_classes)
+            handshake = HandshakeMsg(
+                self.name, self._token, "v0.0.0", self.task_type, self.output_classes
+            )
             socket.send(handshake.serialize_envelope())
             self._req_loop(socket)
         except KeyboardInterrupt:
             print("\nExit...")
             self.stop = True
 
     def prompt(self, func):
@@ -91,14 +93,15 @@
                 if events:
                     # Check if the prompt queue is empty
                     msg_bytes = socket.recv()
                     message = parse_message(msg_bytes)
 
                     if isinstance(message, ImagePromptMsg):
                         prompt_queue.put(message)
+                        last_heartbeat = time.time()
 
                     if isinstance(message, HeartbeatMsg):
                         last_heartbeat = time.time()
 
                     if isinstance(message, HandshakeResponseMsg):
                         print("Connected to server")
                         last_heartbeat = time.time()
```

### Comparing `starmoth-0.6.0/moth/cli/__init__.py` & `starmoth-0.7.0/moth/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.6.0/moth/driver/__init__.py` & `starmoth-0.7.0/moth/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.6.0/moth/message/__init__.py` & `starmoth-0.7.0/moth/message/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from moth.message.exceptions import FailedToParseMessage, UnknownMessageType
 
 
 class HandshakeTaskTypes(str, Enum):
     CLASSIFICATION = "classification"
     OBJECT_DETECTION = "object_detection"
+    SEGMENTATION = "segmentation"
 
 
 def parse_message(msg: bytes) -> Msg:
     try:
         envelope = msgpack.unpackb(msg)
         message_type = envelope["msgType"]
 
@@ -211,14 +212,77 @@
             prompt_id=obj["promptId"],
             object_detection_results=[
                 ObjectDetectionResult.deserialize(bb) for bb in obj["results"]
             ],
         )
 
 
+class SegmentationResult:
+    """
+    Segmentation in the format of [x1, y1, x2, y2, ...].
+    """
+
+    def __init__(
+        self,
+        points: List[int],
+        class_index: Optional[int] = None,
+        class_name: Optional[str] = None,
+        confidence: float = None,
+    ) -> None:
+        self.points = points
+        self.class_name = class_name
+        self.class_index = class_index
+        self.confidence = confidence
+
+    def serialize(self) -> bytes:
+        obj = {
+            "points": self.points,
+            "className": self.class_name,
+            "classIndex": self.class_index,
+            "confidence": self.confidence,
+        }
+        return msgpack.packb(obj)
+
+    @staticmethod
+    def deserialize(data: bytes) -> Msg:
+        obj = msgpack.unpackb(data)
+        return SegmentationResult(
+            points=obj["points"],
+            class_name=obj["className"],
+            class_index=obj["classIndex"],
+            confidence=obj["confidence"],
+        )
+
+
+class SegmentationResultMsg(Msg):
+    """
+    Message for segmentation results.
+    List of SegmentationResults.
+    """
+
+    def __init__(self, prompt_id: str, results: List[SegmentationResult]):
+        self.prompt_id = prompt_id
+        self.results = results
+
+    def serialize(self) -> bytes:
+        obj = {
+            "promptId": self.prompt_id,
+            "results": [r.serialize() for r in self.results],
+        }
+        return msgpack.packb(obj)
+
+    @staticmethod
+    def deserialize(data: bytes) -> Msg:
+        obj = msgpack.unpackb(data)
+        return SegmentationResultMsg(
+            prompt_id=obj["promptId"],
+            results=[SegmentationResult.deserialize(r) for r in obj["results"]],
+        )
+
+
 @dataclass
 class HandshakeMsg(Msg):
     name: str
     handshake_token: str
     version: str = "v0"
     task_type: HandshakeTaskTypes = HandshakeTaskTypes.CLASSIFICATION
     output_classes: Optional[List[str]] = None
@@ -261,14 +325,15 @@
 
 class PromptResultMsg(Msg):
     pass
 
 
 _MESSAGE_CLASSES: Dict[str, Type[Msg]] = {
     HandshakeMsg.msg_type_name(): HandshakeMsg,
-    ImagePromptMsg.msg_type_name(): ImagePromptMsg,
+    HandshakeResponseMsg.msg_type_name(): HandshakeResponseMsg,
     HeartbeatMsg.msg_type_name(): HeartbeatMsg,
+    ImagePromptMsg.msg_type_name(): ImagePromptMsg,
     PromptResultMsg.msg_type_name(): ClassificationResultMsg,  # Ensure backwards compatibility
     ClassificationResultMsg.msg_type_name(): ClassificationResultMsg,
     ObjectDetectionResultMsg.msg_type_name(): ObjectDetectionResultMsg,
-    HandshakeResponseMsg.msg_type_name(): HandshakeResponseMsg,
+    SegmentationResultMsg.msg_type_name(): SegmentationResultMsg
 }
```

### Comparing `starmoth-0.6.0/moth/server/__init__.py` & `starmoth-0.7.0/moth/server/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from typing import Callable, Dict, List, Optional
 from dataclasses import dataclass
 import time
 import zmq
 from moth.driver import ModelDriver
 from moth.message import (
     HandshakeMsg,
-    ClassificationResultMsg,
     HandshakeResponseMsg,
     HeartbeatMsg,
-    Msg,
+    ClassificationResultMsg,
     ObjectDetectionResultMsg,
+    SegmentationResultMsg,
     parse_message,
 )
 from moth.message.exceptions import MothMessageError
 
 
 @dataclass
 class Model:
@@ -94,33 +94,32 @@
                         model = Model(
                             id=identity_str,
                             task_type=message.task_type,
                             output_classes=message.output_classes,
                         )
                         self._drivers[identity] = driver
                         self._models[identity] = model
-                        self._heartbeats[identity] = time.time()
                         if self._on_model_change_handler:
                             self._on_model_change_handler(
                                 list(self._models.values())
                             )  # Pass the list of current drivers
                         print(f"MUT connected: {identity_str}")
                         # Send a handshake response
                         socket.send(identity, zmq.SNDMORE)
                         socket.send(HandshakeResponseMsg().serialize_envelope())
 
-                    if isinstance(message, ClassificationResultMsg):
-                        if identity in self._drivers:
-                            self._drivers[identity].on_model_result(message)
-
-                    if isinstance(message, ObjectDetectionResultMsg):
+                    elif (
+                        isinstance(message, ClassificationResultMsg)
+                        or isinstance(message, ObjectDetectionResultMsg)
+                        or isinstance(message, SegmentationResultMsg)
+                    ):
                         if identity in self._drivers:
                             self._drivers[identity].on_model_result(message)
 
-                    if isinstance(message, HeartbeatMsg):
+                    if identity in self._drivers:
                         self._heartbeats[identity] = time.time()
 
                 except MothMessageError as err:
                     print(err)
                 except Exception as err:
                     print(err)
```

### Comparing `starmoth-0.6.0/setup.py` & `starmoth-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `starmoth-0.6.0/starmoth.egg-info/PKG-INFO` & `starmoth-0.7.0/starmoth.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starmoth
-Version: 0.6.0
+Version: 0.7.0
 Summary: A small wrapper library to help test systems using STAR
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Fraunhofer,STAR,testing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pyzmq>=25.0.0
@@ -20,17 +20,15 @@
 
 `moth server <folder path>`
 
 `moth client`
 
 # Client
 
-
-
-Simplest possible classification model client.
+Simple classification model client.
 ``` python
 from moth import Moth
 from moth.message import ImagePromptMsg, ClassificationResultMsg, HandshakeTaskTypes
 
 moth = Moth("my-ai", task_type=HandshakeTaskTypes.CLASSIFICATION)
 
 @moth.prompt
@@ -43,42 +41,111 @@
 
 ClassificationResultMsg can optionally include a confidence value
 
 ``` python
 ClassificationResultMsg(prompt_id=prompt.id, class_name="cat", confidence=0.9)
 ```
 
-Simplest possible object detection model client.
+Simple object detection model client.
 ``` python
 from moth import Moth
-from moth.message import ImagePromptMsg, ObjectDetectionResultMsg, ObjectDetectionResult, HandshakeTaskTypes
+from moth.message import (
+    ImagePromptMsg,
+    ObjectDetectionResultMsg,
+    ObjectDetectionResult,
+    HandshakeTaskTypes,
+)
 
 moth = Moth("my-ai", task_type=HandshakeTaskTypes.OBJECT_DETECTION)
 
+
 @moth.prompt
 def on_prompt(prompt: ImagePromptMsg):
     # TODO: Do smart AI here
     # Make a list of ObjectDetectionResults
-    l = []
-    l.append(ObjectDetectionResult(0, 0, 50, 50, class_name="cat", class_index=0, confidence=0.9))
-    l.append(ObjectDetectionResult(10, 10, 50, 35, class_name="dog", class_index=1, confidence=0.1))
-    return ObjectDetectionResultMsg(prompt_id=prompt.id, object_detection_results=l)
- 
+    results = []
+    results.append(
+        ObjectDetectionResult(
+            0,
+            0,
+            50,
+            50,
+            class_name="cat",
+            class_index=0,
+            confidence=0.9,  # Optional confidence
+        )
+    )
+    results.append(
+        ObjectDetectionResult(
+            10,
+            10,
+            50,
+            35,
+            class_name="dog",
+            class_index=1,
+            confidence=0.1,  # Optional confidence
+        )
+    )
+    return ObjectDetectionResultMsg(
+        prompt_id=prompt.id, object_detection_results=results
+    )
+
+
+moth.run()
+
+```
+
+Simple segmentation model client.
+``` python
+from moth import Moth
+from moth.message import (
+    ImagePromptMsg,
+    SegmentationResultMsg,
+    SegmentationResult,
+    HandshakeTaskTypes,
+)
+
+moth = Moth("my-ai", task_type=HandshakeTaskTypes.SEGMENTATION)
+
+
+@moth.prompt
+def on_prompt(prompt: ImagePromptMsg):
+    # TODO: Do smart AI here
+    # Make a list of ObjectDetectionResults
+    results = []
+    results.append(
+        SegmentationResult(
+            [0, 0, 50, 50, 20, 20, 0, 0],  # The predicted polygon
+            class_name="cat",
+            class_index=0,
+            confidence=0.9,  # Optional confidence
+        )
+    )
+    results.append(
+        SegmentationResult(
+            [0, 0, 50, 50, 13, 20, 0, 0],  # The predicted polygon
+            class_name="dog",
+            class_index=1,
+            confidence=0.1,  # Optional confidence
+        )
+    )
+    return SegmentationResultMsg(prompt_id=prompt.id, results=results)
+
 
 moth.run()
 ```
 
-You can also define a set of client output classes that get handed over to the server.
+You can also define a set of client output classes that get sent to the server. We recommend you do this.
 ``` python
 moth = Moth("my-ai", task_type=HandshakeTaskTypes.CLASSIFICATION, output_classes=["cat", "dog"])
 ```
 
 # Server
 
-Simplest possible server.
+Simple server.
 ``` python
 from moth.server import Server
 from moth.message import HandshakeMsg
 
 class ModelDriverImpl(ModelDriver):
     # TODO: Implement your model driver here
     pass
@@ -86,15 +153,15 @@
 server = Server(7171)
 
 @server.driver_factory
 def handle_handshake(handshake: HandshakeMsg) -> ModelDriver
     return ModelDriverImpl()
 ```
 
-You can also register to keep an up to date list of connected models.
+You can also subscribe to track changes to the current list of connected models.
 ``` python
 from moth.server import Model
 
 @server.on_model_change
 def handle_model_change(model_list: List[Model]):
     print(f"Connected models: {model_list}")
 ```
```


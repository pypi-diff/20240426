# Comparing `tmp/yolonnx-0.1.2.tar.gz` & `tmp/yolonnx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolonnx-0.1.2.tar", last modified: Thu Apr 25 11:27:33 2024, max compression
+gzip compressed data, was "yolonnx-0.1.3.tar", last modified: Thu Apr 25 13:49:55 2024, max compression
```

## Comparing `yolonnx-0.1.2.tar` & `yolonnx-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1099 2024-04-19 12:11:03.505690 yolonnx-0.1.2/LICENSE
--rw-r--r--   0        0        0     1282 2024-04-22 14:07:07.942295 yolonnx-0.1.2/README.md
--rw-r--r--   0        0        0      664 2024-04-25 11:27:33.072537 yolonnx-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 12:05:13.818667 yolonnx-0.1.2/src/yolonnx/__init__.py
--rw-r--r--   0        0        0      428 2024-04-23 07:40:59.649339 yolonnx-0.1.2/src/yolonnx/model.py
--rw-r--r--   0        0        0     1377 2024-04-22 13:45:27.021530 yolonnx-0.1.2/src/yolonnx/protocols.py
--rw-r--r--   0        0        0      108 2024-04-22 12:06:52.774186 yolonnx-0.1.2/src/yolonnx/services/__init__.py
--rw-r--r--   0        0        0     2327 2024-04-25 11:25:19.964794 yolonnx-0.1.2/src/yolonnx/services/classifier.py
--rw-r--r--   0        0        0     2988 2024-04-23 07:39:11.587139 yolonnx-0.1.2/src/yolonnx/services/detector.py
--rw-r--r--   0        0        0     1364 2024-04-22 13:50:09.339584 yolonnx-0.1.2/src/yolonnx/to_tensor_strategies.py
--rw-r--r--   0        0        0     1569 2024-04-22 12:31:23.751245 yolonnx-0.1.2/src/yolonnx/utils.py
--rw-r--r--   0        0        0        0 2024-04-23 08:14:27.133123 yolonnx-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 yolonnx-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-19 12:11:03.505690 yolonnx-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1282 2024-04-22 14:07:07.942295 yolonnx-0.1.3/README.md
+-rw-r--r--   0        0        0      664 2024-04-25 13:49:55.887157 yolonnx-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-22 12:05:13.818667 yolonnx-0.1.3/src/yolonnx/__init__.py
+-rw-r--r--   0        0        0      428 2024-04-23 07:40:59.649339 yolonnx-0.1.3/src/yolonnx/model.py
+-rw-r--r--   0        0        0     1377 2024-04-22 13:45:27.021530 yolonnx-0.1.3/src/yolonnx/protocols.py
+-rw-r--r--   0        0        0      108 2024-04-22 12:06:52.774186 yolonnx-0.1.3/src/yolonnx/services/__init__.py
+-rw-r--r--   0        0        0     4256 2024-04-25 13:49:05.634010 yolonnx-0.1.3/src/yolonnx/services/classifier.py
+-rw-r--r--   0        0        0     2988 2024-04-23 07:39:11.587139 yolonnx-0.1.3/src/yolonnx/services/detector.py
+-rw-r--r--   0        0        0     1364 2024-04-22 13:50:09.339584 yolonnx-0.1.3/src/yolonnx/to_tensor_strategies.py
+-rw-r--r--   0        0        0     1569 2024-04-22 12:31:23.751245 yolonnx-0.1.3/src/yolonnx/utils.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:14:27.133123 yolonnx-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 yolonnx-0.1.3/PKG-INFO
```

### Comparing `yolonnx-0.1.2/LICENSE` & `yolonnx-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.2/README.md` & `yolonnx-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.2/pyproject.toml` & `yolonnx-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yolonnx"
-version = "0.1.2"
+version = "0.1.3"
 description = "You Only Look ONNX"
 authors = [
     { name = "Kasper Fromm Pedersen", email = "kasperf@cs.aau.dk" },
 ]
 dependencies = [
     "numpy==1.26.*",
     "aau-label==0.2.*",
```

### Comparing `yolonnx-0.1.2/src/yolonnx/protocols.py` & `yolonnx-0.1.3/src/yolonnx/protocols.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.2/src/yolonnx/services/classifier.py` & `yolonnx-0.1.3/src/yolonnx/services/detector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,94 @@
 import ast
 import logging
-from typing import Generic, Sequence, TypeVar
+from typing import Generic, Sequence, TypeVar, cast
 
 import numpy
-from numpy import float32
 from numpy.typing import NDArray
 
-from ..model import ClassifierResult
-from ..protocols import (
-    InferenceSessionProtocol,
-    SparseTensorProtocol,
-    ToTensorStrategyProtocol,
-)
+from .. import utils
+from ..model import DetectorResult, ImgTensor
+from ..protocols import InferenceSessionProtocol, ToTensorStrategyProtocol
 
 T = TypeVar("T")
 logger = logging.getLogger(__name__)
 
 
-class Classifier(Generic[T]):
+class Detector(Generic[T]):
     def __init__(
         self,
         session: InferenceSessionProtocol,
         to_tensor_strategy: ToTensorStrategyProtocol[T],
-        none_cls_name: str = "none",
-        threshold: float = 0.1,
+        conf_threshold: float = 0.25,
+        iou_threshold: float = 0.7,
     ) -> None:
         self.__session = session
         self.__to_tensor_strategy = to_tensor_strategy
-        self.__non_cls_name = none_cls_name
-        self.__threshold = threshold
+        self.__conf_threshold = conf_threshold
+        self.__iou_threshold = iou_threshold
+
         meta = self.__session.get_modelmeta()
         self.__names: dict[int, str] = ast.literal_eval(
             meta.custom_metadata_map["names"]
         )
 
     @property
-    def threshold(self) -> float:
-        return self.__threshold
+    def conf_threshold(self) -> float:
+        return self.__conf_threshold
+
+    @property
+    def iou_threshold(self) -> float:
+        return self.__iou_threshold
 
     @property
     def shape(self) -> tuple[int, int]:
         return self.__session.get_inputs()[0].shape[2:]
 
     @property
     def names(self) -> dict[int, str]:
         return self.__names
 
-    def warmup(self) -> None:
-        tensor = numpy.zeros((1, 3, self.shape[0], self.shape[1]), float32)
-        self.__session.run(None, {"images": tensor})
-
-    def __result_handler(self, results: NDArray) -> Sequence[ClassifierResult]:
-        labels_idx = numpy.argwhere(results > self.threshold)
-        scores: NDArray[float32] = results[labels_idx]
-
-        rv: list[ClassifierResult] = []
-        for i in range(len(labels_idx)):
-            id = labels_idx[i][0]
-            label_name = self.names[id]
-            if label_name != self.__non_cls_name:
-                rv.append(ClassifierResult(name=label_name, score=scores[i][0]))
+    def __result_handler(
+        self, results: NDArray, tensor: ImgTensor
+    ) -> Sequence[DetectorResult]:
+        predictions = numpy.squeeze(results[0]).T
+
+        scores = numpy.max(predictions[:, 4:], axis=1)
+        keep = scores > self.__conf_threshold
+        predictions = predictions[keep, :]
+        scores = scores[keep]
+        class_ids = numpy.argmax(predictions[:, 4:], axis=1)
+
+        boxes = predictions[:, :4]
+        # Make x0, y0 left upper corner instead of box center
+        boxes[:, 0:2] -= boxes[:, 2:4] / 2
+        boxes /= numpy.array(
+            [
+                tensor.scale.width,
+                tensor.scale.height,
+                tensor.scale.width,
+                tensor.scale.height,
+            ],
+            dtype=numpy.float32,
+        )
+        boxes = boxes.astype(numpy.int32)
+
+        keep = utils.nms(boxes, scores, self.__iou_threshold)
+        rv = []
+        for bbox, label, score in zip(boxes[keep], class_ids[keep], scores[keep]):
+            rv.append(
+                DetectorResult(
+                    x=bbox[0].item(),
+                    y=bbox[1].item(),
+                    width=bbox[2].item(),
+                    height=bbox[3].item(),
+                    name=self.__names[label],
+                    score=score.item(),
+                )
+            )
 
-        rv.sort(key=lambda x: x.score, reverse=True)
         return rv
 
-    def run(self, img: T) -> Sequence[ClassifierResult]:
+    def run(self, img: T) -> Sequence[DetectorResult]:
         tensor = self.__to_tensor_strategy(img, *self.shape)
-        results = self.__session.run(None, {"images": tensor.data})[0]
-
-        if isinstance(results, SparseTensorProtocol):
-            results = results.values()
-
-        return self.__result_handler(results[0])
+        results = cast(list[NDArray], self.__session.run(None, {"images": tensor.data}))
+        return self.__result_handler(results[0], tensor)
```

### Comparing `yolonnx-0.1.2/src/yolonnx/to_tensor_strategies.py` & `yolonnx-0.1.3/src/yolonnx/to_tensor_strategies.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.2/src/yolonnx/utils.py` & `yolonnx-0.1.3/src/yolonnx/utils.py`

 * *Files identical despite different names*

### Comparing `yolonnx-0.1.2/PKG-INFO` & `yolonnx-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolonnx
-Version: 0.1.2
+Version: 0.1.3
 Summary: You Only Look ONNX
 Keywords: ONNX,YOLOv8,onnxruntime,vision
 Home-page: https://www.cs.aau.dk/
 Author-Email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>
 License: MIT
 Project-URL: Homepage, https://www.cs.aau.dk/
 Project-URL: Repository, https://github.com/fromm1990/yolonnx
```


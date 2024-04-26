# Comparing `tmp/big_thing_py-0.4.1.5.post9.tar.gz` & `tmp/big_thing_py-0.4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "big_thing_py-0.4.1.5.post9.tar", max compression
+gzip compressed data, was "big_thing_py-0.4.2.0.tar", max compression
```

## Comparing `big_thing_py-0.4.1.5.post9.tar` & `big_thing_py-0.4.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     2831 2023-10-10 07:27:03.817050 big_thing_py-0.4.1.5.post9/README.md
--rw-r--r--   0        0        0       24 2023-12-04 00:55:39.761445 big_thing_py-0.4.1.5.post9/big_thing_py/__init__.py
--rw-r--r--   0        0        0    44361 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/big_thing.py
--rw-r--r--   0        0        0       87 2023-08-18 08:26:19.744139 big_thing_py-0.4.1.5.post9/big_thing_py/common/__init__.py
--rw-r--r--   0        0        0     1225 2023-08-30 07:44:46.657974 big_thing_py-0.4.1.5.post9/big_thing_py/common/common.py
--rw-r--r--   0        0        0     2980 2023-08-18 08:26:19.744139 big_thing_py-0.4.1.5.post9/big_thing_py/common/error.py
--rw-r--r--   0        0        0    28266 2023-12-04 00:55:42.593420 big_thing_py-0.4.1.5.post9/big_thing_py/common/mxtype.py
--rw-r--r--   0        0        0     2045 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/common/thread.py
--rw-r--r--   0        0        0      132 2023-04-05 05:16:38.306626 big_thing_py-0.4.1.5.post9/big_thing_py/core/__init__.py
--rw-r--r--   0        0        0     1705 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/core/argument.py
--rw-r--r--   0        0        0    12947 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/core/function.py
--rw-r--r--   0        0        0     9217 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/core/mqtt_message.py
--rw-r--r--   0        0        0     1687 2023-08-30 07:44:46.657974 big_thing_py-0.4.1.5.post9/big_thing_py/core/request.py
--rw-r--r--   0        0        0     5224 2023-10-10 07:27:03.817050 big_thing_py-0.4.1.5.post9/big_thing_py/core/service.py
--rw-r--r--   0        0        0     1308 2023-11-24 02:16:14.531097 big_thing_py-0.4.1.5.post9/big_thing_py/core/tag.py
--rw-r--r--   0        0        0     9989 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/core/thing.py
--rw-r--r--   0        0        0     5873 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/core/value.py
--rw-r--r--   0        0        0       59 2023-04-02 12:40:49.707991 big_thing_py-0.4.1.5.post9/big_thing_py/manager/__init__.py
--rw-r--r--   0        0        0      747 2023-10-10 07:27:03.817050 big_thing_py-0.4.1.5.post9/big_thing_py/manager/manager_common.py
--rw-r--r--   0        0        0     3624 2023-08-30 07:44:46.657974 big_thing_py-0.4.1.5.post9/big_thing_py/manager/manager_utils.py
--rw-r--r--   0        0        0    21427 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/poll_manager_thing.py
--rw-r--r--   0        0        0     2051 2023-10-10 07:27:03.817050 big_thing_py-0.4.1.5.post9/big_thing_py/staff_thing.py
--rw-r--r--   0        0        0       93 2023-08-18 08:26:19.748139 big_thing_py-0.4.1.5.post9/big_thing_py/super/__init__.py
--rw-r--r--   0        0        0    36127 2023-12-04 00:55:39.761445 big_thing_py-0.4.1.5.post9/big_thing_py/super/super_function.py
--rw-r--r--   0        0        0    12208 2023-08-30 07:44:46.657974 big_thing_py-0.4.1.5.post9/big_thing_py/super/super_mqtt_message.py
--rw-r--r--   0        0        0    17258 2023-08-30 07:44:46.657974 big_thing_py-0.4.1.5.post9/big_thing_py/super/super_request.py
--rw-r--r--   0        0        0    34334 2023-12-04 00:55:39.765445 big_thing_py-0.4.1.5.post9/big_thing_py/super_thing.py
--rw-r--r--   0        0        0      230 2023-04-02 12:40:49.711991 big_thing_py-0.4.1.5.post9/big_thing_py/utils/__init__.py
--rw-r--r--   0        0        0     1905 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/utils/api_util.py
--rw-r--r--   0        0        0      757 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/utils/base64_util.py
--rw-r--r--   0        0        0     8691 2023-11-29 07:38:30.856696 big_thing_py-0.4.1.5.post9/big_thing_py/utils/common_util.py
--rw-r--r--   0        0        0      211 2023-08-18 08:26:19.756139 big_thing_py-0.4.1.5.post9/big_thing_py/utils/exception_util.py
--rw-r--r--   0        0        0      842 2023-08-18 08:26:19.756139 big_thing_py-0.4.1.5.post9/big_thing_py/utils/file_util.py
--rw-r--r--   0        0        0     1356 2023-08-18 08:26:19.756139 big_thing_py-0.4.1.5.post9/big_thing_py/utils/json_util.py
--rw-r--r--   0        0        0     8344 2023-08-30 07:44:46.657974 big_thing_py-0.4.1.5.post9/big_thing_py/utils/log_util.py
--rw-r--r--   0        0        0     2137 2023-08-18 08:26:19.756139 big_thing_py-0.4.1.5.post9/big_thing_py/utils/mqtt_util.py
--rw-r--r--   0        0        0     1676 2023-08-30 07:44:46.657974 big_thing_py-0.4.1.5.post9/big_thing_py/utils/rf_util.py
--rw-r--r--   0        0        0      575 2023-12-04 00:55:42.593420 big_thing_py-0.4.1.5.post9/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 big_thing_py-0.4.1.5.post9/PKG-INFO
+-rw-r--r--   0        0        0     2831 2023-10-11 05:35:40.160391 big_thing_py-0.4.2.0/README.md
+-rw-r--r--   0        0        0       24 2024-04-26 09:04:05.921161 big_thing_py-0.4.2.0/big_thing_py/__init__.py
+-rw-r--r--   0        0        0    57777 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/big_thing.py
+-rw-r--r--   0        0        0       87 2023-10-11 05:35:40.160391 big_thing_py-0.4.2.0/big_thing_py/common/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/common/common.py
+-rw-r--r--   0        0        0     3202 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/common/error.py
+-rw-r--r--   0        0        0    38328 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/common/mxtype.py
+-rw-r--r--   0        0        0     2161 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/common/thread.py
+-rw-r--r--   0        0        0      132 2023-07-31 10:08:18.080866 big_thing_py-0.4.2.0/big_thing_py/core/__init__.py
+-rw-r--r--   0        0        0     2826 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/core/argument.py
+-rw-r--r--   0        0        0     9912 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/core/ble_advertiser.py
+-rw-r--r--   0        0        0    10764 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/core/function.py
+-rw-r--r--   0        0        0    12275 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/core/mqtt_message.py
+-rw-r--r--   0        0        0     3166 2024-04-26 09:03:10.721297 big_thing_py-0.4.2.0/big_thing_py/core/request.py
+-rw-r--r--   0        0        0     5877 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/core/service.py
+-rw-r--r--   0        0        0     1511 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/core/tag.py
+-rw-r--r--   0        0        0    12435 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/core/thing.py
+-rw-r--r--   0        0        0     7425 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/core/value.py
+-rw-r--r--   0        0        0     5010 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/core/wifi_manager.py
+-rw-r--r--   0        0        0       30 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/manager/__init__.py
+-rw-r--r--   0        0        0     1921 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/manager/manager_common.py
+-rw-r--r--   0        0        0    25295 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/manager_thing.py
+-rw-r--r--   0        0        0     2513 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/staff_thing.py
+-rw-r--r--   0        0        0       93 2023-10-11 05:35:40.160391 big_thing_py-0.4.2.0/big_thing_py/super/__init__.py
+-rw-r--r--   0        0        0    35787 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/super/super_function.py
+-rw-r--r--   0        0        0    12160 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/super/super_mqtt_message.py
+-rw-r--r--   0        0        0    17073 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/super/super_request.py
+-rw-r--r--   0        0        0    34284 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/super_thing.py
+-rw-r--r--   0        0        0      230 2023-07-31 10:08:18.080866 big_thing_py-0.4.2.0/big_thing_py/utils/__init__.py
+-rw-r--r--   0        0        0     2368 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/utils/api_util.py
+-rw-r--r--   0        0        0     1347 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/utils/base64_util.py
+-rw-r--r--   0        0        0    10349 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/utils/common_util.py
+-rw-r--r--   0        0        0      211 2023-10-11 05:35:40.160391 big_thing_py-0.4.2.0/big_thing_py/utils/exception_util.py
+-rw-r--r--   0        0        0      842 2023-10-11 05:35:40.160391 big_thing_py-0.4.2.0/big_thing_py/utils/file_util.py
+-rw-r--r--   0        0        0     1356 2023-10-11 05:35:40.160391 big_thing_py-0.4.2.0/big_thing_py/utils/json_util.py
+-rw-r--r--   0        0        0     8615 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/utils/log_util.py
+-rw-r--r--   0        0        0     1896 2024-04-26 09:03:10.725297 big_thing_py-0.4.2.0/big_thing_py/utils/mqtt_util.py
+-rw-r--r--   0        0        0     1676 2023-10-11 05:35:40.160391 big_thing_py-0.4.2.0/big_thing_py/utils/rf_util.py
+-rw-r--r--   0        0        0      730 2024-04-26 09:07:31.984895 big_thing_py-0.4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4059 1970-01-01 00:00:00.000000 big_thing_py-0.4.2.0/PKG-INFO
```

### Comparing `big_thing_py-0.4.1.5.post9/README.md` & `big_thing_py-0.4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/common/common.py` & `big_thing_py-0.4.2.0/big_thing_py/common/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import *
-from typing_extensions import override
+from typing_extensions import override, overload
 from termcolor import *
 from abc import *
 from enum import Enum, auto
 
 
 EMPTY_JSON = {}
-THREAD_TIME_OUT = 0.0001
+THREAD_TIME_OUT = 0.01
 
 
 class TimeFormat(Enum):
     DATETIME1 = '%Y-%m-%d %H:%M:%S'
     DATETIME2 = '%Y%m%d_%H%M%S'
     DATE = '%Y-%m-%d'
     TIME = '%H:%M:%S'
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/common/error.py` & `big_thing_py-0.4.2.0/big_thing_py/common/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,29 @@
 
 class MXErrorCode(Enum):
     NO_ERROR = 0
     FAIL = -1
     TIMEOUT = -2
     NO_PARALLEL = -3
     DUPLICATE = -4
-    NOT_SUPPORTED = -5
+    TARGET_NOT_FOUND = -5
+    REQUESTER_NOT_FOUND = -6
     INVALID_REQUEST = -7
-
-    REGISTER_NO_ERROR = -8
-    REGISTER_FAIL = -9
-    REGISTER_DUPLICATE = -10
-
+    INVALID_DATA = -8
+    TOO_LONG_IDENTIFIER = -9
     EXECUTE_FAIL = -11
     EXECUTE_TIMEOUT = -12
     EXECUTE_NO_PARALLEL = -13
     EXECUTE_DUPLICATE = -14
-
     EXECUTE_ARG_FAIL = -15
-
     VALUE_ERROR = -16
     TYPE_ERROR = -18
     NOT_FOUND_ERROR = -19
+    CONNECTION_ERROR = -20
+    NOT_SUPPORTED = -21
 
     UNDEFINED = 'undefined'
 
     @classmethod
     def to_mx_error_code(cls, type: int):
         if type is not None:
             for mx_error_code in MXErrorCode:
@@ -99,7 +97,12 @@
     def __init__(self, *args: object, **kwargs: dict) -> None:
         super().__init__(MXErrorCode.TYPE_ERROR, *args, **kwargs)
 
 
 class MXNotFoundError(MXError):
     def __init__(self, *args: object, **kwargs: dict) -> None:
         super().__init__(MXErrorCode.NOT_FOUND_ERROR, *args, **kwargs)
+
+
+class MXConnectionError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.CONNECTION_ERROR, *args, **kwargs)
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/common/thread.py` & `big_thing_py-0.4.2.0/big_thing_py/common/thread.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,28 +43,30 @@
 
         self._args = tuple(self._args)
 
         if not self._name:
             self._name = '_'.join(self._target.__name__.split('_')[:-1])
 
         if self._mode == ThreadMode.NORMAL:
-            self._thread = Thread(
-                target=self._target, name=self._name, args=self._args, kwargs=self._kwargs, daemon=self._daemon
-            )
+            self._thread = Thread(target=self._target, name=self._name, args=self._args, kwargs=self._kwargs, daemon=self._daemon)
         elif self._mode == ThreadMode.TIMER:
-            self._thread = Timer(
-                target=self._target, name=self._name, args=self._args, kwargs=self._kwargs, daemon=self._daemon
-            )
+            self._thread = Timer(target=self._target, name=self._name, args=self._args, kwargs=self._kwargs, daemon=self._daemon)
         else:
             raise Exception('[MXThread] Invalid thread mode')
 
     def start(self) -> None:
         self._thread.start()
 
     def join(self) -> None:
         self._thread.join()
 
     def is_alive(self) -> bool:
         return self._thread.is_alive()
 
     def get_name(self) -> str:
         return self._name
+
+    def get_target_function_name(self) -> str:
+        return self._name.split('_')[0]
+
+    def get_target_scenario_name(self) -> str:
+        return self._name.split('_')[1]
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/core/function.py` & `big_thing_py-0.4.2.0/big_thing_py/core/function.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from big_thing_py.common import *
 from big_thing_py.core.request import *
 from big_thing_py.core.mqtt_message import *
 from big_thing_py.core.argument import *
 from big_thing_py.core.service import *
 
-from func_timeout import StoppableThread, FunctionTimedOut
-import threading
+import asyncio
 
 
 class MXFunction(MXService):
+
     def __init__(
         self,
         func: Callable,
         tag_list: List[MXTag],
         return_type: MXType,
         name: str = '',
+        category: MXFunctionCategory = MXFunctionCategory.undefined,
         energy: float = 0,
         desc: str = '',
         thing_name: str = '',
         middleware_name: str = '',
         arg_list: List[MXArgument] = [],
         exec_time: float = 0,
         timeout: float = 0,
         range_type: MXRangeType = MXRangeType.SINGLE,
     ) -> None:
         super().__init__(
             func=func,
             tag_list=tag_list,
             name=name,
+            category=category,
             energy=energy,
             desc=desc,
             thing_name=thing_name,
             middleware_name=middleware_name,
         )
 
         self._return_type = return_type
@@ -41,60 +43,55 @@
         # TODO: range_type will be removed from MXFunction
         self._range_type = range_type
 
         self._return_value = None
         self._running = False
         self._running_scenario_list: List[str] = []
 
-        # Queue
-        self._publish_queue: Queue = None
-
         if self._return_type in [MXType.UNDEFINED] or isinstance(self._return_type, str):
             raise MXValueError('return_type cannot be undefined or `str` type')
         if (not len(self._arg_list) == len(get_function_info(self._func)['args'])) if self._func else False:
-            raise MXValueError('Length of argument list must be same with callback function')
+            raise MXValueError(
+                f'Length of argument list must be same with callback function.\n'
+                f'given: {len(self._arg_list)}, expected: {len(get_function_info(self._func)["args"])}'
+            )
 
         # TODO: return type detection feature
         # if not self._return_type or self._return_type in [MXType.UNDEFINED]:
         #     func_info = get_function_info(self._func)
         #     self._return_type = MXType().get(func_info[2])
         #     raise MXValueError('type must be specified')
         # elif self._return_type in [MXType.UNDEFINED]:
         #     raise MXValueError('type cannot be undefined or void')
 
+        self._category = MXFunctionCategory.get(self._func.__name__)
+
     def __eq__(self, o: 'MXFunction') -> bool:
         instance_check = isinstance(o, MXFunction)
         arg_list_check = o._arg_list == self._arg_list
         return_type_check = o._return_type == self._return_type
         exec_time_check = o._exec_time == self._exec_time
         timeout_check = o._timeout == self._timeout
         range_type_check = o._range_type == self._range_type
 
         return (
-            super().__eq__(o)
-            and instance_check
-            and arg_list_check
-            and return_type_check
-            and exec_time_check
-            and timeout_check
-            and range_type_check
+            super().__eq__(o) and instance_check and arg_list_check and return_type_check and exec_time_check and timeout_check and range_type_check
         )
 
     def __getstate__(self):
         state = super().__getstate__()
 
         state['_return_type'] = self._return_type
         state['_arg_list'] = self._arg_list
         state['_exec_time'] = self._exec_time
         state['_timeout'] = self._timeout
         state['_range_type'] = self._range_type
 
         del state['_return_value']
         del state['_running']
-        del state['_publish_queue']
         del state['_running_scenario_list']
 
         return state
 
     def __setstate__(self, state):
         super().__setstate__(state)
 
@@ -102,258 +99,200 @@
         self._min = state['_min']
         self._max = state['_max']
         self._cycle = state['_cycle']
         self._format = state['_format']
 
         self._return_value = None
         self._running = False
-        self._publish_queue = None
         self._running_scenario_list = []
 
-    def _wrapper(self, execute_request: MXExecuteRequest) -> bool:
+    async def _async_wrapper(self, *args, **kwargs):
+        return self._func(*args, **kwargs)
+
+    async def execute(self, execute_request: Union[MXExecuteRequest, MXInnerExecuteRequest]) -> Tuple['MXFunction', MXErrorCode]:
         execute_msg = execute_request.trigger_msg
+        self._running_scenario_list.append(execute_msg.scenario)
+        execute_request.timer_start()
+
+        execute_msg = execute_request._trigger_msg
         MXLOG_DEBUG(f'[FUNC RUN] run {self._name} function by {execute_msg.scenario}', 'green')
 
         try:
             if not isinstance(execute_msg, MXExecuteMessage):
-                raise Exception(
-                    f'[{get_current_function_name()}] Wrong ExecuteMessage type - execute_msg: {type(execute_msg)}'
-                )
+                raise Exception(f'[{get_current_function_name()}] Wrong ExecuteMessage type - execute_msg: {type(execute_msg)}')
 
             self._running = True
-            error = MXErrorCode.NO_ERROR
+            execute_request.result_msg.error = MXErrorCode.NO_ERROR
 
             if self._timeout:
-                # self._return_value = func_timeout(self._timeout, self._func, args=(*execute_msg.tuple_arguments(), ))
-                current_thread = threading.current_thread()
-                self._return_value = self._run_with_timeout(
-                    timeout=self._timeout,
-                    func=self._func,
-                    name=current_thread.name,
-                    user_data=dict(scenario=execute_msg.scenario),
-                    args=(*execute_msg.tuple_arguments(),),
-                )
+                if asyncio.iscoroutinefunction(self._func):
+                    self._return_value = await asyncio.wait_for(self._func(*execute_msg.tuple_arguments()), timeout=self._timeout)
+                else:
+                    self._return_value = await asyncio.wait_for(self._async_wrapper(*execute_msg.tuple_arguments()), timeout=self._timeout)
             else:
-                self._return_value = self._func(*execute_msg.tuple_arguments())
+                if asyncio.iscoroutinefunction(self._func):
+                    self._return_value = await self._func(*execute_msg.tuple_arguments())
+                else:
+                    self._return_value = await self._async_wrapper(*execute_msg.tuple_arguments())
         except KeyboardInterrupt as e:
             # TODO: for wrapup main thread, but not test it yet
             print_error(e)
             MXLOG_DEBUG('Function execution exit by user', 'red')
             raise e
-        except FunctionTimedOut as e:
-            MXLOG_DEBUG(
-                f'[FUNC TIMEOUT] function {self._name} by scenario {execute_msg.scenario} was timeout!!!', 'yellow'
-            )
-            error = MXErrorCode.TIMEOUT
-        except Exception as e:
+        except asyncio.CancelledError as e:
+            # TODO: for wrapup main thread, but not test it yet
+            print_error(e)
+            MXLOG_DEBUG('Function execution exit by user', 'red')
+            raise e
+        except asyncio.TimeoutError as e:
+            MXLOG_DEBUG(f'[FUNC TIMEOUT] function {self._name} by scenario {execute_msg.scenario} was timeout!!!', 'yellow')
+            execute_request.result_msg.error = MXErrorCode.TIMEOUT
+        except BaseException as e:
             print_error(e)
             MXLOG_DEBUG(
                 f'[FUNC FAIL] function {self._name} by scenario {execute_msg.scenario} is failed while executing!!!',
                 'red',
             )
-            error = MXErrorCode.FAIL
+            execute_request.result_msg.error = MXErrorCode.FAIL
         else:
-            error = MXErrorCode.NO_ERROR
+            execute_request.result_msg.error = MXErrorCode.NO_ERROR
         finally:
-            # result_msg = MXExecuteResultMessage(function=self,
-            #                                      scenario=execute_msg.scenario,
-            #                                      request_ID=execute_request.trigger_msg.request_ID,
-            #                                      error=error)
-            # execute_request.set_return_msg(result_msg)
-            self._send_TM_RESULT_EXECUTE(scenario=execute_msg.scenario, error=error, request_ID=execute_msg.request_ID)
+            if isinstance(self._return_value, str) and is_base64(self._return_value) and self._return_type != MXType.BINARY:
+                raise MXValueError('return value is base64, but type is not BINARY')
 
-            execute_request.timer_end()
             self._running = False
             self._running_scenario_list.remove(execute_msg.scenario)
+
+            execute_request.result_msg.return_value = self._return_value
+            execute_request.timer_end()
             MXLOG_DEBUG(
                 f'[FUNC END] function {self._name} end. -> return value : {self._return_value}, duration: {execute_request.duration():.4f} Sec',
                 'green',
             )
 
-    def start_execute_thread(self, execute_msg: MXExecuteMessage) -> MXThread:
-        execute_result_msg = MXExecuteResultMessage(function=self, scenario=execute_msg.scenario)
-        execute_request = MXExecuteRequest(trigger_msg=execute_msg, result_msg=execute_result_msg)
-        self._running_scenario_list.append(execute_msg.scenario)
-        execute_request.timer_start()
-
-        execute_thread = MXThread(
-            target=self._wrapper,
-            name=f'{self._func.__name__}_{execute_msg.scenario}_thread',
-            daemon=True,
-            args=(execute_request,),
-        )
-        execute_thread.start()
-
-        return execute_thread
-
-    def _run_with_timeout(
-        self,
-        timeout: float,
-        func: Callable,
-        name: str = '',
-        user_data: dict = None,
-        args: tuple = (),
-        kwargs: dict = None,
-    ):
-        if not kwargs:
-            kwargs = {}
-        if not args:
-            args = ()
-
-        ret = []
-        exception = []
-        isStopped = False
-
-        def funcwrap(args2, kwargs2):
-            try:
-                ret.append(func(*args2, **kwargs2))
-            except FunctionTimedOut:
-                # Don't print traceback to stderr if we time out
-                pass
-            except Exception as e:
-                exc_info = sys.exc_info()
-                if isStopped is False:
-                    # Assemble the alternate traceback, excluding this function
-                    #  from the trace (by going to next frame)
-                    # Python3 reads native from __traceback__,
-                    # python2 has a different form for "raise"
-                    e.__traceback__ = exc_info[2].tb_next
-                    exception.append(e)
-
-        thread = StoppableThread(target=funcwrap, name=name, args=(args, kwargs))
-        thread.daemon = True
-        thread.user_data = user_data
-
-        thread.start()
-        thread.join(timeout)
-
-        stopException = None
-        if thread.is_alive():
-            isStopped = True
-
-            class FunctionTimedOutTempType(FunctionTimedOut):
-                def __init__(self):
-                    return FunctionTimedOut.__init__(self, '', timeout, func, args, kwargs)
-
-            FunctionTimedOutTemp = type(
-                'FunctionTimedOut' + str(hash("%d_%d_%d_%d" % (id(timeout), id(func), id(args), id(kwargs)))),
-                FunctionTimedOutTempType.__bases__,
-                dict(FunctionTimedOutTempType.__dict__),
-            )
-
-            stopException = FunctionTimedOutTemp
-            thread._stopThread(stopException)
-            thread.join(min(0.1, timeout / 50.0))
-            raise FunctionTimedOut('', timeout, func, args, kwargs)
-        else:
-            # We can still cleanup the thread here..
-            # Still give a timeout... just... cuz..
-            thread.join(0.5)
-
-        if exception:
-            raise exception[0] from None
-
-        if ret:
-            return ret[0]
-
-    def _send_TM_RESULT_EXECUTE(self, scenario: str, error: MXErrorCode, request_ID: str = None) -> None:
-        execute_result_msg = self.generate_execute_result_message(scenario=scenario, error=error, request_ID=request_ID)
-        execute_result_mqtt_msg = execute_result_msg.mqtt_message()
-        self._publish_queue.put(execute_result_mqtt_msg)
+            return execute_request
 
     def dict(self) -> dict:
         return {
             "name": self._name,
+            "category": self._category.value,
             "description": self._desc,
             "exec_time": self._exec_time * 1000 if self._exec_time is not None else 0,
             "return_type": self._return_type.value,
             "energy": self._energy,
             "tags": [tag.dict() for tag in self._tag_list],
-            "use_arg": 1 if self._arg_list else 0,
+            "use_arg": 1 if len(self._arg_list) > 0 else 0,
             "arguments": [argument.dict() for argument in self._arg_list] if self._arg_list else [],
         }
 
     # ========================
     #         _    _  _
     #        | |  (_)| |
     #  _   _ | |_  _ | | ___
     # | | | || __|| || |/ __|
     # | |_| || |_ | || |\__ \
     #  \__,_| \__||_||_||___/
     # ========================
 
     def generate_execute_result_message(
-        self, scenario: str, error: MXErrorCode, request_ID: str
+        self,
+        execute_request: Union[MXExecuteRequest, MXInnerExecuteRequest],
     ) -> MXExecuteResultMessage:
-        execute_result_msg = MXExecuteResultMessage(
-            function=self, scenario=scenario, request_ID=request_ID, error=error
+        trigger_msg = execute_request.trigger_msg
+        result_msg = execute_request.result_msg
+
+        return MXExecuteResultMessage(
+            function_name=trigger_msg.function_name,
+            thing_name=result_msg.thing_name,
+            middleware_name=result_msg.middleware_name,
+            scenario=trigger_msg.scenario,
+            client_id=trigger_msg.client_id,
+            request_ID=trigger_msg.request_ID,
+            return_type=result_msg.return_type,
+            return_value=result_msg.return_value,
+            error=result_msg.error,
+            action_type=execute_request.action_type,
         )
-        return execute_result_msg
 
     # ====================================
     #               _    _
     #              | |  | |
     #   __ _   ___ | |_ | |_   ___  _ __
     #  / _` | / _ \| __|| __| / _ \| '__|
     # | (_| ||  __/| |_ | |_ |  __/| |
     #  \__, | \___| \__| \__| \___||_|
     #   __/ |
     #  |___/
     # ====================================
 
-    def get_exec_time(self) -> float:
+    @property
+    def exec_time(self) -> float:
         return self._exec_time
 
-    def get_timeout(self) -> float:
+    @property
+    def timeout(self) -> float:
         return self._timeout
 
-    def get_arg_list(self) -> List[MXArgument]:
+    @property
+    def arg_list(self) -> List[MXArgument]:
         return self._arg_list
 
-    def get_return_type(self) -> MXType:
+    @property
+    def return_type(self) -> MXType:
         return self._return_type
 
-    def get_return_value(self) -> Union[int, float, str, bool]:
+    @property
+    def return_value(self) -> Union[int, float, str, bool]:
         return self._return_value
 
-    def get_running(self) -> bool:
+    @property
+    def running(self) -> bool:
         return self._running
 
-    def get_range_type(self) -> MXRangeType:
+    @property
+    def range_type(self) -> MXRangeType:
         return self._range_type
 
-    def get_running_scenario_list(self) -> List[str]:
+    @property
+    def running_scenario_list(self) -> List[str]:
         return self._running_scenario_list
 
     # ==================================
     #             _    _
     #            | |  | |
     #  ___   ___ | |_ | |_   ___  _ __
     # / __| / _ \| __|| __| / _ \| '__|
     # \__ \|  __/| |_ | |_ |  __/| |
     # |___/ \___| \__| \__| \___||_|
     # ==================================
 
-    def set_exec_time(self, exec_time: float) -> None:
+    @exec_time.setter
+    def exec_time(self, exec_time: float) -> None:
         self._exec_time = exec_time
 
-    def set_timeout(self, timeout: float) -> None:
+    @timeout.setter
+    def timeout(self, timeout: float) -> None:
         self._timeout = timeout
 
-    def set_arg_list(self, arg_list: List[MXArgument]) -> None:
+    @arg_list.setter
+    def arg_list(self, arg_list: List[MXArgument]) -> None:
         self._arg_list = arg_list
 
-    def set_return_type(self, return_type: MXType) -> None:
+    @return_type.setter
+    def return_type(self, return_type: MXType) -> None:
         self._return_type = return_type
 
-    def set_return_value(self, return_value: Union[int, float, str, bool]) -> None:
+    @return_value.setter
+    def return_value(self, return_value: Union[int, float, str, bool]) -> None:
         self._return_value = return_value
 
-    def set_running(self, running: bool) -> None:
+    @running.setter
+    def running(self, running: bool) -> None:
         self._running = running
 
-    def set_range_type(self, range_type: MXRangeType) -> None:
+    @range_type.setter
+    def range_type(self, range_type: MXRangeType) -> None:
         self._range_type = range_type
 
-    # for link to big_thing's publish_queue
-    def set_publish_queue(self, queue: Queue):
-        self._publish_queue = queue
+
+if __name__ == '__main__':
+    pass
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/core/mqtt_message.py` & `big_thing_py-0.4.2.0/big_thing_py/core/mqtt_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,115 +5,155 @@
     return '@'.join([scenario_name, requester_middleware_name])
 
 
 def make_sub_service_request_key(sub_service_name: str, sub_service_request_order: int) -> str:
     return '@'.join([sub_service_name, str(sub_service_request_order)])
 
 
-def make_request_ID(
-    requester_middleware_name: str, super_thing_name: str, super_service_name: str, sub_service_request_order: int
-):
+def make_request_ID(requester_middleware_name: str, super_thing_name: str, super_service_name: str, sub_service_request_order: int):
     return '@'.join([requester_middleware_name, super_thing_name, super_service_name, str(sub_service_request_order)])
 
 
 class MXMQTTMessage:
-    def __init__(self) -> None:
-        self._protocol_type: Union[MXProtocolType.Base, MXProtocolType.Super, MXProtocolType.WebClient] = None
-        self.timestamp: float = None
+    def __init__(self, protocol_type: Union[MXProtocolType.Base, MXProtocolType.Super, MXProtocolType.WebClient]) -> None:
+        self.protocol_type = protocol_type
         self.topic: str = None
+        self.timestamp: float = None
+
+        self.topic_error: bool = False
+        self.payload_error: bool = False
 
     def set_timestamp(self, timestamp: float = None) -> None:
         if timestamp:
             self.timestamp = timestamp
         else:
             self.timestamp = time.time()
 
 
 class MXMQTTSendMessage(MXMQTTMessage):
-    def __init__(self) -> None:
-        super().__init__()
-        self.payload: dict = None
+    def __init__(self, topic: str, payload: dict, protocol_type: Union[MXProtocolType.Base, MXProtocolType.Super, MXProtocolType.WebClient]) -> None:
+        super().__init__(protocol_type)
+        self.topic = topic
+        self.payload = payload
 
-    def mqtt_message(self) -> mqtt.MQTTMessage:
+        if MXProtocolType.get(self.topic) != self.protocol_type:
+            self.topic_error = True
+        else:
+            self.topic_error = False
+
+    def mqtt_message(self) -> MQTTMessage:
         msg = encode_MQTT_message(self.topic, self.payload)
         return msg
 
 
 class MXMQTTReceiveMessage(MXMQTTMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__()
-        self.topic, self.payload, self.timestamp = decode_MQTT_message(msg)
-        self.topic_error: bool = False
-        self.payload_error: bool = False
+    def __init__(self, msg: MQTTMessage, protocol_type: Union[MXProtocolType.Base, MXProtocolType.Super, MXProtocolType.WebClient]) -> None:
+        super().__init__(protocol_type)
+        self.topic, self.payload = decode_MQTT_message(msg)
+
+        if MXProtocolType.get(self.topic) != self.protocol_type:
+            self.topic_error = True
+        else:
+            self.topic_error = False
+
+
+##############################################################################################################################
 
 
 class MXRegisterMessage(MXMQTTSendMessage):
-    def __init__(self, thing) -> None:
-        from big_thing_py.core.thing import MXThing
+    def __init__(self, thing_name: str, payload: dict) -> None:
+        protocol_type = MXProtocolType.Base.TM_REGISTER
+        topic = protocol_type.value % (thing_name)
+        super().__init__(topic=topic, payload=payload, protocol_type=protocol_type)
 
-        thing: MXThing = thing
 
-        super().__init__()
-        self._protocol_type = MXProtocolType.Base.TM_REGISTER
-        self.topic = self._protocol_type.value % (thing.get_name())
-        self.payload = thing.dict()
+class MXRequestRegisterInfoMessage(MXMQTTReceiveMessage):
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg, protocol_type=MXProtocolType.Base.MT_REQUEST_REGISTER_INFO)
+        self.middleware_name = self.topic.split('/')[2]
+        self.error: MXErrorCode = None
 
+        self.client_id: str = self.payload.get('client_id', None)
+        if self.client_id is None:
+            self.payload_error = True
 
-##############################################################################################################################
+
+class MXRequestUnregisterMessage(MXMQTTReceiveMessage):
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg, protocol_type=MXProtocolType.Base.MT_REQUEST_UNREGISTER)
+        self.middleware_name = self.topic.split('/')[2]
+        self.error: MXErrorCode = None
+
+        self.client_id: str = self.payload.get('client_id', None)
+        if self.client_id is None:
+            self.payload_error = True
 
 
 class MXRegisterResultMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.Base.MT_RESULT_REGISTER
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg, protocol_type=MXProtocolType.Base.MT_RESULT_REGISTER)
         self.thing_name = self.topic.split('/')[3]
         self.middleware_name: str = self.payload['middleware_name']
         self.error: MXErrorCode = MXErrorCode.get(self.payload['error'])
 
 
 class MXUnregisterMessage(MXMQTTSendMessage):
-    def __init__(self, thing) -> None:
-        from big_thing_py.core.thing import MXThing
-
-        thing: MXThing = thing
-
-        super().__init__()
-        self._protocol_type = MXProtocolType.Base.TM_UNREGISTER
-        self.topic = self._protocol_type.value % (thing.get_name())
-        self.payload = EMPTY_JSON
+    def __init__(self, thing_name: str) -> None:
+        protocol_type = MXProtocolType.Base.TM_UNREGISTER
+        topic = protocol_type.value % (thing_name)
+        payload = EMPTY_JSON
+        super().__init__(topic=topic, payload=payload, protocol_type=protocol_type)
 
 
 class MXUnregisterResultMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.Base.MT_RESULT_UNREGISTER
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg, protocol_type=MXProtocolType.Base.MT_RESULT_UNREGISTER)
         self.thing_name: str = self.topic.split('/')[3]
         self.error: MXErrorCode = MXErrorCode.get(self.payload['error'])
 
 
 class MXExecuteMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.Base.MT_EXECUTE
-        self.function_name: str = self.topic.split('/')[2]
-        self.thing_name: str = self.topic.split('/')[3]
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg, protocol_type=MXProtocolType.get(msg.topic.decode()))
+
+        if self.protocol_type in [MXProtocolType.Base.MT_EXECUTE, MXProtocolType.Base.MT_IN_EXECUTE]:
+            self.topic_error = False
+        else:
+            self.topic_error = True
+            return
 
-        if len(self.topic.split('/')) == 6:
-            self.middleware_name: str = self.topic.split('/')[4]
-            self.request_ID: str = self.topic.split('/')[5]
-            if not self.middleware_name or not self.request_ID:
+        self.middleware_name: str = ''
+        self.request_ID: str = ''
+        self.client_id: str = ''
+
+        if self.protocol_type == MXProtocolType.Base.MT_EXECUTE:
+            self.function_name: str = self.topic.split('/')[2]
+            self.thing_name: str = self.topic.split('/')[3]
+
+            if len(self.topic.split('/')) == 6:
+                # MT/EXECUTE/[FunctionName]/[ThingName]/[TargetMiddlewareName]/[Request_ID] topic
+                self.middleware_name: str = self.topic.split('/')[4]
+                self.request_ID: str = self.topic.split('/')[5]
+                if not self.middleware_name or not self.request_ID:
+                    self.topic_error = True
+            elif len(self.topic.split('/')) == 4:
+                # MT/EXECUTE/[FunctionName]/[ThingName] topic
+                self.middleware_name: str = ''
+                self.request_ID: str = ''
+            else:
                 self.topic_error = True
-        elif len(self.topic.split('/')) == 4:
+        elif self.protocol_type == MXProtocolType.Base.MT_IN_EXECUTE:
+            self.function_name: str = self.topic.split('/')[3]
+            self.thing_name: str = self.topic.split('/')[4]
             self.middleware_name: str = ''
             self.request_ID: str = ''
-        else:
-            self.topic_error = True
 
         self.scenario: str = self.payload.get('scenario', '')
         self.arguments: List[dict] = self.payload.get('arguments', [])
+        self.client_id: str = self.payload.get('client_id', '')
 
         if not self.scenario or self.arguments == None:
             self.payload_error = True
         elif not all([isinstance(arg.get('order', None), int) for arg in self.arguments]) or not all(
             [isinstance(arg.get('value', None), (int, float, str, bool)) for arg in self.arguments]
         ):
             self.payload_error = True
@@ -127,120 +167,133 @@
         self.arguments = sorted(self.arguments, key=lambda x: int(x['order']))
         json_arguments = [dict(order=arg['order'], value=arg['value']) for arg in self.arguments]
         return json_arguments
 
 
 class MXExecuteResultMessage(MXMQTTSendMessage):
     def __init__(
-        self, function, scenario: str, request_ID: str = '', error: MXErrorCode = MXErrorCode.UNDEFINED
+        self,
+        function_name: str = '',
+        thing_name: str = '',
+        middleware_name: str = '',
+        scenario: str = '',
+        client_id: str = '',
+        request_ID: str = '',
+        return_type: MXType = MXType.UNDEFINED,
+        return_value: Union[int, float, str, bool] = None,
+        error: MXErrorCode = MXErrorCode.UNDEFINED,
+        action_type: MXActionType = MXActionType.EXECUTE,
     ) -> None:
-        from big_thing_py.core.function import MXFunction
+        if action_type == MXActionType.EXECUTE:
+            protocol_type = MXProtocolType.Base.TM_RESULT_EXECUTE
+        elif action_type == MXActionType.INNER_EXECUTE:
+            protocol_type = MXProtocolType.Base.TM_IN_RESULT_EXECUTE
+        else:
+            self.topic_error = True
+            return
 
-        super().__init__()
-        self._protocol_type = MXProtocolType.Base.TM_RESULT_EXECUTE
-        self.function: MXFunction = function
-        self.request_ID = request_ID
+        self.function_name = function_name
+        self.thing_name = thing_name
+        self.middleware_name = middleware_name
         self.scenario = scenario
+        self.client_id = client_id
+        self.request_ID = request_ID
+        self.return_type = return_type
+        self.return_value = return_value
         self._error = error
 
         if self.request_ID:
-            self.topic = self._protocol_type.value % (
-                self.function.get_name(),
-                self.function.get_thing_name(),
-                self.function.get_middleware_name(),
+            topic = protocol_type.value % (
+                self.function_name,
+                self.thing_name,
+                self.middleware_name,
                 self.request_ID,
             )
         else:
-            self.topic = (
-                self._protocol_type.value % (self.function.get_name(), self.function.get_thing_name(), '', '')
-            ).rstrip('/')
+            if action_type == MXActionType.EXECUTE:
+                topic = (protocol_type.value % (self.function_name, self.thing_name, '', '')).rstrip('/')
+            elif action_type == MXActionType.INNER_EXECUTE:
+                topic = protocol_type.value % (self.function_name, self.thing_name)
+
+        if action_type == MXActionType.EXECUTE:
+            payload = dict(
+                error=self._error.value,
+                scenario=self.scenario,
+                return_type=self.return_type.value,
+                return_value=self.return_value,
+            )
+        elif action_type == MXActionType.INNER_EXECUTE:
+            payload = dict(
+                error=self._error.value,
+                scenario=self.scenario,
+                client_id=self.client_id,
+                return_type=self.return_type.value,
+                return_value=self.return_value,
+            )
 
-        self.payload = dict(
-            error=self._error.value,
-            scenario=self.scenario,
-            return_type=self.function.get_return_type().value,
-            return_value=self.function.get_return_value(),
-        )
+        super().__init__(topic=topic, payload=payload, protocol_type=protocol_type)
 
     @property
     def error(self) -> dict:
         return self._error
 
     @error.setter
     def error(self, error: MXErrorCode):
         if not isinstance(error, MXErrorCode):
             raise MXTypeError("error must be an MXErrorType")
         self._error = error
         self.payload = dict(
             error=self._error.value,
             scenario=self.scenario,
-            return_type=self.function.get_return_type().value,
-            return_value=self.function.get_return_value(),
+            return_type=self.return_type.value,
+            return_value=self.return_value,
         )
 
 
 # TODO: binary 부분 구현 완료 후 작성하기
 class MXBinaryValueResultMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.Base.MT_RESULT_BINARY_VALUE
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg, protocol_type=MXProtocolType.Base.MT_RESULT_BINARY_VALUE)
         self.thing_name = self.topic.split('/')[3]
-        self.value_name = self.payload['value_name']
+        self.value_name = self.payload['value']
 
 
 class MXAliveMessage(MXMQTTSendMessage):
-    def __init__(self, thing) -> None:
-        from big_thing_py.core.thing import MXThing
-
-        thing: MXThing = thing
-
-        super().__init__()
-        self._protocol_type = MXProtocolType.Base.TM_ALIVE
-        self.topic = self._protocol_type.value % (thing.get_name())
-        self.payload = EMPTY_JSON
+    def __init__(self, thing_name: str) -> None:
+        protocol_type = MXProtocolType.Base.TM_ALIVE
+        topic = protocol_type.value % (thing_name)
+        payload = EMPTY_JSON
+        super().__init__(topic=topic, payload=payload, protocol_type=protocol_type)
 
 
 class MXValuePublishMessage(MXMQTTSendMessage):
-    def __init__(self, thing, value) -> None:
-        from big_thing_py.core.thing import MXThing
-        from big_thing_py.core.value import MXValue
-
-        thing: MXThing = thing
-        value: MXValue = value
-
-        super().__init__()
-        self._protocol_type = MXProtocolType.Base.TM_VALUE_PUBLISH
-        self.topic = self._protocol_type.value % (value.get_name(), thing.get_name())
-        self.payload = value.publish_dict()
+    def __init__(self, value_name: str, thing_name: str, payload: dict) -> None:
+        protocol_type = MXProtocolType.Base.TM_VALUE_PUBLISH
+        topic = protocol_type.value % (value_name, thing_name)
+        super().__init__(topic=topic, payload=payload, protocol_type=protocol_type)
 
 
 # for middleware detect
-class MXClientServiceListResultMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.WebClient.ME_RESULT_SERVICE_LIST
+class MXHomeResultMessage(MXMQTTReceiveMessage):
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg, protocol_type=MXProtocolType.WebClient.ME_RESULT_HOME)
         self._client_id = self.topic.split('/')[3]
 
 
-class MXClientRefreshMessage(MXMQTTSendMessage):
-    def __init__(self, thing) -> None:
-        from big_thing_py.core.thing import MXThing
-
-        thing: MXThing = thing
-
-        super().__init__()
-        self._protocol_type = MXProtocolType.WebClient.EM_REFRESH
-        self.topic = self._protocol_type.value % (thing.get_name())
-        self.payload = EMPTY_JSON
+class MXGetHomeMessage(MXMQTTSendMessage):
+    def __init__(self, thing_name: str) -> None:
+        protocol_type = MXProtocolType.WebClient.EM_GET_HOME
+        topic = protocol_type.value % (thing_name)
+        payload = EMPTY_JSON
+        super().__init__(topic=topic, payload=payload, protocol_type=protocol_type)
 
 
 class MXNotifyMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.WebClient.ME_NOTIFY_CHANGE
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg, protocol_type=MXProtocolType.WebClient.ME_NOTIFY_CHANGE)
 
         # topic
         self._client_id = self.topic.split('/')[2]
 
         # payload
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/core/service.py` & `big_thing_py-0.4.2.0/big_thing_py/core/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 from big_thing_py.core.tag import *
 from abc import *
+from asyncio import iscoroutinefunction
 
 
 class MXService(metaclass=ABCMeta):
+
     def __init__(
         self,
         name: str,
-        func: Callable,
+        category: Union[MXValueCategory, MXFunctionCategory],
+        func: Union[Callable, Coroutine],
         tag_list: List[MXTag],
         energy: float,
         desc: str,
         thing_name: str,
         middleware_name: str,
     ) -> None:
         self._name = name
+        self._category = category
         self._func = func
         self._tag_list = tag_list
         self._energy = energy
         self._desc = desc
         self._thing_name = thing_name
         self._middleware_name = middleware_name
 
-        if not callable(self._func):
-            raise MXValueError(f'func must be callable')
+        if not callable(self._func) and not iscoroutinefunction(self._func):
+            raise MXValueError(f'func must be callable or coroutine function.')
         if not self._name:
             self._name = func.__name__
-        if not check_valid_identifier(self._name):
-            raise MXValueError(
-                f'name cannot be empty & can only contain alphanumeric characters and underscores. name: {self._name}'
-            )
+        if check_valid_identifier(self._name) == MXErrorCode.INVALID_DATA:
+            raise MXValueError(f'name cannot be empty & can only contain alphanumeric characters and underscores. name: {self._name}')
+        elif check_valid_identifier(self._name) == MXErrorCode.TOO_LONG_IDENTIFIER:
+            raise MXValueError(f'too long identifier. name: {self._name}, length: {len(self._name)}')
+
         if any([not isinstance(tag, MXTag) for tag in self._tag_list]) or len(self._tag_list) == 0:
             raise MXValueError('tag_list must contain MXTag object')
         else:
-            self._tag_list = [MXTag(name=tag) for tag in sorted(list(set(self.get_tag_list(string_mode=True))))]
+            self.sort_tag()
+
         if not isinstance(self._energy, (int, float)):
             raise MXValueError(f'energy must be int or float')
         if not isinstance(self._desc, str):
             raise MXValueError(f'desc must be str')
         if not isinstance(self._thing_name, str):
             raise MXValueError(f'thing_name must be str')
         if not isinstance(self._middleware_name, str):
@@ -47,23 +53,15 @@
         name_check = o._name == self._name
         thing_name_check = o._thing_name == self._thing_name
         middleware_name_check = o._middleware_name == self._middleware_name
         tag_list_check = o._tag_list == self._tag_list
         func_check = o._func == self._func
         energy_check = o._energy == self._energy
 
-        return (
-            instance_check
-            and name_check
-            and thing_name_check
-            and middleware_name_check
-            and tag_list_check
-            and func_check
-            and energy_check
-        )
+        return instance_check and name_check and thing_name_check and middleware_name_check and tag_list_check and func_check and energy_check
 
     def __getstate__(self):
         state = self.__dict__.copy()
 
         del state['_func']
 
         return state
@@ -80,26 +78,30 @@
         if isinstance(tag, MXTag):
             if not tag in self._tag_list:
                 self._tag_list.append(tag)
         elif all(isinstance(t, MXTag) for t in tag):
             for t in tag:
                 if not t in self._tag_list:
                     self._tag_list.append(t)
-        self._tag_list = sorted(self._tag_list, key=lambda x: x.get_name())
+        self._tag_list = sorted(self._tag_list, key=lambda x: x.name)
 
         return self
 
     def remove_tag(self, tag: str) -> 'MXService':
         if not isinstance(tag, str):
             raise Exception('tag to remove must be str')
 
         for t in self._tag_list:
-            if t.get_name() == tag:
+            if t.name == tag:
                 self._tag_list.remove(MXTag(tag))
 
+    def sort_tag(self) -> 'MXService':
+        self._tag_list = sorted(self._tag_list, key=lambda x: x.name)
+        return self
+
     @abstractmethod
     def dict(self) -> dict:
         pass
 
     # ====================================
     #               _    _
     #              | |  | |
@@ -107,60 +109,79 @@
     #  / _` | / _ \| __|| __| / _ \| '__|
     # | (_| ||  __/| |_ | |_ |  __/| |
     #  \__, | \___| \__| \__| \___||_|
     #   __/ |
     #  |___/
     # ====================================
 
-    def get_name(self) -> str:
+    @property
+    def name(self) -> str:
         return self._name
 
-    def get_thing_name(self) -> str:
+    @property
+    def category(self) -> Union[MXValueCategory, MXFunctionCategory]:
+        return self._category
+
+    @property
+    def thing_name(self) -> str:
         return self._thing_name
 
-    def get_middleware_name(self) -> str:
+    @property
+    def middleware_name(self) -> str:
         return self._middleware_name
 
-    def get_tag_list(self, string_mode: bool = False) -> List[MXTag]:
-        if string_mode:
-            return [str(tag) for tag in self._tag_list]
-        else:
-            return self._tag_list
+    @property
+    def tag_list(self) -> List[MXTag]:
+        return self._tag_list
 
-    def get_desc(self) -> str:
+    @property
+    def desc(self) -> str:
         return self._desc
 
-    def get_func(self) -> Callable:
+    @property
+    def func(self) -> Callable:
         return self._func
 
-    def get_energy(self) -> float:
+    @property
+    def energy(self) -> float:
         return self._energy
 
     # ==================================
     #             _    _
     #            | |  | |
     #  ___   ___ | |_ | |_   ___  _ __
     # / __| / _ \| __|| __| / _ \| '__|
     # \__ \|  __/| |_ | |_ |  __/| |
     # |___/ \___| \__| \__| \___||_|
     # ==================================
 
-    def set_name(self, name: str) -> None:
+    @name.setter
+    def name(self, name: str) -> None:
         self._name = name
 
-    def set_thing_name(self, thing_name: str) -> None:
+    @category.setter
+    def category(self, category: Union[MXValueCategory, MXFunctionCategory]) -> None:
+        self._category = category
+
+    @thing_name.setter
+    def thing_name(self, thing_name: str) -> None:
         self._thing_name = thing_name
 
-    def set_middleware_name(self, middleware_name: str) -> None:
+    @middleware_name.setter
+    def middleware_name(self, middleware_name: str) -> None:
         self._middleware_name = middleware_name
 
-    def set_tag_list(self, tag_list: List[MXTag]) -> None:
+    @tag_list.setter
+    def tag_list(self, tag_list: List[MXTag]) -> None:
         self._tag_list = tag_list
 
-    def set_desc(self, desc: str) -> None:
+    @desc.setter
+    def desc(self, desc: str) -> None:
         self._desc = desc
 
-    def set_func(self, func: Callable) -> None:
+    @func.setter
+    def func(self, func: Callable) -> None:
         self._func = func
 
-    def set_energy(self, energy: float) -> None:
+    @energy.setter
+    def energy(self, energy: float) -> None:
         self._energy = energy
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/core/tag.py` & `big_thing_py-0.4.2.0/big_thing_py/core/argument.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,84 @@
 from big_thing_py.utils import *
 
 
-class MXTag:
-    def __init__(self, name: str):
-        self._name: str = name
-
-        if not check_valid_identifier(self._name):
-            raise MXValueError(
-                f'name cannot be empty & can only contain alphanumeric characters and underscores. name: {self._name}'
-            )
-
-    def __eq__(self, o: 'MXTag') -> bool:
-        name_check = o._name == self._name
+class MXArgument:
+    def __init__(self, name: str, type: MXType, bound: Tuple[float, float] = ()):
+        self._name = name
+        self._type = type
+        if self._type in [MXType.STRING, MXType.BINARY]:
+            self._min, self._max = -1, -1
+        else:
+            self._min, self._max = bound
+            if self._min >= self._max:
+                raise MXValueError('bound must be min < max')
+
+        if check_valid_identifier(self._name) == MXErrorCode.INVALID_DATA:
+            raise MXValueError(f'name cannot be empty & can only contain alphanumeric characters and underscores. name: {self._name}')
+        elif check_valid_identifier(self._name) == MXErrorCode.TOO_LONG_IDENTIFIER:
+            raise MXValueError(f'too long identifier. name: {self._name}, length: {len(self._name)}')
 
-        return isinstance(o, MXTag) and name_check
+        if self._type in [MXType.UNDEFINED, MXType.VOID] or isinstance(self._type, str):
+            raise MXValueError('type cannot be UNDEFINED or VOID or `str` type')
 
     def __str__(self) -> str:
         return self._name
 
-    def dict(self):
-        return {'name': self._name}
+    def __eq__(self, o: 'MXArgument') -> bool:
+        instance_check = isinstance(o, MXArgument)
+        name_check = o._name == self._name
+        type_check = o._type == self._type
+        min_check = o._min == self._min
+        max_check = o._max == self._max
+
+        return instance_check and name_check and type_check and min_check and max_check
+
+    def dict(self) -> dict:
+        return {'name': self._name, 'type': self._type.value, 'bound': {'min_value': self._min, 'max_value': self._max}}
 
     # ====================================
     #               _    _
     #              | |  | |
     #   __ _   ___ | |_ | |_   ___  _ __
     #  / _` | / _ \| __|| __| / _ \| '__|
     # | (_| ||  __/| |_ | |_ |  __/| |
     #  \__, | \___| \__| \__| \___||_|
     #   __/ |
     #  |___/
     # ====================================
 
-    def get_name(self):
+    @property
+    def name(self) -> str:
         return self._name
 
+    @property
+    def type(self) -> MXType:
+        return self._type
+
+    @property
+    def bound(self) -> Tuple[float, float]:
+        return self._min, self._max
+
     # ==================================
     #             _    _
     #            | |  | |
     #  ___   ___ | |_ | |_   ___  _ __
     # / __| / _ \| __|| __| / _ \| '__|
     # \__ \|  __/| |_ | |_ |  __/| |
     # |___/ \___| \__| \__| \___||_|
     # ==================================
 
-    def set_name(self, name):
+    @name.setter
+    def set_name(self, name: str):
         self._name = name
+
+    @type.setter
+    def type(self, type: MXType):
+        self._type = type
+
+    @bound.setter
+    def bound(self, bound: Tuple[float, float]):
+        if self._type in [MXType.STRING, MXType.BINARY]:
+            self._min, self._max = -1, -1
+        else:
+            self._min = bound[0]
+            self._max = bound[1]
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/super/super_function.py` & `big_thing_py-0.4.2.0/big_thing_py/super/super_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,17 +117,17 @@
 
         self._send_SM_SCHEDULE(subschedule_msg)
 
     def _select_target_sub_service_by_range_type(
         self, super_schedule_request: MXSuperScheduleRequest, single_select_func: Callable
     ) -> MXSubScheduleRequest:
         for sub_service_request in self._sub_service_request_list:
-            sub_service_request_range_type = sub_service_request._sub_service_type.get_range_type()
+            sub_service_request_range_type = sub_service_request._sub_service_type.range_type
             sub_service_request_key = make_sub_service_request_key(
-                sub_service_name=sub_service_request._sub_service_type.get_name(),
+                sub_service_name=sub_service_request._sub_service_type.name,
                 sub_service_request_order=sub_service_request._sub_service_request_order,
             )
             target_sub_service_request = super_schedule_request._sub_service_request_table[sub_service_request_key]
 
             if sub_service_request_range_type == MXRangeType.ALL:
                 for candidate_request in target_sub_service_request._candidate_request_list:
                     if candidate_request._status == MXScheduleStatus.CHECK:
@@ -227,39 +227,34 @@
             else:
                 return False
         else:
             return True
 
     def _check_confirm_parallel(self, super_schedule_request: MXSuperScheduleRequest) -> bool:
         self._check_parallel(super_schedule_request=super_schedule_request)
-        self._select_target_sub_service_by_range_type(
-            super_schedule_request=super_schedule_request, single_select_func=lambda x: x[0]
-        )
+        self._select_target_sub_service_by_range_type(super_schedule_request=super_schedule_request, single_select_func=lambda x: x[0])
         self._confirm_parallel(super_schedule_request=super_schedule_request)
 
         return True
 
     def _print_schedule_result(self, scenario_name: str, requester_middleware_name: str):
         schedule_result_string = '\n[SCHEDULE RESULT] ============================================\n'
-        super_request_key = make_super_request_key(
-            scenario_name=scenario_name, requester_middleware_name=requester_middleware_name
-        )
+        super_request_key = make_super_request_key(scenario_name=scenario_name, requester_middleware_name=requester_middleware_name)
         for super_k, super_execute_req in self._mapping_table.items():
             if super_k != super_request_key:
                 continue
             schedule_result_string += f'super_key: {super_k} -> super_service: {self._name}\n'
             for sub_k, sub_service_req in super_execute_req._sub_service_request_table.items():
                 schedule_result_string += (
                     ' ' * 4
-                    + f'sub_key: {sub_k} -> sub_service: {sub_service_req._sub_service_type.get_name()}|{sub_service_req._sub_service_request_order}\n'
+                    + f'sub_key: {sub_k} -> sub_service: {sub_service_req._sub_service_type.name}|{sub_service_req._sub_service_request_order}\n'
                 )
                 for target_req in sub_service_req._target_request_list:
                     schedule_result_string += (
-                        ' ' * 8
-                        + f'target: {target_req.trigger_msg.sub_service_name}|{target_req.trigger_msg.target_middleware_name}\n'
+                        ' ' * 8 + f'target: {target_req.trigger_msg.sub_service_name}|{target_req.trigger_msg.target_middleware_name}\n'
                     )
         schedule_result_string += '==============================================================\n'
         MXLOG_DEBUG(schedule_result_string, 'green')
 
     def _super_schedule_wrapper(
         self,
         super_schedule_request: MXSuperScheduleRequest,
@@ -283,29 +278,25 @@
         '''
         if not isinstance(super_schedule_request, MXSuperScheduleRequest):
             raise MXTypeError(f'[{get_current_function_name()}] Wrong Request type: {type(super_schedule_request)}')
 
         super_schedule_msg = super_schedule_request.trigger_msg
         requester_middleware_name = super_schedule_msg.requester_middleware_name
         scenario = super_schedule_msg.scenario
-        super_service_request_key = make_super_request_key(
-            scenario_name=scenario, requester_middleware_name=requester_middleware_name
-        )
+        super_service_request_key = make_super_request_key(scenario_name=scenario, requester_middleware_name=requester_middleware_name)
 
         MXLOG_DEBUG(f'[SUPER_SCHEDULE START] {self._name} by scenario {scenario}.', 'green')
 
         try:
             super_schedule_request._running = True
             self._schedule_running = True
             error = MXErrorCode.NO_ERROR
 
             # 후보 sub_service들에 대해서 스케쥴링을 진행한다.
-            super_schedule_request.generate_sub_service_schedule_request(
-                self._sub_service_request_list, hierarchical_service_table['functions']
-            )
+            super_schedule_request.generate_sub_service_schedule_request(self._sub_service_request_list, hierarchical_service_table['functions'])
 
             # func_timeout(timeout, self._check_confirm_parallel, args=(super_schedule_request, ))
             current_thread = threading.current_thread()
             self._run_with_timeout(
                 timeout=timeout,
                 func=self._check_confirm_parallel,
                 name=current_thread.name,
@@ -382,17 +373,15 @@
         sub_function_type_list과 sub_function_list는 독립적인 공간을 가진다.
         super_service 내부에 req함수 가 존재하여 사용자가 요청하고 싶은 sub_service이 명세되어있는데 여기서 명세되어지는
         sub_service은 실제 타겟 sub_service이 아닌 sub_service_type이다. 실제 sub_service 정보는 middleware로 부터 받은
         service_list를 통해 추출한다. 그리고 해당 정보는 super_service의 sub_service_list에 저장된다.
         '''
 
         if not isinstance(super_service_execute_request, MXSuperExecuteRequest):
-            raise MXTypeError(
-                f'[{get_current_function_name()}] Wrong Request type: {type(super_service_execute_request)}'
-            )
+            raise MXTypeError(f'[{get_current_function_name()}] Wrong Request type: {type(super_service_execute_request)}')
 
         super_execute_msg = super_service_execute_request.trigger_msg
         requester_middleware_name = super_execute_msg.requester_middleware_name
         scenario = super_execute_msg.scenario
 
         MXLOG_DEBUG(f'[SUPER_EXECUTE START] {self._name} by scenario {scenario}.', 'green')
 
@@ -400,23 +389,21 @@
             super_service_execute_request._running = True
             self._running = True
             error = MXErrorCode.NO_ERROR
 
             # super service argument check
             arguments = list(super_execute_msg.tuple_arguments())
             for i, (arg, real_arg) in enumerate(zip(self._arg_list, arguments)):
-                if arg.get_type() in [MXType.INTEGER, MXType.DOUBLE] and MXType.get(type(real_arg)) in [
+                if arg.get_type in [MXType.INTEGER, MXType.DOUBLE] and MXType.get(type(real_arg)) in [
                     MXType.INTEGER,
                     MXType.DOUBLE,
                 ]:
                     arguments[i] = float(real_arg)
-                elif arg.get_type() != MXType.get(type(real_arg)):
-                    raise Exception(
-                        f'Argument type is not matched: {arg.get_name()}: {arg.get_type()} != {MXType.get(real_arg)}'
-                    )
+                elif arg.get_type != MXType.get(type(real_arg)):
+                    raise Exception(f'Argument type is not matched: {arg.name}: {arg.get_type} != {MXType.get(real_arg)}')
 
             if self._timeout:
                 # self._return_value = func_timeout(self._timeout, self._func, args=(*tuple(arguments), ))
                 current_thread = threading.current_thread()
                 self._return_value = self._run_with_timeout(
                     timeout=self._timeout,
                     func=self._func,
@@ -501,17 +488,15 @@
         super_schedule_result_msg = MXSuperScheduleResultMessage(
             super_service_name=self._name,
             super_thing_name=self._thing_name,
             super_middleware_name=self._middleware_name,
             requester_middleware_name=super_schedule_msg.requester_middleware_name,
             scenario=super_schedule_msg.scenario,
         )
-        super_schedule_request = MXSuperScheduleRequest(
-            trigger_msg=super_schedule_msg, result_msg=super_schedule_result_msg
-        )
+        super_schedule_request = MXSuperScheduleRequest(trigger_msg=super_schedule_msg, result_msg=super_schedule_result_msg)
         super_service_request_key = make_super_request_key(
             scenario_name=super_schedule_msg.scenario,
             requester_middleware_name=super_schedule_msg.requester_middleware_name,
         )
         self._temporary_scheduling_table[super_service_request_key] = super_schedule_request
         super_schedule_request.timer_start()
 
@@ -525,17 +510,15 @@
                 timeout,
             ),
         )
         super_schedule_thread.start()
 
         return super_schedule_thread
 
-    def start_super_execute_thread(
-        self, super_execute_msg: MXSuperExecuteMessage, SUPER_SERVICE_REQUEST_KEY_TABLE: Dict[str, List[str]]
-    ) -> MXThread:
+    def start_super_execute_thread(self, super_execute_msg: MXSuperExecuteMessage, SUPER_SERVICE_REQUEST_KEY_TABLE: Dict[str, List[str]]) -> MXThread:
         super_service_request_key = make_super_request_key(
             scenario_name=super_execute_msg.scenario,
             requester_middleware_name=super_execute_msg.requester_middleware_name,
         )
         if super_service_request_key in self._temporary_scheduling_table:
             MXLOG_DEBUG(
                 f'[{get_current_function_name()}] Super request with key: {super_service_request_key} is currently in the scheduling phase!',
@@ -560,17 +543,15 @@
             scenario=super_execute_msg.scenario,
             return_type=self._return_type,
         )
         self._running_scenario_list.append(super_execute_msg.scenario)
         super_service_execute_request.timer_start()
 
         thread_name = f'{self._func.__name__}_{super_execute_msg.scenario}_thread'
-        super_execute_thread = MXThread(
-            target=self._super_execute_wrapper, name=thread_name, daemon=True, args=(super_service_execute_request,)
-        )
+        super_execute_thread = MXThread(target=self._super_execute_wrapper, name=thread_name, daemon=True, args=(super_service_execute_request,))
         super_execute_thread.start()
 
         sub_service_request_key_list = list(super_service_execute_request._sub_service_request_table)
         SUPER_SERVICE_REQUEST_KEY_TABLE[super_service_request_key] = sub_service_request_key_list
 
         return super_execute_thread
 
@@ -580,31 +561,31 @@
         sub_service_name: str,
         arg_list: Union[Tuple[MXArgument], Tuple],
         tag_list: List[MXTag],
         return_type: MXType,
         range_type: MXRangeType,
     ):
         mx_arg_list = [
-            arg
-            if isinstance(arg, MXArgument)
-            else MXArgument(name=f'DUMMY_ARG_{i}', bound=(-sys.maxsize - 1, sys.maxsize), type=MXType.get(type(arg)))
+            (
+                arg
+                if isinstance(arg, MXArgument)
+                else MXArgument(name=f'DUMMY_ARG_{i}', bound=(-sys.maxsize - 1, sys.maxsize), type=MXType.get(type(arg)))
+            )
             for i, arg in enumerate(arg_list)
         ]
         sub_service_request_order = len(self._sub_service_request_list)
         sub_service_type = MXFunction(
             name=sub_service_name,
             func=dummy_func(arg_list=mx_arg_list),
             return_type=return_type,
             arg_list=mx_arg_list,
             tag_list=tag_list,
             range_type=range_type,
         )
-        sub_service_request = MXSubServiceRequest(
-            sub_service_type=sub_service_type, sub_service_request_order=sub_service_request_order
-        )
+        sub_service_request = MXSubServiceRequest(sub_service_type=sub_service_type, sub_service_request_order=sub_service_request_order)
         self._add_sub_service_request(sub_service_request)
 
         MXLOG_DEBUG(f'sub_service: {sub_service_name}:{sub_service_request_order}', 'green')
         return True
 
     def put_subschedule_result(
         self,
@@ -616,35 +597,29 @@
             MXLOG_DEBUG(
                 f'Could not find key {super_service_request_key} in temporary_scheduling_table... This key is not mine!',
                 'yellow',
             )
             return False
 
         super_schedule_request = self._temporary_scheduling_table[super_service_request_key]
-        result = super_schedule_request.put_sub_service_schedule_result_msg(
-            sub_service_request_key, subschedule_result_msg
-        )
+        result = super_schedule_request.put_sub_service_schedule_result_msg(sub_service_request_key, subschedule_result_msg)
         return result
 
     def put_sub_service_execute_result(
         self,
         super_service_request_key: str,
         sub_service_request_key: str,
         sub_service_execute_result_msg: MXSubExecuteResultMessage,
     ) -> bool:
         if super_service_request_key not in self._mapping_table:
-            MXLOG_DEBUG(
-                f'Could not find key {super_service_request_key} in mapping_table... This key is not mine!', 'yellow'
-            )
+            MXLOG_DEBUG(f'Could not find key {super_service_request_key} in mapping_table... This key is not mine!', 'yellow')
             return False
 
         super_service_execute_request = self._mapping_table[super_service_request_key]
-        result = super_service_execute_request.put_sub_service_execute_result_msg(
-            sub_service_request_key, sub_service_execute_result_msg
-        )
+        result = super_service_execute_request.put_sub_service_execute_result_msg(sub_service_request_key, sub_service_execute_result_msg)
         return result
 
     def _send_SM_SCHEDULE(self, subschedule_msg: MXSubScheduleMessage) -> None:
         subschedule_mqtt_msg = subschedule_msg.mqtt_message()
         self._publish_queue.put(subschedule_mqtt_msg)
 
     def _send_SM_EXECUTE(self, sub_service_execute_msg: MXSubExecuteMessage) -> None:
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/super/super_mqtt_message.py` & `big_thing_py-0.4.2.0/big_thing_py/super/super_mqtt_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 class MXSuperRefreshMessage(MXMQTTSendMessage):
     def __init__(self, thing) -> None:
         from big_thing_py.core.thing import MXThing
 
         thing: MXThing = thing
 
         super().__init__()
-        self._protocol_type = MXProtocolType.Super.SM_REFRESH
-        self.topic = self._protocol_type.value % (thing.get_name())
+        self.protocol_type = MXProtocolType.Super.SM_REFRESH
+        self.topic = self.protocol_type.value % (thing.name)
         self.payload = EMPTY_JSON
 
 
 class MXSuperServiceListResultMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.Super.MS_RESULT_SERVICE_LIST
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg)
+        self.protocol_type = MXProtocolType.Super.MS_RESULT_SERVICE_LIST
         self.super_thing_name: str = self.topic.split('/')[3]
         self.service_list: List[dict] = self.payload['services']
 
 
 class MXSuperScheduleMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.Super.MS_SCHEDULE
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg)
+        self.protocol_type = MXProtocolType.Super.MS_SCHEDULE
 
         # topic
         self.super_service_name = self.topic.split('/')[2]
         self.super_thing_name = self.topic.split('/')[3]
         self.super_middleware_name = self.topic.split('/')[4]
         self.requester_middleware_name = self.topic.split('/')[5]
 
@@ -66,17 +66,17 @@
         super_thing_name: str,
         super_middleware_name: str,
         requester_middleware_name: str,
         scenario: str,
         error: MXErrorCode = MXErrorCode.UNDEFINED,
     ) -> None:
         super().__init__()
-        self._protocol_type = MXProtocolType.Super.SM_RESULT_SCHEDULE
+        self.protocol_type = MXProtocolType.Super.SM_RESULT_SCHEDULE
 
-        self.topic = self._protocol_type.value % (
+        self.topic = self.protocol_type.value % (
             super_service_name,
             super_thing_name,
             super_middleware_name,
             requester_middleware_name,
         )
         self.payload = dict(scenario=scenario, error=error.value)
 
@@ -95,15 +95,15 @@
         period: float = None,
         tag_list: List[str] = [],
         range_type: MXRangeType = None,
         request_ID: str = None,
         status: MXScheduleStatus = None,
     ) -> None:
         super().__init__()
-        self._protocol_type = MXProtocolType.Super.SM_SCHEDULE
+        self.protocol_type = MXProtocolType.Super.SM_SCHEDULE
 
         # topic
         self.sub_service_name = sub_service_name
         self.target_thing_name = target_thing_name
         self.target_middleware_name = target_middleware_name
 
         self.requester_middleware_name = requester_middleware_name
@@ -123,15 +123,15 @@
             self.request_ID = make_request_ID(
                 self.requester_middleware_name,
                 self.super_thing_name,
                 self.super_service_name,
                 self.sub_service_request_order,
             )
 
-        self.topic = self._protocol_type.value % (self.sub_service_name, self.target_middleware_name, self.request_ID)
+        self.topic = self.protocol_type.value % (self.sub_service_name, self.target_middleware_name, self.request_ID)
         self.payload = dict(
             scenario=self.scenario,
             period=self.period,
             status=self._status.value,
             tag_list=self.tag_list,
             range=self.range_type.value,
         )
@@ -151,17 +151,17 @@
             status=self._status.value,
             tag_list=self.tag_list,
             range=self.range_type.value,
         )
 
 
 class MXSubScheduleResultMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.Super.MS_RESULT_SCHEDULE
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg)
+        self.protocol_type = MXProtocolType.Super.MS_RESULT_SCHEDULE
 
         # topic
         self.sub_service_name = self.topic.split('/')[3]
         self.target_thing_name = self.topic.split('/')[4]
         self.target_middleware_name = self.topic.split('/')[5]
 
         self.request_ID = self.topic.split('/')[6]
@@ -173,17 +173,17 @@
         # payload
         self.scenario = self.payload['scenario']
         self.error = MXErrorCode.get(self.payload['error'])
         self.status = MXScheduleStatus.get(self.payload.get('status', None))  # 'check' or 'confirm'
 
 
 class MXSuperExecuteMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.Super.MS_EXECUTE
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg)
+        self.protocol_type = MXProtocolType.Super.MS_EXECUTE
 
         # topic
         self.super_service_name = self.topic.split('/')[2]
         self.super_thing_name = self.topic.split('/')[3]
         self.super_middleware_name = self.topic.split('/')[4]
         self.requester_middleware_name = self.topic.split('/')[5]
 
@@ -218,31 +218,29 @@
         requester_middleware_name: str,
         scenario: str,
         return_type: MXType,
         return_value: Union[int, float, bool, str] = None,
         error: MXErrorCode = MXErrorCode.UNDEFINED,
     ) -> None:
         super().__init__()
-        self._protocol_type = MXProtocolType.Super.SM_RESULT_EXECUTE
+        self.protocol_type = MXProtocolType.Super.SM_RESULT_EXECUTE
 
         # payload
         self.scenario = scenario
         self.return_type = return_type
         self.return_value = return_value
         self.error = error
 
-        self.topic = self._protocol_type.value % (
+        self.topic = self.protocol_type.value % (
             super_service_name,
             super_thing_name,
             super_middleware_name,
             requester_middleware_name,
         )
-        self.payload = dict(
-            scenario=scenario, return_type=return_type.value, return_value=return_value, error=error.value
-        )
+        self.payload = dict(scenario=scenario, return_type=return_type.value, return_value=return_value, error=error.value)
 
 
 class MXSubExecuteMessage(MXMQTTSendMessage):
     def __init__(
         self,
         sub_service_name: str,
         target_thing_name: str,
@@ -252,15 +250,15 @@
         super_service_name: str = None,
         sub_service_request_order: int = None,
         scenario: str = None,
         arguments: List[dict] = None,
         request_ID: str = None,
     ) -> None:
         super().__init__()
-        self._protocol_type = MXProtocolType.Super.SM_EXECUTE
+        self.protocol_type = MXProtocolType.Super.SM_EXECUTE
 
         # topic
         self.sub_service_name = sub_service_name
         self.target_thing_name = target_thing_name
         self.target_middleware_name = target_middleware_name
 
         self.requester_middleware_name = requester_middleware_name
@@ -277,15 +275,15 @@
             self.request_ID = make_request_ID(
                 self.requester_middleware_name,
                 self.super_thing_name,
                 self.super_service_name,
                 self.sub_service_request_order,
             )
 
-        self.topic = self._protocol_type.value % (self.sub_service_name, self.target_middleware_name, self.request_ID)
+        self.topic = self.protocol_type.value % (self.sub_service_name, self.target_middleware_name, self.request_ID)
         self.payload = dict(scenario=self.scenario, arguments=self._arguments)
 
     @property
     def arguments(self) -> dict:
         return self._arguments
 
     @arguments.setter
@@ -299,17 +297,17 @@
     # def json_arguments(self) -> List[dict]:
     #     self._arguments = sorted(self._arguments, key=lambda x: int(x['order']))
     #     json_arguments = [dict(order=arg['order'], value=arg['value']) for arg in self._arguments]
     #     return json_arguments
 
 
 class MXSubExecuteResultMessage(MXMQTTReceiveMessage):
-    def __init__(self, msg: mqtt.MQTTMessage) -> None:
-        super().__init__(msg)
-        self._protocol_type = MXProtocolType.Super.MS_RESULT_EXECUTE
+    def __init__(self, msg: MQTTMessage) -> None:
+        super().__init__(msg=msg)
+        self.protocol_type = MXProtocolType.Super.MS_RESULT_EXECUTE
 
         # topic
         self.sub_service_name = self.topic.split('/')[3]
         self.target_thing_name = self.topic.split('/')[4]
         self.target_middleware_name = self.topic.split('/')[5]
 
         self.request_ID = self.topic.split('/')[6]
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/super/super_request.py` & `big_thing_py-0.4.2.0/big_thing_py/super/super_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from big_thing_py.core.request import *
 from big_thing_py.super.super_mqtt_message import *
 from big_thing_py.core.function import *
 
 
 class MXSuperScheduleRequest(MXRequest):
-    def __init__(
-        self, trigger_msg: MXSuperScheduleMessage = None, result_msg: MXSuperScheduleResultMessage = None
-    ) -> None:
-        super().__init__(trigger_msg, result_msg)
+    def __init__(self, trigger_msg: MXSuperScheduleMessage = None, result_msg: MXSuperScheduleResultMessage = None) -> None:
+        super().__init__(trigger_msg=trigger_msg, result_msg=result_msg)
         self._action_type = MXActionType.SUPER_SCHEDULE
 
         self.trigger_msg: MXSuperScheduleMessage
         self.result_msg: MXSuperScheduleResultMessage
         self._check_duration: float = 0.0
         self._confirm_duration: float = 0.0
         self._status: MXScheduleStatus = MXScheduleStatus.INIT
@@ -50,17 +48,17 @@
             return False
 
         target_sub_service_request = self._sub_service_request_table[sub_service_request_key]
         for candidate_request in target_sub_service_request._candidate_request_list:
             thing_check = candidate_request.trigger_msg.target_thing_name == result_msg.target_thing_name
             middleware_check = candidate_request.trigger_msg.target_middleware_name == result_msg.target_middleware_name
             request_ID_check = candidate_request.trigger_msg.request_ID == result_msg.request_ID
-            status_check = (
-                result_msg.status == MXScheduleStatus.CONFIRM and candidate_request._status == MXScheduleStatus.SELECT
-            ) or (result_msg.status == MXScheduleStatus.CHECK)
+            status_check = (result_msg.status == MXScheduleStatus.CONFIRM and candidate_request._status == MXScheduleStatus.SELECT) or (
+                result_msg.status == MXScheduleStatus.CHECK
+            )
 
             if thing_check and middleware_check and request_ID_check and status_check:
                 candidate_request.put_result_msg(result_msg, timeout=timeout)
                 return True
         else:
             raise Exception(f'No sub_service {sub_service_request_key} found in _sub_service_request_table')
 
@@ -76,64 +74,60 @@
             )
             # TODO: 해당 로직 부분 분리하기
             # 미들웨어 마다 sub_service_request가 실행하고자 하는 sub_service이 존재하는 지 체크한다.
             target_sub_service = target_sub_service_request._sub_service_type
 
             candidate_middleware_name_list = []
             for function_service in hierarchical_function_service_table:
-                name_check = target_sub_service.get_name() == function_service.get_name()
-                if name_check and function_service.get_middleware_name() not in candidate_middleware_name_list:
-                    candidate_middleware_name_list.append(function_service.get_middleware_name())
-                    target_sub_service.set_middleware_name(function_service.get_middleware_name())
+                name_check = target_sub_service.name == function_service.name
+                if name_check and function_service.middleware_name not in candidate_middleware_name_list:
+                    candidate_middleware_name_list.append(function_service.middleware_name)
+                    target_sub_service.middleware_name = function_service.middleware_name
 
             candidate_request_list = []
             for middleware_name in candidate_middleware_name_list:
                 sub_service_schedule_msg = MXSubScheduleMessage(
-                    sub_service_name=target_sub_service.get_name(),
+                    sub_service_name=target_sub_service.name,
                     target_thing_name='SUPER',
                     target_middleware_name=middleware_name,
                     requester_middleware_name=self.trigger_msg.requester_middleware_name,
                     super_thing_name=self.trigger_msg.super_thing_name,
                     super_service_name=self.trigger_msg.super_service_name,
                     sub_service_request_order=target_sub_service_request._sub_service_request_order,
                     scenario=self.trigger_msg.scenario,
                     period=self.trigger_msg.period,
-                    tag_list=[dict(name=tag.get_name()) for tag in target_sub_service.get_tag_list()],
-                    range_type=target_sub_service.get_range_type(),
+                    tag_list=[dict(name=tag.name) for tag in target_sub_service.tag_list],
+                    range_type=target_sub_service.range_type,
                     request_ID=None,
                     status=MXScheduleStatus.INIT,
                 )
 
                 # NOTE:sub_service_request에 대한 부분이 미들웨어당 1개만 생성될 것으로 예상됨. len(candidate_request_list) == 1 ?
                 # TODO: _result_msg도 생성해서 넣어서 나중에 결과 토픽을 구독할 때 topic()으로 간단하게 사용할 수 있게 하면 좋을 것 같다.
                 sub_service_schedule_request = MXSubScheduleRequest(trigger_msg=sub_service_schedule_msg)
                 candidate_request_list.append(sub_service_schedule_request)
 
             target_sub_service_request._candidate_request_list = candidate_request_list
             sub_service_request_key = make_sub_service_request_key(
-                sub_service_name=target_sub_service.get_name(),
+                sub_service_name=target_sub_service.name,
                 sub_service_request_order=target_sub_service_request._sub_service_request_order,
             )
             self._sub_service_request_table[sub_service_request_key] = target_sub_service_request
 
             if len(target_sub_service_request._candidate_request_list) == 0:
                 for function_service in hierarchical_function_service_table:
-                    MXLOG_DEBUG(
-                        f'sub_service found! - {function_service.get_name()}|{function_service.get_thing_name()}|{function_service.get_middleware_name()}'
-                    )
+                    MXLOG_DEBUG(f'sub_service found! - {function_service.name}|{function_service.thing_name}|{function_service.middleware_name}')
                 raise Exception(
                     f'No candidate sub_service found in key:{sub_service_request_key} {self.trigger_msg.super_service_name} super service'
                 )
 
 
 class MXSuperExecuteRequest(MXRequest):
-    def __init__(
-        self, trigger_msg: MXSuperExecuteMessage = None, super_schedule_request: MXSuperScheduleRequest = None
-    ) -> None:
-        super().__init__(trigger_msg, None)
+    def __init__(self, trigger_msg: MXSuperExecuteMessage = None, super_schedule_request: MXSuperScheduleRequest = None) -> None:
+        super().__init__(trigger_msg=trigger_msg, result_msg=None)
         self._action_type = MXActionType.SUPER_EXECUTE
 
         self.trigger_msg: MXSuperExecuteMessage
         self.result_msg: MXSuperExecuteResultMessage
         self._running: bool = False
 
         # scheduling이 끝나면 해당 scenario에 대해 어떤 sub_service_type에 대해 thing을 선택할 것인지 정해진다.
@@ -152,49 +146,41 @@
 
     def is_completed(self):
         if self.result_msg:
             return True
         else:
             return False
 
-    def put_sub_service_execute_result_msg(
-        self, sub_service_request_key: str, result_msg: MXSubExecuteResultMessage, timeout: float = None
-    ) -> bool:
+    def put_sub_service_execute_result_msg(self, sub_service_request_key: str, result_msg: MXSubExecuteResultMessage, timeout: float = None) -> bool:
         if sub_service_request_key not in self._sub_service_request_table:
             MXLOG_DEBUG(
                 f'Could not find key {sub_service_request_key} in sub_service_request_table... This key is not mine!',
                 'yellow',
             )
             return False
 
         target_sub_service_request = self._sub_service_request_table[sub_service_request_key]
         for target_request in target_sub_service_request._target_request_list:
             target_thing_check = target_request.trigger_msg.target_thing_name == result_msg.target_thing_name
-            target_middleware_check = (
-                target_request.trigger_msg.target_middleware_name == result_msg.target_middleware_name
-            )
+            target_middleware_check = target_request.trigger_msg.target_middleware_name == result_msg.target_middleware_name
             request_ID_check = target_request.trigger_msg.request_ID == result_msg.request_ID
             if target_thing_check and target_middleware_check and request_ID_check:
                 target_request.put_result_msg(result_msg, timeout=timeout)
                 return True
         else:
             raise Exception(f'No sub_service {sub_service_request_key} found in _sub_service_request_table')
 
-    def get_sub_service_execute_result_msg_list(
-        self, sub_service_request_key: str, timeout: float = None
-    ) -> List[MXSubExecuteResultMessage]:
+    def get_sub_service_execute_result_msg_list(self, sub_service_request_key: str, timeout: float = None) -> List[MXSubExecuteResultMessage]:
         result_msg_list = []
         target_sub_service_request = self._sub_service_request_table[sub_service_request_key]
         for target_request in target_sub_service_request._target_request_list:
             result_msg_list.append(target_request.get_result_msg(timeout=timeout))
         return result_msg_list
 
-    def generate_sub_service_execute_request_list(
-        self, super_schedule_request: 'MXSuperScheduleRequest' = None
-    ) -> 'MXSuperExecuteRequest':
+    def generate_sub_service_execute_request_list(self, super_schedule_request: 'MXSuperScheduleRequest' = None) -> 'MXSuperExecuteRequest':
         # schedule 단계에서 MXSuperExecuteRequest를 생성한다.
         for sub_service_request_key, sub_service_request in super_schedule_request._sub_service_request_table.items():
             self._sub_service_request_table[sub_service_request_key] = MXSubServiceRequest(
                 sub_service_type=sub_service_request._sub_service_type,
                 sub_service_request_order=sub_service_request._sub_service_request_order,
                 candidate_request_list=sub_service_request._candidate_request_list,
             )
@@ -203,18 +189,16 @@
                 if candidate_request._status == MXScheduleStatus.CONFIRM:
                     target_request_list.append(to_sub_service_execute_request(candidate_request))
             self._sub_service_request_table[sub_service_request_key]._target_request_list = target_request_list
         return self
 
 
 class MXSubScheduleRequest(MXRequest):
-    def __init__(
-        self, trigger_msg: MXSubScheduleMessage = None, result_mqtt_msg: MXSubScheduleResultMessage = None
-    ) -> None:
-        super().__init__(trigger_msg, result_mqtt_msg)
+    def __init__(self, trigger_msg: MXSubScheduleMessage = None, result_msg: MXSubScheduleResultMessage = None) -> None:
+        super().__init__(trigger_msg=trigger_msg, result_msg=result_msg)
         self._action_type = MXActionType.SUB_SCHEDULE
 
         self.trigger_msg: MXSubScheduleMessage
         self.result_msg: MXSubScheduleResultMessage
         self._status: MXScheduleStatus = MXScheduleStatus.INIT
         self._result_queue = Queue()
 
@@ -237,18 +221,16 @@
         try:
             return self._result_queue.get(timeout=timeout)
         except Empty:
             raise FunctionTimedOut
 
 
 class MXSubExecuteRequest(MXRequest):
-    def __init__(
-        self, trigger_msg: MXSubExecuteMessage = None, result_mqtt_msg: MXSubExecuteResultMessage = None
-    ) -> None:
-        super().__init__(trigger_msg, result_mqtt_msg)
+    def __init__(self, trigger_msg: MXSubExecuteMessage = None, result_msg: MXSubExecuteResultMessage = None) -> None:
+        super().__init__(trigger_msg=trigger_msg, result_msg=result_msg)
         self._action_type = MXActionType.SUB_EXECUTE
 
         self.trigger_msg: MXSubExecuteMessage
         self.result_msg: MXSubExecuteResultMessage
         self._result_queue = Queue()
 
     def __getstate__(self):
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/super_thing.py` & `big_thing_py-0.4.2.0/big_thing_py/super_thing.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,54 +14,58 @@
     #      ...
     # }
     _SUPER_SERVICE_REQUEST_KEY_TABLE: Dict[str, List[str]] = dict()
 
     def __init__(
         self,
         name: str = DEFAULT_NAME,
+        desc: str = '',
+        version: str = sdk_version(),
         service_list: List[MXService] = [],
         alive_cycle: float = 60,
         is_super: bool = True,
         is_parallel: bool = True,
         ip: str = '127.0.0.1',
         port: int = 1883,
         ssl_ca_path: str = '',
-        ssl_enable: bool = False,
+        ssl_cert_path: str = '',
+        ssl_key_path: str = '',
         log_name: str = '',
         log_enable: bool = True,
         log_mode: MXPrintMode = MXPrintMode.ABBR,
         append_mac_address: bool = True,
         refresh_cycle: float = 30,
     ):
         self._global_service_table: Dict[str, Union[List[MXFunction], List[MXValue]]] = dict(values=[], functions=[])
         self._SUPER_SERVICE_REQUEST_KEY_TABLE = dict()
 
         super().__init__(
-            name,
-            service_list,
-            alive_cycle,
-            is_super,
-            is_parallel,
-            ip,
-            port,
-            ssl_ca_path,
-            ssl_enable,
-            log_name,
-            log_enable,
-            log_mode,
-            append_mac_address,
+            name=name,
+            desc=desc,
+            version=version,
+            service_list=service_list,
+            alive_cycle=alive_cycle,
+            is_super=is_super,
+            is_parallel=is_parallel,
+            ip=ip,
+            port=port,
+            ssl_ca_path=ssl_ca_path,
+            ssl_cert_path=ssl_cert_path,
+            ssl_key_path=ssl_key_path,
+            log_name=log_name,
+            log_enable=log_enable,
+            log_mode=log_mode,
+            append_mac_address=append_mac_address,
         )
 
         self._refresh_cycle = refresh_cycle
 
         self._last_refresh_time = 0
 
-        self._function_list: List[MXSuperFunction] = self._function_list
-
-        self._thread_func_list += [
+        self._task_func_list += [
             self._refresh_thread_func,
         ]
 
     def __eq__(self, o: 'MXSuperThing'):
         instance_check = isinstance(o, MXSuperThing)
         refresh_cycle_check = self._refresh_cycle == o._refresh_cycle
 
@@ -78,37 +82,37 @@
 
     def __setstate__(self, state):
         super().__setstate__(state)
 
         self._refresh_cycle = state['_refresh_cycle']
 
         self._last_refresh_time = 0
-        self._thread_func_list = self._thread_func_list + [
+        self._task_func_list = self._task_func_list + [
             self._refresh_thread_func,
         ]
 
     @override
-    def setup(self, avahi_enable=True) -> 'MXSuperThing':
+    def _setup(self) -> 'MXSuperThing':
         self._init_logger()
         self._extract_sub_service_request_info()
-        return super().setup(avahi_enable)
+        return super()._setup()
 
     # ===========================================================================================
     #  _    _                             _    __                      _    _
     # | |  | |                           | |  / _|                    | |  (_)
     # | |_ | |__   _ __   ___   __ _   __| | | |_  _   _  _ __    ___ | |_  _   ___   _ __   ___
     # | __|| '_ \ | '__| / _ \ / _` | / _` | |  _|| | | || '_ \  / __|| __|| | / _ \ | '_ \ / __|
     # | |_ | | | || |   |  __/| (_| || (_| | | |  | |_| || | | || (__ | |_ | || (_) || | | |\__ \
     #  \__||_| |_||_|    \___| \__,_| \__,_| |_|   \__,_||_| |_| \___| \__||_| \___/ |_| |_||___/
     # ===========================================================================================
 
     def _refresh_thread_func(self, stop_event: Event):
         try:
             while not stop_event.wait(THREAD_TIME_OUT):
-                if self._is_registered:
+                if self._is_registered.is_set():
                     if (get_current_time() - self._last_refresh_time) > self._refresh_cycle:
                         self._send_SM_REFRESH()
                         self._last_refresh_time = get_current_time()
                         # time.sleep(self._refresh_cycle / 2)
 
         except Exception as e:
             stop_event.set()
@@ -142,18 +146,17 @@
     # | | | || (_| || | | || (_| || ||  __/ | |  | |\ \/' /  | |    | |   | | | | | ||  __/\__ \\__ \| (_| || (_| ||  __/
     # |_| |_| \__,_||_| |_| \__,_||_| \___| \_|  |_/ \_/\_\  \_/    \_/   |_| |_| |_| \___||___/|___/ \__,_| \__, | \___|
     #                                                                                                         __/ |
     #                                                                                                        |___/
     # ====================================================================================================================
 
     @override
-    def _handle_mqtt_message(self, msg: mqtt.MQTTMessage) -> bool:
+    def _handle_mqtt_message(self, msg: MQTTMessage) -> bool:
         topic_string = decode_MQTT_message(msg)[0]
         protocol = MXProtocolType.get(topic_string)
-        msg.timestamp = time.time()
 
         if protocol == MXProtocolType.Super.MS_RESULT_SCHEDULE:
             rc = self._handle_MS_RESULT_SCHEDULE(msg)
         elif protocol == MXProtocolType.Super.MS_RESULT_EXECUTE:
             rc = self._handle_MS_RESULT_EXECUTE(msg)
         elif protocol == MXProtocolType.Super.MS_RESULT_SERVICE_LIST:
             rc = self._handle_MS_RESULT_SERVICE_LIST(msg)
@@ -163,15 +166,15 @@
             rc = self._handle_MS_EXECUTE(msg)
         elif protocol == MXProtocolType.WebClient.ME_NOTIFY_CHANGE:
             rc = self._handle_ME_NOTIFY(msg)
 
         elif protocol == MXProtocolType.Base.MT_RESULT_REGISTER:
             rc = self._handle_MT_RESULT_REGISTER(msg)
         elif protocol == MXProtocolType.Base.MT_RESULT_UNREGISTER:
-            rc = self._handle_MT_RESULT_UNREGISTER(msg)
+            rc = self._handle_MT_RESULT_UNREGISTER(msg, target_thing=self._thing_data)
         elif protocol == MXProtocolType.Base.MT_RESULT_BINARY_VALUE:
             MXLOG_DEBUG(f'[{get_current_function_name()}] Not permitted topic! topic: {topic_string}')
             return False
         elif protocol == MXProtocolType.Base.MT_EXECUTE:
             MXLOG_DEBUG(f'[{get_current_function_name()}] Not permitted topic! topic: {topic_string}')
             return False
         else:
@@ -189,15 +192,15 @@
     # |  \/  |/  ___|
     # | .  . |\ `--.
     # | |\/| | `--. \
     # | |  | |/\__/ /
     # \_|  |_/\____/
     # ================
 
-    def _handle_MS_SCHEDULE(self, msg: mqtt.MQTTMessage) -> bool:
+    def _handle_MS_SCHEDULE(self, msg: MQTTMessage) -> bool:
         super_schedule_msg = MXSuperScheduleMessage(msg)
         target_super_service = self._get_function(super_schedule_msg.super_service_name)
 
         if not target_super_service:
             MXLOG_DEBUG(
                 f'[{get_current_function_name()}] Super Service {super_schedule_msg.super_service_name} does not exist...',
                 'red',
@@ -216,30 +219,28 @@
             )
             return False
         if super_schedule_msg.topic_error or super_schedule_msg.payload_error:
             MXLOG_DEBUG(f'[{get_current_function_name()}] super_schedule_msg Message has error!', 'red')
             return False
         if not self._check_super_service_exist(target_super_service):
             MXLOG_DEBUG(
-                f'[{get_current_function_name()}] Super Service {target_super_service.get_name()} does not exist...',
+                f'[{get_current_function_name()}] Super Service {target_super_service.name} does not exist...',
                 'red',
             )
             return False
 
-        schedule_thread = target_super_service.start_super_schedule_thread(
-            super_schedule_msg, self._global_service_table, timeout=1000
-        )
+        schedule_thread = target_super_service.start_super_schedule_thread(super_schedule_msg, self._global_service_table, timeout=1000)
         if not schedule_thread:
             return False
         elif schedule_thread.is_alive():
             return True
         else:
             return False
 
-    def _handle_MS_EXECUTE(self, msg: mqtt.MQTTMessage) -> bool:
+    def _handle_MS_EXECUTE(self, msg: MQTTMessage) -> bool:
         super_execute_msg = MXSuperExecuteMessage(msg)
         target_super_service = self._get_function(super_execute_msg.super_service_name)
 
         if not target_super_service:
             MXLOG_DEBUG(
                 f'[{get_current_function_name()}] Super Service {super_execute_msg.super_service_name} does not exist...',
                 'red',
@@ -258,34 +259,32 @@
             )
             return False
         if super_execute_msg.topic_error or super_execute_msg.payload_error:
             MXLOG_DEBUG(f'[{get_current_function_name()}] super_execute_msg Message has error!', 'red')
             return False
 
         # 중복된 시나리오로부터 온 실행 요청이면 -4 에러코드를 보낸다.
-        if super_execute_msg.scenario in target_super_service.get_running_scenario_list():
+        if super_execute_msg.scenario in target_super_service.running_scenario_list:
             target_super_service._send_SM_RESULT_EXECUTE(
                 super_service_name=super_execute_msg.super_service_name,
                 super_thing_name=super_execute_msg.super_thing_name,
                 super_middleware_name=super_execute_msg.super_middleware_name,
                 requester_middleware_name=super_execute_msg.requester_middleware_name,
                 scenario=super_execute_msg.scenario,
                 error=MXErrorCode.DUPLICATE,
             )
             return True
 
-        super_execute_thread = target_super_service.start_super_execute_thread(
-            super_execute_msg, self._SUPER_SERVICE_REQUEST_KEY_TABLE
-        )
+        super_execute_thread = target_super_service.start_super_execute_thread(super_execute_msg, self._SUPER_SERVICE_REQUEST_KEY_TABLE)
         if not super_execute_thread:
             return False
         else:
             return True
 
-    def _handle_MS_RESULT_SCHEDULE(self, msg: mqtt.MQTTMessage) -> bool:
+    def _handle_MS_RESULT_SCHEDULE(self, msg: MQTTMessage) -> bool:
         subschedule_result_msg = MXSubScheduleResultMessage(msg)
         subschedule_result_msg.set_timestamp()
         super_service_request_key = make_super_request_key(
             scenario_name=subschedule_result_msg.scenario,
             requester_middleware_name=subschedule_result_msg.requester_middleware_name,
         )
         sub_service_request_key = make_sub_service_request_key(
@@ -297,20 +296,18 @@
         if not target_super_service:
             MXLOG_DEBUG(
                 f'[{get_current_function_name()}] Super Service {subschedule_result_msg.super_service_name} does not exist...',
                 'yellow',
             )
             return False
 
-        result = target_super_service.put_subschedule_result(
-            super_service_request_key, sub_service_request_key, subschedule_result_msg
-        )
+        result = target_super_service.put_subschedule_result(super_service_request_key, sub_service_request_key, subschedule_result_msg)
         return result
 
-    def _handle_MS_RESULT_EXECUTE(self, msg: mqtt.MQTTMessage) -> bool:
+    def _handle_MS_RESULT_EXECUTE(self, msg: MQTTMessage) -> bool:
         sub_service_execute_result_msg = MXSubExecuteResultMessage(msg)
         sub_service_execute_result_msg.set_timestamp()
         super_service_request_key = make_super_request_key(
             scenario_name=sub_service_execute_result_msg.scenario,
             requester_middleware_name=sub_service_execute_result_msg.requester_middleware_name,
         )
         sub_service_request_key = make_sub_service_request_key(
@@ -327,15 +324,15 @@
             return False
 
         result = target_super_service.put_sub_service_execute_result(
             super_service_request_key, sub_service_request_key, sub_service_execute_result_msg
         )
         return result
 
-    def _handle_MS_RESULT_SERVICE_LIST(self, msg: mqtt.MQTTMessage) -> bool:
+    def _handle_MS_RESULT_SERVICE_LIST(self, msg: MQTTMessage) -> bool:
         try:
             service_list = MXSuperServiceListResultMessage(msg)
             service_list.set_timestamp()
 
             for middleware in service_list.service_list:
                 hierarchy_type = middleware['hierarchy']
                 if not hierarchy_type in ['local', 'child']:
@@ -356,17 +353,15 @@
                     is_super = thing['is_super']
                     alive_cycle = thing['alive_cycle']
 
                     # value 정보를 추출
                     value_service_list = self._extract_value_info(thing=thing, middleware_name=middleware_name)
                     self._global_service_table['values'].extend(value_service_list)
 
-                    function_service_list = self._extract_function_info(
-                        thing_info=thing, middleware_name=middleware_name
-                    )
+                    function_service_list = self._extract_function_info(thing_info=thing, middleware_name=middleware_name)
                     self._global_service_table['functions'].extend(function_service_list)
 
             self._last_refresh_time = get_current_time()
             return True
         except KeyError as e:
             print_error(e)
             MXLOG_DEBUG(f'[{get_current_function_name()}] KeyError', 'red')
@@ -385,15 +380,15 @@
     #  |  \/  | |  ____|
     #  | \  / | | |__
     #  | |\/| | |  __|
     #  | |  | | | |____
     #  |_|  |_| |______|
     # ===================
 
-    def _handle_ME_NOTIFY(self, msg: mqtt.MQTTMessage):
+    def _handle_ME_NOTIFY(self, msg: MQTTMessage):
         notify_msg = MXNotifyMessage(msg)
         notify_msg.set_timestamp()
         self._send_SM_REFRESH()
 
     # ================
     #  _____ ___  ___
     # /  ___||  \/  |
@@ -423,46 +418,44 @@
 
     def generate_super_refresh_message(self) -> MXSuperRefreshMessage:
         super_refresh_msg = MXSuperRefreshMessage(self)
         return super_refresh_msg
 
     @override
     def _get_function(self, function_name: str) -> MXSuperFunction:
-        for function in self._function_list:
-            if function.get_name() == function_name:
+        for function in self.function_list:
+            if function.name == function_name:
                 return function
 
     @override
     def _subscribe_init_topic_list(self):
         super()._subscribe_init_topic_list()
 
         topic_list = [MXProtocolType.Super.MS_RESULT_SERVICE_LIST.value % "#"]
 
         for topic in topic_list:
             self._subscribe(topic)
 
     @override
     def _subscribe_service_topic_list(self):
-        for function in self._function_list:
+        for function in self.function_list:
             # Super Schedule, Super Execute에 필요한 토픽들을 미리 구독을 해놓는다.
             topic_list = [
-                MXProtocolType.Super.MS_SCHEDULE.value % (function.get_name(), self._name, self._middleware_name, '#'),
+                MXProtocolType.Super.MS_SCHEDULE.value % (function.name, self._name, self._middleware_name, '#'),
                 MXProtocolType.Super.MS_RESULT_SCHEDULE.value % ('+', '+', '#'),
-                MXProtocolType.Super.MS_EXECUTE.value % (function.get_name(), self._name, self._middleware_name, '#'),
+                MXProtocolType.Super.MS_EXECUTE.value % (function.name, self._name, self._middleware_name, '#'),
                 MXProtocolType.Super.MS_RESULT_EXECUTE.value % ('+', '+', '#'),
             ]
 
             for topic in topic_list:
                 self._subscribe(topic)
 
     def _request_sub_service_execute(self, sub_service_execute_request: MXSubExecuteRequest) -> None:
         if not isinstance(sub_service_execute_request, MXSubExecuteRequest):
-            raise MXTypeError(
-                f'[{get_current_function_name()}] Invalid type of sub_service_execute_request: {type(sub_service_execute_request)}'
-            )
+            raise MXTypeError(f'[{get_current_function_name()}] Invalid type of sub_service_execute_request: {type(sub_service_execute_request)}')
 
         sub_service_execute_msg = sub_service_execute_request.trigger_msg
         self._send_SM_EXECUTE(sub_service_execute_msg)
 
     # 하나의 sub_service_request에 있는 sub_service_execute_request들을 병렬로 실행한다.
     def _sub_service_execute_parallel(
         self, sub_service_execute_request_list: List[MXSubExecuteRequest], arg_list: List[Union[int, float, str, bool]]
@@ -501,23 +494,23 @@
                 'cyan',
             )
 
         return result_list
 
     def _get_sub_service_from_global_service_table(self, sub_service_name: str) -> MXFunction:
         for function in self._global_service_table['functions']:
-            if function.get_name() == sub_service_name:
+            if function.name == sub_service_name:
                 return function
         return None
 
     def _check_sub_service_callable(self, sub_service_name: str, return_type: MXType):
         global_sub_service = self._get_sub_service_from_global_service_table(sub_service_name)
         if not global_sub_service:
             return False
-        if not global_sub_service.get_return_type() == return_type:
+        if not global_sub_service.return_type == return_type:
             return False
 
         return True
 
     def _check_req_valid(
         self,
         sub_service_name: str,
@@ -540,37 +533,33 @@
         elif service_type == MXServiceType.VALUE and return_type == MXType.VOID:
             raise MXTypeError(f'Value service cannot have a return_type of void')
         if not range_type in [MXRangeType.SINGLE, MXRangeType.ALL]:
             raise MXTypeError(f'Invalid range_type: {range_type}')
 
         return True
 
-    def _check_req_return_type(
-        self, sub_service_return_type: MXType, req_return_type: MXType, service_type: MXServiceType
-    ):
+    def _check_req_return_type(self, sub_service_return_type: MXType, req_return_type: MXType, service_type: MXServiceType):
         if req_return_type in [MXType.INTEGER, MXType.DOUBLE] and sub_service_return_type in [
             MXType.INTEGER,
             MXType.DOUBLE,
         ]:
             return True
         elif req_return_type == MXType.VOID and service_type == MXServiceType.VALUE:
-            raise MXTypeError(
-                f'Not matched return_type. Value service cannot have a return_type of void: {sub_service_return_type}'
-            )
+            raise MXTypeError(f'Not matched return_type. Value service cannot have a return_type of void: {sub_service_return_type}')
         elif req_return_type != sub_service_return_type:
             raise MXTypeError(f'Not matched return_type: {sub_service_return_type} != {req_return_type}')
 
         return True
 
     def _check_super_service_exist(self, super_service: MXSuperFunction):
         return all(
             [
                 self._check_sub_service_callable(
-                    sub_service_request._sub_service_type.get_name(),
-                    sub_service_request._sub_service_type.get_return_type(),
+                    sub_service_request._sub_service_type.name,
+                    sub_service_request._sub_service_type.return_type,
                 )
                 for sub_service_request in super_service._sub_service_request_list
             ]
         )
 
     def req(
         self,
@@ -615,20 +604,18 @@
                 range_type=range_type,
             )
             return []
         else:
             if not self._check_sub_service_callable(sub_service_name, return_type):
                 MXLOG_DEBUG(f'sub_service {sub_service_name} is not callable', 'red')
                 return False
-            if not self._compare_arg_list(target_sub_service.get_arg_list(), list(arg_list)):
+            if not self._compare_arg_list(target_sub_service.arg_list, list(arg_list)):
                 MXLOG_DEBUG(f'Not matched arg_list')
                 return False
-            if not self._check_req_return_type(
-                target_sub_service.get_return_type(), req_return_type=return_type, service_type=service_type
-            ):
+            if not self._check_req_return_type(target_sub_service.return_type, req_return_type=return_type, service_type=service_type):
                 MXLOG_DEBUG(f'Not matched return_type')
                 return False
 
             current_thread = threading.current_thread()
             scenario_name = current_thread.user_data['scenario']
             requester_middleware_name = current_thread.user_data['requester_middleware']
             # super_service_request_key = scenario_name@requester_middleware_name
@@ -645,17 +632,15 @@
                 f'[DEBUG] after pop SUPER_SERVICE_REQUEST_KEY_TABLE: \n{dict_to_json_string(self._SUPER_SERVICE_REQUEST_KEY_TABLE, pretty=True)}'
                 f'\n super_service_request_key: {super_service_request_key} '
             )
             if len(sub_service_request_key_list) == 0:
                 self._SUPER_SERVICE_REQUEST_KEY_TABLE.pop(super_service_request_key)
 
             super_service_execute_request = target_super_service._mapping_table[super_service_request_key]
-            sub_service_execute_request_list = super_service_execute_request._sub_service_request_table[
-                sub_service_request_key
-            ]._target_request_list
+            sub_service_execute_request_list = super_service_execute_request._sub_service_request_table[sub_service_request_key]._target_request_list
 
             result_list = self._sub_service_execute_parallel(sub_service_execute_request_list, arg_list)
             return result_list
 
     # TODO: implement this
     def r(self, line: str = None, *arg_list) -> Union[List[dict], bool]:
         super_service_name = get_upper_function_name()
@@ -677,19 +662,19 @@
             if '$' in arg:
                 index = int(arg[1:])
                 arguments[i] = arg_list[index - 1]
 
         arguments = tuple(arguments)
 
     def _extract_sub_service_request_info(self) -> None:
-        for function in self._function_list:
-            if self._is_super and not function.get_is_scanned():
-                arg_list = function.get_arg_list()
+        for function in self.function_list:
+            if self.is_super and not function.get_is_scanned():
+                arg_list = function.arg_list
                 try:
-                    MXLOG_DEBUG(f'Detect super service: {function.get_name()}', 'green')
+                    MXLOG_DEBUG(f'Detect super service: {function.name}', 'green')
                     function._func(*tuple(arg_list))
                 except MXError as e:
                     # req를 실행하다가 MySSIXError와 관련된 에러가 발생한다는 것은 req명세가 잘못
                     # 되었다는 것을 의미한다. 만약 MySSIXError에러가 아닌 다른 예외가 발생한 경우,
                     # super service안에 있는 코드 중, req() 코드 부분이 아닌 코드에 의한 예외이므로
                     # 정상적으로 req()에 대한 정보를 추출한 것이다.
                     raise e
@@ -764,22 +749,23 @@
     # | (_| ||  __/| |_ | |_ |  __/| |
     #  \__, | \___| \__| \__| \___||_|
     #   __/ |
     #  |___/
     # ====================================
 
     @override
-    def get_function_list(self) -> List[MXSuperFunction]:
-        return self._function_list
+    @property
+    def function_list(self) -> List[MXSuperFunction]:
+        return sorted([service for service in self._service_list if isinstance(service, MXFunction)], key=lambda x: x.name)
 
     # ==================================
     #             _    _
     #            | |  | |
     #  ___   ___ | |_ | |_   ___  _ __
     # / __| / _ \| __|| __| / _ \| '__|
     # \__ \|  __/| |_ | |_ |  __/| |
     # |___/ \___| \__| \__| \___||_|
     # ==================================
 
     @override
     def set_function_list(self, function_list: List[MXSuperFunction]) -> None:
-        self._function_list = function_list
+        self.function_list = function_list
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/utils/common_util.py` & `big_thing_py-0.4.2.0/big_thing_py/utils/common_util.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import copy
 import random
 from pathlib import Path
 import getmac
 import re
 import sys
 import typing
+import importlib.metadata
 
 
 def static_vars(**kwargs):
     def decorate(func):
         for k in kwargs:
             setattr(func, k, kwargs[k])
         return func
@@ -59,14 +60,25 @@
     elif step > 1:
         co_name = get_upper_function_name(step - 1, frame.f_back)
     else:
         co_name = 'too many steps... return MAX upper function name'
     return co_name
 
 
+def get_function_return_type(func: Callable, to_mxtype: bool = False) -> Union[MXType, str]:
+    return_type = inspect.signature(func).return_annotation
+    if return_type is inspect.Signature.empty:
+        raise MXNotSupportedError('Return type is not defined!!!')
+
+    if to_mxtype:
+        return MXType.get(return_type)
+    else:
+        return return_type
+
+
 def get_mac_address(interface: str = None) -> str:
     mac_address = getmac.get_mac_address(interface)
 
     if mac_address:
         mac_address = mac_address.replace(':', '').upper()
         return mac_address
     else:
@@ -133,24 +145,24 @@
             return MXType.UNDEFINED
         else:
             raise MXNotSupportedError('Unexpected MXType type!!!')
     elif in_type == None or type(in_type) == type(None):
         return MXType.VOID
 
 
-def json_file_read(path: str) -> Union[dict, bool]:
+def json_file_read(path: str, mode: str = 'r') -> Union[dict, bool]:
     try:
-        with open(path, 'r') as f:
+        with open(path, mode) as f:
             return json.load(f)
     except FileNotFoundError:
         return False
 
 
-def json_file_write(path: str, data: Union[str, dict], indent: int = 4) -> None:
-    with open(path, 'w') as f:
+def json_file_write(path: str, data: Union[str, dict], mode: str = 'w', indent: int = 4) -> None:
+    with open(path, mode) as f:
         if isinstance(data, (dict, str)):
             json.dump(data, f, indent=indent)
         else:
             raise Exception(f'common_util.json_file_write: data type error - {type(data)}')
 
 
 def get_project_root(project_name: str = 'big-thing-py') -> Path:
@@ -158,17 +170,23 @@
     while True:
         if str(start_path).split('/')[-1] == project_name:
             return str(start_path)
         else:
             start_path = start_path.parent
 
 
-def check_valid_identifier(identifier: str) -> bool:
-    pattern = r'^[a-zA-Z0-9_]*$'
-    return bool(re.match(pattern, identifier))
+def check_valid_identifier(identifier: str) -> MXErrorCode:
+    pattern = r'^[_a-zA-Z0-9]*$'
+
+    if len(identifier) >= 256:
+        return MXErrorCode.TOO_LONG_IDENTIFIER
+    elif not bool(re.match(pattern, identifier)):
+        return MXErrorCode.INVALID_DATA
+    else:
+        return MXErrorCode.NO_ERROR
 
 
 def convert_special_char(char: str) -> str:
     # conversion_dict = {
     #     ' ': 'space',
     #     '!': 'exclamation_mark',
     #     '"': 'double_quote',
@@ -261,19 +279,29 @@
         return host_ip
     elif not all([(0 <= int(ip_token) <= 255) for ip_token in ip_list]) or len(ip_list) != 4:
         raise Exception('wrong ip format')
     else:
         return url
 
 
-def check_python_version():
-    if sys.version_info[0] <= 3 and sys.version_info[1] < 6:
-        raise Exception(
-            'Avahi feature is not supported on python3.6<=. try python3.7 or higher. or disable avahi feature. (avahi_enable=False)'
-        )
+def get_local_ip() -> str:
+    try:
+        with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
+            s.connect(('192.168.0.1', 80))
+            local_ip = s.getsockname()[0]
+            return local_ip
+    except Exception as e:
+        return f"Error occurred: {e}"
+
+
+def check_python_version() -> bool:
+    if not (sys.version_info[0] >= 3 and sys.version_info[1] > 6):
+        return False
+
+    return True
 
 
 def is_valid_ip_address(ip_address: str) -> bool:
     if ip_address:
         octets = ip_address.split('.')
     else:
         return False
@@ -312,9 +340,34 @@
 def dummy_func(arg_list: list):
     args = ', '.join([str(arg) for arg in arg_list])
     lambda_str = f"lambda {args}: None"
     exec(lambda_str)
     return eval(lambda_str)
 
 
+def sdk_version(package_name='big-thing-py'):
+    try:
+        return importlib.metadata.version(package_name)
+    except importlib.metadata.PackageNotFoundError:
+        return None
+
+
+def prune_payload(payload: str, mode: MXPrintMode = MXPrintMode.ABBR) -> str:
+    if mode == MXPrintMode.SKIP:
+        payload = colored(f'skip... (mode={mode})', 'yellow')
+    elif mode == MXPrintMode.ABBR:
+        if payload.count('\n') > 10:
+            payload = '\n'.join(payload.split('\n')[:10]) + '\n' + colored(f'skip... (mode={mode})', 'yellow')
+        elif len(payload) > 1000:
+            payload = payload[:1000] + '\n' + colored(f'skip... (mode={mode})', 'yellow')
+        else:
+            pass
+    elif mode == MXPrintMode.FULL:
+        pass
+    else:
+        raise Exception(f'[prune_payload] Unknown mode!!! mode should be [skip|abbr|full] mode : {mode}', 'red')
+
+    return payload
+
+
 if __name__ == '__main__':
     pass
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/utils/file_util.py` & `big_thing_py-0.4.2.0/big_thing_py/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/utils/json_util.py` & `big_thing_py-0.4.2.0/big_thing_py/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/utils/log_util.py` & `big_thing_py-0.4.2.0/big_thing_py/utils/log_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,15 @@
 
         if self._logging_mode == self.LoggingMode.ALL:
             os.makedirs('/'.join(self._file_path.rstrip('/').split('/')), exist_ok=True)
 
             file_logger = logging.getLogger('file_logger')
             file_logger.setLevel(logging.DEBUG)
             file_handler_list = [
-                logging.FileHandler(filename='/'.join([self._file_path, self._file_name]), mode='a', encoding='utf-8')
-                for _ in range(5)
+                logging.FileHandler(filename='/'.join([self._file_path, self._file_name]), mode='a', encoding='utf-8') for _ in range(5)
             ]
 
             for level, file_handler in zip(level_list, file_handler_list):
                 file_handler.setLevel(level)
                 file_handler.setFormatter(formatter)
                 file_logger.addHandler(file_handler)
 
@@ -93,17 +92,15 @@
 
             self._console_logger = console_logger
         elif self._logging_mode == self.LoggingMode.FILE:
             os.makedirs('/'.join(self._file_path.rstrip('/').split('/')), exist_ok=True)
 
             file_logger = logging.getLogger('file_logger')
             file_logger.setLevel(logging.DEBUG)
-            file_handler_list = [
-                logging.FileHandler(filename='/'.join([self._file_path, self._file_name]), mode='a') for _ in range(5)
-            ]
+            file_handler_list = [logging.FileHandler(filename='/'.join([self._file_path, self._file_name]), mode='a') for _ in range(5)]
 
             for level, file_handler in zip(level_list, file_handler_list):
                 file_handler.setLevel(level)
                 file_handler.setFormatter(formatter)
                 file_logger.addHandler(file_handler)
 
             self._file_logger = file_logger
@@ -129,23 +126,21 @@
 
     def select_by_logger_name(self, logger_name: str, logging_func: Callable, msg: List[str], color: str):
         if logger_name == 'console_logger':
             logging_func(colored(msg, color))
         elif logger_name == 'file_logger':
             logging_func(self._remove_color(msg))
 
-    def select_by_print_mode(
-        self, logger: logging.Logger, msg: List[str], color: str, print_mode: PrintMode = PrintMode.DEBUG
-    ):
+    def select_by_print_mode(self, logger: logging.Logger, msg: List[str], color: str, print_mode: PrintMode = PrintMode.DEBUG):
         if print_mode == self.PrintMode.DEBUG:
             self.select_by_logger_name(logger.name, logger.debug, msg, color)
         elif print_mode == self.PrintMode.INFO:
             self.select_by_logger_name(logger.name, logger.info, msg, color)
         elif print_mode == self.PrintMode.WARN:
-            self.select_by_logger_name(logger.name, logger.warn, msg, color)
+            self.select_by_logger_name(logger.name, logger.warning, msg, color)
         elif print_mode == self.PrintMode.ERROR:
             self.select_by_logger_name(logger.name, logger.error, msg, color)
         elif print_mode == self.PrintMode.CRITICAL:
             self.select_by_logger_name(logger.name, logger.critical, msg, color)
         else:
             cprint(f'[MXLOG_DEBUG] not supported print mode...', 'red')
 
@@ -172,39 +167,48 @@
 
 def START_LOGGER(whole_log_path: str = None, logging_mode: MXLogger.LoggingMode = MXLogger.LoggingMode.ALL):
     global base_logger
 
     if not whole_log_path:
         whole_log_path = f'./log/mqtt_message_{time.strftime("%Y%m%d%H%M", time.localtime(time.time()))}.log'
     else:
-        whole_log_path = (
-            f'./{whole_log_path.rsplit(".", 1)[0]}_{time.strftime("%Y%m%d%H%M", time.localtime(time.time()))}.log'
-        )
-    os.makedirs(os.path.dirname(whole_log_path), exist_ok=True)
-    log_name = os.path.basename(whole_log_path)
-    log_path = os.path.dirname(whole_log_path)
+        whole_log_path = f'./{whole_log_path.rsplit(".", 1)[0]}_{time.strftime("%Y%m%d%H%M", time.localtime(time.time()))}.log'
+
+    log_name = ''
+    log_path = ''
+    if logging_mode in [MXLogger.LoggingMode.FILE, MXLogger.LoggingMode.ALL]:
+        os.makedirs(os.path.dirname(whole_log_path), exist_ok=True)
+        log_name = os.path.basename(whole_log_path)
+        log_path = os.path.dirname(whole_log_path)
 
     if base_logger is None:
-        base_logger = MXLogger(log_name, log_path, logging_mode)
+        base_logger = MXLogger(file_name=log_name, file_path=log_path, logging_mode=logging_mode)
         base_logger.start()
     # cprint('logger is started!', 'green')
 
 
 def MXLOG_DEBUG(msg: List[str], color: str = None, mode: MXLogger.PrintMode = MXLogger.PrintMode.DEBUG):
     global base_logger
-    if base_logger is not None:
-        base_logger.print(msg, color, mode)
-    else:
-        cprint('MXLogger is not initialized... start logger init', 'red')
-        # START_LOGGER()
+    if base_logger is None:
+        START_LOGGER()
+
+    base_logger.print(msg, color, mode)
+
+
+def MXLOG_WARN(msg: List[str], color: str = 'yellow', mode: MXLogger.PrintMode = MXLogger.PrintMode.DEBUG):
+    MXLOG_DEBUG(msg, color, mode)
+
+
+def MXLOG_ERROR(msg: List[str], color: str = 'red', mode: MXLogger.PrintMode = MXLogger.PrintMode.DEBUG):
+    MXLOG_DEBUG(msg, color, mode)
 
 
 if __name__ == '__main__':
     # START_LOGGER(logging_mode=MXLogger.LoggingMode.ALL)
-    START_LOGGER(logging_mode=MXLogger.LoggingMode.FILE)
+    START_LOGGER(logging_mode=MXLogger.LoggingMode.OFF)
     # START_LOGGER(logging_mode=MXLogger.LoggingMode.CONSOLE)
     MXLOG_DEBUG('test', 'red')
     MXLOG_DEBUG('test')
     # logger.print(f'INFO test', color='red', mode=MXLogger.PrintMode.INFO)
     # logger.print(f'WARN test', color='red', mode=MXLogger.PrintMode.WARN)
     # logger.print(f'ERROR test', color='red', mode=MXLogger.PrintMode.ERROR)
     # logger.print(f'CRITICAL test', color='red',
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/utils/mqtt_util.py` & `big_thing_py-0.4.2.0/big_thing_py/utils/mqtt_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,67 @@
 from big_thing_py.utils.exception_util import *
 from big_thing_py.utils.log_util import *
 from big_thing_py.utils.json_util import *
 
-import paho.mqtt.client as mqtt
+from gmqtt import Message as MQTTMessage
 
 
-def encode_MQTT_message(topic: str, payload: Union[str, dict], timestamp: float = None) -> mqtt.MQTTMessage:
+def encode_MQTT_message(topic: str, payload: Union[str, dict]) -> MQTTMessage:
     try:
-        msg = mqtt.MQTTMessage()
-        msg.topic = bytes(topic, encoding='utf-8')
         if isinstance(payload, str):
-            msg.payload = bytes(payload, encoding='utf-8')
+            payload = bytes(payload, encoding='utf-8')
         elif isinstance(payload, dict):
-            msg.payload = dict_to_json_string(payload)
-        msg.timestamp = timestamp
+            payload = dict_to_json_string(payload)
 
-        return msg
+        return MQTTMessage(topic, payload)
     except Exception as e:
         print_error(e)
         raise e
 
 
-def decode_MQTT_message(msg: mqtt.MQTTMessage, mode=dict) -> Tuple[str, dict]:
+def decode_MQTT_message(msg: MQTTMessage, mode=dict) -> Tuple[str, dict]:
     topic = msg.topic
     payload = msg.payload
-    timestamp: float = msg.timestamp
 
     if isinstance(topic, bytes):
         topic = topic.decode()
     if isinstance(payload, bytes):
         payload = payload.decode()
 
     if isinstance(payload, str):
         if mode == str:
-            return topic, payload, timestamp
+            return topic, payload
         elif mode == dict:
-            return topic, json_string_to_dict(payload), timestamp
+            return topic, json_string_to_dict(payload)
         else:
             raise MXNotSupportedError(f'Unexpected mode!!! - {mode}')
     elif isinstance(payload, dict):
         if mode == str:
-            return topic, dict_to_json_string(payload), timestamp
+            return topic, dict_to_json_string(payload)
         elif mode == dict:
-            return topic, payload, timestamp
+            return topic, payload
         else:
             raise MXNotSupportedError(f'Unexpected mode!!! - {mode}')
     else:
         raise MXNotSupportedError(f'Unexpected type!!! - {type(payload)}')
 
 
 def topic_split(topic: str):
     return topic.split('/')
 
 
 def topic_join(topic: List[str]):
     return '/'.join(topic)
 
 
-def unpack_mqtt_message(msg: mqtt.MQTTMessage) -> Tuple[List[str], str]:
-    topic, payload, timestamp = decode_MQTT_message(msg, dict)
+def unpack_mqtt_message(msg: MQTTMessage) -> Tuple[List[str], str]:
+    topic, payload = decode_MQTT_message(msg, dict)
     topic = topic_split(topic)
 
-    return topic, payload, timestamp
+    return topic, payload
 
 
-def pack_mqtt_message(topic_list: List[str], payload: str) -> mqtt.MQTTMessage:
+def pack_mqtt_message(topic_list: List[str], payload: str) -> MQTTMessage:
     topic = topic_join(topic_list)
     msg = encode_MQTT_message(topic, payload)
 
     return msg
```

### Comparing `big_thing_py-0.4.1.5.post9/big_thing_py/utils/rf_util.py` & `big_thing_py-0.4.2.0/big_thing_py/utils/rf_util.py`

 * *Files identical despite different names*

### Comparing `big_thing_py-0.4.1.5.post9/PKG-INFO` & `big_thing_py-0.4.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: big-thing-py
-Version: 0.4.1.5.post9
+Version: 0.4.2.0
 Summary: MySSIX Thing SDK
 Author: caplab
-Author-email: caplab94@gmail.com
+Author-email: mysmaxlab@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bless (>=0.2.5,<0.3.0)
+Requires-Dist: dataclasses (>=0.6,<0.7)
+Requires-Dist: dbus-next (==0.2.3)
 Requires-Dist: func-timeout (>=4.3.5,<5.0.0)
 Requires-Dist: getmac (>=0.9.4,<0.10.0)
-Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
-Requires-Dist: pytest (>=7.3.2,<8.0.0)
+Requires-Dist: gmqtt (>=0.6.14,<0.7.0)
+Requires-Dist: importlib-metadata (>=7.0.1,<8.0.0)
+Requires-Dist: pytest (>=7.4.3,<8.0.0)
+Requires-Dist: pytest-asyncio (>=0.23.2,<0.24.0)
+Requires-Dist: pytest-timeout (>=2.2.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
-Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
+Requires-Dist: typing-extensions (>=4.0,<5.0)
+Requires-Dist: uvloop (==0.19.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Requires-Dist: zeroconf (>=0.69.0,<0.70.0)
 Description-Content-Type: text/markdown
 
 # MySSIX Thing SDK for Python
 
 [![PyPI version](https://badge.fury.io/py/big-thing-py.svg)](https://badge.fury.io/py/big-thing-py)
```


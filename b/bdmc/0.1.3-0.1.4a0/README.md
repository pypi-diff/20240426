# Comparing `tmp/bdmc-0.1.3.tar.gz` & `tmp/bdmc-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.3.tar", last modified: Wed Apr 24 15:34:35 2024, max compression
+gzip compressed data, was "bdmc-0.1.4a0.tar", last modified: Fri Apr 26 02:34:30 2024, max compression
```

## Comparing `bdmc-0.1.3.tar` & `bdmc-0.1.4a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5296 2024-04-24 15:34:16.527923 bdmc-0.1.3/README.md
--rw-r--r--   0        0        0      545 2024-04-24 15:34:35.795927 bdmc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      526 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/__init__.py
--rw-r--r--   0        0        0      133 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0    13632 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2266 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7404 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0      682 2024-04-24 15:34:16.527923 bdmc-0.1.3/tests/find_tests.py
--rw-r--r--   0        0        0     4405 2024-04-24 15:34:16.527923 bdmc-0.1.3/tests/test_context.py
--rw-r--r--   0        0        0     1991 2024-04-24 15:34:16.527923 bdmc-0.1.3/tests/test_controller.py
--rw-r--r--   0        0        0     5610 1970-01-01 00:00:00.000000 bdmc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5296 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/README.md
+-rw-r--r--   0        0        0      547 2024-04-26 02:34:30.017123 bdmc-0.1.4a0/pyproject.toml
+-rw-r--r--   0        0        0      526 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    16964 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7404 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-04-26 02:34:08.669059 bdmc-0.1.4a0/tests/find_tests.py
+-rw-r--r--   0        0        0     4405 2024-04-26 02:34:08.673059 bdmc-0.1.4a0/tests/test_context.py
+-rw-r--r--   0        0        0     1991 2024-04-26 02:34:08.673059 bdmc-0.1.4a0/tests/test_controller.py
+-rw-r--r--   0        0        0     5612 1970-01-01 00:00:00.000000 bdmc-0.1.4a0/PKG-INFO
```

### Comparing `bdmc-0.1.3/README.md` & `bdmc-0.1.4a0/README.md`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.3/pyproject.toml` & `bdmc-0.1.4a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.3"
+version = "0.1.4a0"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.3/src/bdmc/__init__.py` & `bdmc-0.1.4a0/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.3/src/bdmc/modules/controller.py` & `bdmc-0.1.4a0/src/bdmc/modules/controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,14 +37,50 @@
         return self.code_sign == other.code_sign
 
     def __hash__(self) -> int:
         return hash(self.code_sign)
 
 
 class CloseLoopController:
+    """
+    CloseLoopController is a class designed to manage and control a system involving multiple motors with closed-loop feedback.
+    It provides methods for setting motor speeds, sending commands, introducing delays with breakers, and updating a shared context.
+    The controller maintains a connection to a serial client for communication with the hardware, manages a command queue,
+    and runs a dedicated thread for message sending. It also allows registering context updaters and getters to facilitate data flow within the application.
+
+    Key features and functionality include:
+
+    1. **Initialization**:
+       - Accepts a list of `MotorInfo` objects, specifying motor IDs and directions, and an optional serial port for communication.
+       - Initializes a `SerialClient` for interfacing with the hardware, a command queue, and a flag for controlling the message sending thread.
+
+    2. **Context Management**:
+       - Maintains a dictionary (`_context`) to store shared data across the application.
+       - Provides methods `register_context_updater` and `register_context_getter` to register functions that update or retrieve specific context variables.
+
+    3. **Motor Control**:
+       - `set_motors_speed`: Sets the speed of each motor based on a provided list of speeds, ensuring consistency with the provided `MotorInfo`.
+       - `send_cmd`: Adds a command to the command queue for transmission to the hardware.
+
+    4. **Message Sending**:
+       - Manages a background thread (`_msg_send_thread`) responsible for continuously retrieving messages from the command queue and writing them to the serial channel.
+       - Offers `start_msg_sending` and `stop_msg_sending` methods to control the message sending thread's lifecycle.
+
+    5. **Delay Functions**:
+       - `delay`: Introduces a simple delay for a specified duration in seconds.
+       - `delay_b`: Delays execution for a given time, periodically checking a breaker function that can abort the delay if it returns True.
+       - `delay_b_match`: Similar to `delay_b`, but returns the result of the breaker function once the delay has completed or the breaker condition is met.
+
+    6. **Utility Methods**:
+       - `wait_exec`: Executes a given function and returns the instance of the class itself.
+       - Properties `context`, `motor_ids`, `motor_dirs`, `cmd_queue`, and `serial_client` provide convenient access to internal attributes.
+
+    Overall, the CloseLoopController serves as a central hub for coordinating motor operations, handling communication with the hardware, managing shared data, and introducing controlled delays with breakers in a closed-loop motor control system.
+    """
+
     def __init__(
         self, motor_infos: Sequence[MotorInfo], port: Optional[str] = None, context: Optional[Dict[str, Any]] = None
     ) -> None:
         """
         :param motor_infos: A list of MotorInfo objects containing motor ID and direction.
         """
         if len(motor_infos) != len(set(motor_infos)):
@@ -147,14 +183,27 @@
 
             case _:
                 raise ValueError(
                     f"Invalid arguments for register_context_updater function. got {input_keys} and {output_keys} and {freeze_inputs}"
                 )
         return _updater
 
+    def register_context_getter(self, var_key: str) -> Callable[[], Any]:
+        """
+        Register a context getter function for a given variable key.
+
+        Args:
+            var_key (str): The key of the variable.
+
+        Returns:
+            Callable[[], Any]: A function that returns the value of the variable.
+        """
+        context = self._context
+        return lambda: context.get(var_key)
+
     def wait_exec(self, function: Callable[[], None]) -> Self:
         """
         Executes the given function and returns the instance of the class itself.
 
         Parameters:
             function (Callable[[], None]): The function to be executed.
 
@@ -233,39 +282,47 @@
         """
 
         while self._msg_send_thread_should_run:
             temp = self._cmd_queue.get()
             _logger.debug(f"Writing {temp} to channel,remaining {self._cmd_queue.qsize()}")
             self._serial.write(temp)
 
-    def set_motors_speed(self, speeds: Sequence[int]) -> Self:
+    def set_motors_speed(self, speeds: Sequence[int | float]) -> Self:
         """
         Set the speed for each motor based on the provided speed_list.
 
         Parameters:
-            speeds (Sequence[int]): A list of speeds for each motor.
+            speeds (Sequence[int|float]): A list of speeds for each motor.
 
         Returns:
             None
         """
 
         if len(speeds) != len(self._motor_infos):
             raise ValueError("Length of speed_list must be equal to the number of motors")
         self._cmd_queue.put(
             (
                 "".join(
-                    f"{motor_info.code_sign}v{speed * motor_info.direction}\r"
+                    f"{motor_info.code_sign}v{int(speed * motor_info.direction)}\r"
                     for motor_info, speed in zip(self._motor_infos, speeds)
                 )
             ).encode("ascii")
         )
         return self
 
     def send_cmd(self, cmd: CMD) -> Self:
+        """
+        Add a command to the command queue.
 
+        Args:
+            cmd (CMD): The command to be added to the queue.
+
+        Returns:
+            Self: Returns the instance of the class.
+        """
         self._cmd_queue.put(cmd.value)
         return self
 
     def delay_b(
         self,
         delay_sec: float,
         breaker: Callable[[], Any],
```

### Comparing `bdmc-0.1.3/src/bdmc/modules/debug.py` & `bdmc-0.1.4a0/src/bdmc/modules/debug.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.3/src/bdmc/modules/logger.py` & `bdmc-0.1.4a0/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.3/src/bdmc/modules/port.py` & `bdmc-0.1.4a0/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.3/src/bdmc/modules/seriald.py` & `bdmc-0.1.4a0/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.3/tests/find_tests.py` & `bdmc-0.1.4a0/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.3/tests/test_context.py` & `bdmc-0.1.4a0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.3/tests/test_controller.py` & `bdmc-0.1.4a0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.3/PKG-INFO` & `bdmc-0.1.4a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdmc
-Version: 0.1.3
+Version: 0.1.4a0
 Summary: An api wrapper lib designed for the uptech BDMC divers
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pyserial>=3.5
 Requires-Dist: coloredlogs>=15.0.1
 Description-Content-Type: text/markdown
```


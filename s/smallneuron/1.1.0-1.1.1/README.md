# Comparing `tmp/smallneuron-1.1.0.tar.gz` & `tmp/smallneuron-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.1.0.tar", last modified: Fri Apr 19 22:24:26 2024, max compression
+gzip compressed data, was "smallneuron-1.1.1.tar", last modified: Fri Apr 26 20:44:57 2024, max compression
```

## Comparing `smallneuron-1.1.0.tar` & `smallneuron-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 22:24:26.822252 smallneuron-1.1.0/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.0/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.0/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-19 22:24:26.822252 smallneuron-1.1.0/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-14 21:53:34.000000 smallneuron-1.1.0/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.0/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-04-19 22:22:47.000000 smallneuron-1.1.0/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-04-19 22:24:26.822252 smallneuron-1.1.0/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 22:24:26.818252 smallneuron-1.1.0/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 22:24:26.818252 smallneuron-1.1.0/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.0/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.0/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.0/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.0/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.0/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.0/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    13916 2024-04-19 22:22:47.000000 smallneuron-1.1.0/src/smallneuron/smallneuron.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.0/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.0/src/smallneuron/sngpio.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4087 2024-04-14 22:54:22.000000 smallneuron-1.1.0/src/smallneuron/snhttp.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.0/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.0/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2555 2024-04-14 22:54:22.000000 smallneuron-1.1.0/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.0/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 22:24:26.822252 smallneuron-1.1.0/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-19 22:24:26.000000 smallneuron-1.1.0/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      775 2024-04-19 22:24:26.000000 smallneuron-1.1.0/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-04-19 22:24:26.000000 smallneuron-1.1.0/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-04-19 22:24:26.000000 smallneuron-1.1.0/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 22:24:26.818252 smallneuron-1.1.0/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.0/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.0/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.0/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.0/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.989407 smallneuron-1.1.1/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.1/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.1/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-26 20:44:57.989407 smallneuron-1.1.1/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-14 21:53:34.000000 smallneuron-1.1.1/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.1/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-04-26 20:35:05.000000 smallneuron-1.1.1/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-04-26 20:44:57.989407 smallneuron-1.1.1/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.985407 smallneuron-1.1.1/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.985407 smallneuron-1.1.1/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.1/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    13916 2024-04-19 22:22:47.000000 smallneuron-1.1.1/src/smallneuron/smallneuron.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.1/src/smallneuron/snapi.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.1/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.1/src/smallneuron/sngpio.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.1/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.1/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3048 2024-04-26 20:35:05.000000 smallneuron-1.1.1/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.1/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.989407 smallneuron-1.1.1/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-26 20:44:57.000000 smallneuron-1.1.1/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-04-26 20:44:57.000000 smallneuron-1.1.1/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-04-26 20:44:57.000000 smallneuron-1.1.1/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-04-26 20:44:57.000000 smallneuron-1.1.1/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.985407 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.1.0/LICENSE` & `smallneuron-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/PKG-INFO` & `smallneuron-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.0
+Version: 1.1.1
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.0/README.md` & `smallneuron-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/example.py` & `smallneuron-1.1.1/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/pyproject.toml` & `smallneuron-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.1.0/src/smallneuron/gpio_h3.c` & `smallneuron-1.1.1/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron/gpio_h3.h` & `smallneuron-1.1.1/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron/gpio_h3.so` & `smallneuron-1.1.1/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron/logger.py` & `smallneuron-1.1.1/src/smallneuron/logger.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron/smallneuron.py` & `smallneuron-1.1.1/src/smallneuron/smallneuron.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron/sndummy.py` & `smallneuron-1.1.1/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron/sngpio.py` & `smallneuron-1.1.1/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron/snhttp.py` & `smallneuron-1.1.1/src/smallneuron/snapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,28 +83,25 @@
             print("forwarding content ", content )
             logger(syslog.LOG_INFO,  "forwarding to ", content["url"], " payload ", content["post"] )
             r=post(args["url"], json=content["post"]);
             return r.json(), r.status_code
         else:
             return None, 405
             
+api.add_resource(PlannerServer, '/<string:action>','/<string:action>/<string:kart_id>')  # Kart list status, and plan
+api.add_resource(Order, '/order', '/order/<int:order_id>')                        # POST New order, GET Order status ,DELETE Order    ,  '/order/<int:order_id>',  endpoint="order_id"
+api.add_resource(Task, '/task/<int:task_id>')  # End task
+api.add_resource(Kart, '/kart/<string:kart_id>', '/kart/<string:component>/<string:code>')   # Checkin and send event
 
 class SnHttp(Flask):
     def __init__(self):
         super().__init__(__name__)
         self.app = Flask(__name__)
         self.api = Api(self.app)
+    
+    def add_resource(self, resource, *urls, **kwargs):
+        self.api.add_resource(resource, urls, kwargs)
 
-    def addEvent(self, event_name, path):
-        self.api.add_resource(HttpEvent, path )
-
-    def start(self):
+    def start(self, service_port=9000):
         self.app.config['MAX_CONTENT_LENGTH'] = 1024 * 1024 * 1024
-        self.app.run(debug=False, host= '0.0.0.0')
-
+        self.app.run(debug=False, host= '0.0.0.0', port=service_port)
 
-if __name__ == '__main__': 
-    except KeyboardInterrupt:
-        pass
-    finally:
-        pass
-        #stopAllKarts()
```

### Comparing `smallneuron-1.1.0/src/smallneuron/sninput.py` & `smallneuron-1.1.1/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron/snmqtt.py` & `smallneuron-1.1.1/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron/snserial.py` & `smallneuron-1.1.1/src/smallneuron/snserial.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,52 +2,65 @@
 # Este modulo escucha en una puerta serial, se definen eventos
 # en base a patrones (regEx) del contenido leido, se testean
 # secuencialemnte en el orden que dueron agregados
 #
 # pip install pyserial
 #
 import serial
+import time
 import re
 import threading
 import os.path
 import traceback
 from .logger import Logger
 
 log=Logger("smallneuron.SnSerial")
 
 def eventWait(snserial):
     try:
         log.info("reader started")
+        fails=0
         while True:
-            line = snserial.read_until(snserial.eol)
-
-            for e in snserial.events:
-                if re.search(e[1], line) != None:
-                    if snserial.eventManager == None:
-                        log.error("Warning eventManager not defined")
-                    else:
-                        snserial.eventManager.putEvent(e[0], {"data": str(line)})
-                    log.info("event ", e[0], line)
-                    break
+            try:
+                line = snserial.read_until(snserial.eol)
+                fails=0
+                for e in snserial.events:
+                    if re.search(e[1], line) != None:
+                        if snserial.eventManager == None:
+                            log.error("Warning eventManager not defined")
+                        else:
+                            snserial.eventManager.putEvent(e[0], {"data": str(line)})
+                        log.info("event ", e[0], line)
+                        break
+            except Exception as e:
+                fails=fails+1
+                if fails > 10:
+                    raise("Falla multiples veces lectura serial "+str(fails))
+                log.error("Reintentamos lectura "+str(e) )
+                time.sleep(1)
+                snserial.close()
+                snserial.rotateOpen()
+                
     except Exception as e:
         log.error(e)
         log.error(traceback.format_exc())
         snserial.eventManager.putEvent("panic", str(e))
-        exit(1)
+
 
 
 class SnSerial(serial.Serial):
     def __init__(self, eventManager, port, baudrate, bytesize, parity, stopbits, endofline: bytes = b"\r"):
         super().__init__(baudrate=baudrate, bytesize=bytesize, parity=parity, stopbits=stopbits)
-        self.rotateOpen(port=port)
+        self.originalPort=port
+        self.rotateOpen()
         self.eventManager = eventManager
         self.eol = endofline
         self.events = []
         log.info("start")
-
+        
     def addEvent(self, event, pattern=".*"):
         self.events.append((event, pattern))
 
     def read_until(self, end_of_read_byte: bytes = b"\r"):
         line = b""
         c = b""
         while c != end_of_read_byte:
@@ -56,20 +69,21 @@
         return line[:-1].decode("utf-8")
 
     def start(self):
         log.debug("SnSerial started")
         threading.Thread(target=lambda: eventWait(self)).start()
 
     # Intentara abrir la puerta termina con 0 (cero) y falla lo cambiara el final por 1 (uno)
-    def rotateOpen(self, port):
+    def rotateOpen(self):
+        port=self.originalPort
         if not os.path.exists(port):
                 port=port[:-1]+"1"
                 log.debug("snserial port not exist, trying ",port)
         self.port=port # al parecer esto abre el puerto
-        self.open()      # pero para estar seguro
+        self.open()    # pero para estar seguro
         log.debug("snserial port:", port)
 
 
 # Para pruebas
 if __name__ == '__main__':
     print("Waiting for read")
     s=SnSerial( None, "/dev/ttyACM0", 9600, serial.EIGHTBITS, serial.PARITY_NONE, serial.STOPBITS_ONE)
```

### Comparing `smallneuron-1.1.0/src/smallneuron/sntimer.py` & `smallneuron-1.1.1/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.0/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.1.1/src/smallneuron.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.0
+Version: 1.1.1
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.0/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.1.1/src/smallneuron.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 src/smallneuron/__init__.py
 src/smallneuron/build
 src/smallneuron/gpio_h3.c
 src/smallneuron/gpio_h3.h
 src/smallneuron/gpio_h3.so
 src/smallneuron/logger.py
 src/smallneuron/smallneuron.py
+src/smallneuron/snapi.py
 src/smallneuron/sndummy.py
 src/smallneuron/sngpio.py
-src/smallneuron/snhttp.py
 src/smallneuron/sninput.py
 src/smallneuron/snmqtt.py
 src/smallneuron/snserial.py
 src/smallneuron/sntimer.py
 src/smallneuron.egg-info/PKG-INFO
 src/smallneuron.egg-info/SOURCES.txt
 src/smallneuron.egg-info/dependency_links.txt
```

### Comparing `smallneuron-1.1.0/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files identical despite different names*


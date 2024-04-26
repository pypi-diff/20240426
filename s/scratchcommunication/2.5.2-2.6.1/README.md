# Comparing `tmp/scratchcommunication-2.5.2.tar.gz` & `tmp/scratchcommunication-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.5.2.tar", last modified: Sun Apr 21 15:00:49 2024, max compression
+gzip compressed data, was "scratchcommunication-2.6.1.tar", last modified: Fri Apr 26 18:44:18 2024, max compression
```

## Comparing `scratchcommunication-2.5.2.tar` & `scratchcommunication-2.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:00:49.412691 scratchcommunication-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-21 15:00:49.412691 scratchcommunication-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:00:49.408692 scratchcommunication-2.5.2/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:00:49.412691 scratchcommunication-2.5.2/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:00:49.412691 scratchcommunication-2.5.2/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-21 15:00:49.000000 scratchcommunication-2.5.2/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 15:00:49.000000 scratchcommunication-2.5.2/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:00:49.000000 scratchcommunication-2.5.2/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 15:00:49.000000 scratchcommunication-2.5.2/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 15:00:49.000000 scratchcommunication-2.5.2/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 15:00:49.412691 scratchcommunication-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:00:49.412691 scratchcommunication-2.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-21 15:00:40.000000 scratchcommunication-2.5.2/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.254598 scratchcommunication-2.6.1/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.254598 scratchcommunication-2.6.1/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 18:44:18.000000 scratchcommunication-2.6.1/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:44:18.258597 scratchcommunication-2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 18:44:14.000000 scratchcommunication-2.6.1/tests/test1.py
```

### Comparing `scratchcommunication-2.5.2/LICENSE` & `scratchcommunication-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.5.2/PKG-INFO` & `scratchcommunication-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.5.2
+Version: 2.6.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -276,15 +276,15 @@
 
 Stop the cloud requests handler using the `stop` method. (Only if the cloud requests handler is running in a thread)
 
 ```python
 cloud_requests.stop()
 ```
 
-## Encrypted data transmition
+## Encrypted data transmission
 
 See [Cloud Socket Security](#cloud-socket-security) for this.
 
 ## Client side
 
 If you haven't already, you'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud requests to work.
```

### Comparing `scratchcommunication-2.5.2/README.md` & `scratchcommunication-2.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
 Stop the cloud requests handler using the `stop` method. (Only if the cloud requests handler is running in a thread)
 
 ```python
 cloud_requests.stop()
 ```
 
-## Encrypted data transmition
+## Encrypted data transmission
 
 See [Cloud Socket Security](#cloud-socket-security) for this.
 
 ## Client side
 
 If you haven't already, you'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud requests to work.
```

### Comparing `scratchcommunication-2.5.2/scratchcommunication/cloud.py` & `scratchcommunication-2.6.1/scratchcommunication/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.5.2/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.6.1/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.5.2/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.6.1/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.5.2/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.6.1/scratchcommunication/cloudrequests/requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,19 +75,24 @@
                         for req_name, raw_req in zip(sub_request_names, raw_sub_requests):
                             if re.match(r"\w+\(.*\)$", raw_req) and self.requests[req_name].allow_python_syntax:
                                 name, args, kwargs = parse_python_request(raw_req, req_name)
                             elif not re.match(r"\w+(.*)$", raw_req):
                                 name, args, kwargs = parse_normal_request(raw_req, req_name)
                             else:
                                 raise PermissionError("Python syntax is not allowed for this.")
+                    except Exception:
+                        response = "The command syntax was wrong."
+                        warnings.warn("Received a request with an invalid syntax.", RuntimeWarning)
+                    else:
+                        try:
                             self.execute_request(name, args=args, kwargs=kwargs, client=client)
                             response = None
-                    except Exception:
-                        response = "There was an error."
-                        warnings.warn("Received a request with an invalid syntax.", SyntaxWarning)
+                        except Exception:
+                            response = "Something went wrong."
+                            warnings.warn("Something went wrong with a request.", RuntimeWarning)
                     if response:
                         client.send(response)
             except Exception:
                 warnings.warn(f"There was an uncaught error in the request handler: {traceback.format_exc()}", RuntimeWarning)
                 
     
     def execute_request(self, name, *, args : Sequence[Any], kwargs : Mapping[str, Any], client : CloudSocketConnection) -> Union[str, float, int]:
@@ -112,15 +117,19 @@
                     continue
                 if not annotation.kind.value in [1, 3]:
                     raise ValueError("Signature doesn't match")
                 kwargs[arg] = annotation.annotation(kwargs[arg])
             if inspect.signature(request_handling_function).return_annotation != inspect.Signature.empty:
                 return_converter = inspect.signature(request_handling_function).return_annotation
         def respond():
-            client.send(str(return_converter(request_handling_function(*args, **kwargs))))
+            try:
+                response = str(return_converter(request_handling_function(*args, **kwargs)))
+            except ErrorMessage as e:
+                response = " ".join(e.args)
+            client.send(response)
         if request_handling_function.thread:
             thread = StoppableThread(target=respond)
             thread.start()
             return
         respond()
     
     def stop(self):
@@ -207,15 +216,18 @@
         except StopIteration:
             args.append(float(content) if mode == FLT else (int(content) if mode == NUM else content))
             break
     assert args.pop(0) == name
     return name, args, {}
 
 
-
+class ErrorMessage(Exception):
+    """
+    Error with a message
+    """
```

### Comparing `scratchcommunication-2.5.2/scratchcommunication/security.py` & `scratchcommunication-2.6.1/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.5.2/scratchcommunication/session.py` & `scratchcommunication-2.6.1/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.5.2/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.6.1/scratchcommunication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.5.2
+Version: 2.6.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -276,15 +276,15 @@
 
 Stop the cloud requests handler using the `stop` method. (Only if the cloud requests handler is running in a thread)
 
 ```python
 cloud_requests.stop()
 ```
 
-## Encrypted data transmition
+## Encrypted data transmission
 
 See [Cloud Socket Security](#cloud-socket-security) for this.
 
 ## Client side
 
 If you haven't already, you'll need to put the first sprite from this [project](https://scratch.mit.edu/projects/884190099/) in your project for cloud requests to work.
```

### Comparing `scratchcommunication-2.5.2/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.6.1/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.5.2/setup.py` & `scratchcommunication-2.6.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.5.2'
+VERSION = '2.6.1'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.5.2/tests/test1.py` & `scratchcommunication-2.6.1/tests/test1.py`

 * *Files identical despite different names*


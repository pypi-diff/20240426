# Comparing `tmp/echo_endpoints-0.0.3.tar.gz` & `tmp/echo_endpoints-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echo_endpoints-0.0.3.tar", last modified: Tue Apr 23 06:25:24 2024, max compression
+gzip compressed data, was "echo_endpoints-0.0.4.tar", last modified: Fri Apr 26 07:08:55 2024, max compression
```

## Comparing `echo_endpoints-0.0.3.tar` & `echo_endpoints-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-23 06:25:24.482357 echo_endpoints-0.0.3/
--rw-r--r--   0 jheaminoff   (501) staff       (20)     1066 2024-04-23 05:50:31.000000 echo_endpoints-0.0.3/LICENSE
--rw-r--r--   0 jheaminoff   (501) staff       (20)     1256 2024-04-23 06:25:24.481647 echo_endpoints-0.0.3/PKG-INFO
--rw-r--r--   0 jheaminoff   (501) staff       (20)      890 2024-04-23 06:10:50.000000 echo_endpoints-0.0.3/README.md
--rw-r--r--   0 jheaminoff   (501) staff       (20)      352 2024-04-23 06:23:25.000000 echo_endpoints-0.0.3/pyproject.toml
--rw-r--r--   0 jheaminoff   (501) staff       (20)       38 2024-04-23 06:25:24.482500 echo_endpoints-0.0.3/setup.cfg
-drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-23 06:25:24.474717 echo_endpoints-0.0.3/src/
-drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-23 06:25:24.477372 echo_endpoints-0.0.3/src/echo_endpoints/
--rw-r--r--   0 jheaminoff   (501) staff       (20)        0 2024-04-23 05:47:19.000000 echo_endpoints-0.0.3/src/echo_endpoints/__init__.py
--rw-r--r--   0 jheaminoff   (501) staff       (20)     5636 2024-04-23 06:25:16.000000 echo_endpoints-0.0.3/src/echo_endpoints/echo_endpoints.py
-drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-23 06:25:24.481016 echo_endpoints-0.0.3/src/echo_endpoints.egg-info/
--rw-r--r--   0 jheaminoff   (501) staff       (20)     1256 2024-04-23 06:25:24.000000 echo_endpoints-0.0.3/src/echo_endpoints.egg-info/PKG-INFO
--rw-r--r--   0 jheaminoff   (501) staff       (20)      268 2024-04-23 06:25:24.000000 echo_endpoints-0.0.3/src/echo_endpoints.egg-info/SOURCES.txt
--rw-r--r--   0 jheaminoff   (501) staff       (20)        1 2024-04-23 06:25:24.000000 echo_endpoints-0.0.3/src/echo_endpoints.egg-info/dependency_links.txt
--rw-r--r--   0 jheaminoff   (501) staff       (20)       15 2024-04-23 06:25:24.000000 echo_endpoints-0.0.3/src/echo_endpoints.egg-info/top_level.txt
+drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-26 07:08:55.368140 echo_endpoints-0.0.4/
+-rw-r--r--   0 jheaminoff   (501) staff       (20)     1066 2024-04-23 05:50:31.000000 echo_endpoints-0.0.4/LICENSE
+-rw-r--r--   0 jheaminoff   (501) staff       (20)     1280 2024-04-26 07:08:55.367388 echo_endpoints-0.0.4/PKG-INFO
+-rw-r--r--   0 jheaminoff   (501) staff       (20)      890 2024-04-23 06:10:50.000000 echo_endpoints-0.0.4/README.md
+-rw-r--r--   0 jheaminoff   (501) staff       (20)      386 2024-04-26 07:08:47.000000 echo_endpoints-0.0.4/pyproject.toml
+-rw-r--r--   0 jheaminoff   (501) staff       (20)       38 2024-04-26 07:08:55.368320 echo_endpoints-0.0.4/setup.cfg
+drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-26 07:08:55.356864 echo_endpoints-0.0.4/src/
+drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-26 07:08:55.360132 echo_endpoints-0.0.4/src/echo_endpoints/
+-rw-r--r--   0 jheaminoff   (501) staff       (20)       41 2024-04-26 07:07:38.000000 echo_endpoints-0.0.4/src/echo_endpoints/__init__.py
+-rw-r--r--   0 jheaminoff   (501) staff       (20)     5552 2024-04-26 07:05:15.000000 echo_endpoints-0.0.4/src/echo_endpoints/echo_endpoints.py
+drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-26 07:08:55.366621 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/
+-rw-r--r--   0 jheaminoff   (501) staff       (20)     1280 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/PKG-INFO
+-rw-r--r--   0 jheaminoff   (501) staff       (20)      309 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/SOURCES.txt
+-rw-r--r--   0 jheaminoff   (501) staff       (20)        1 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/dependency_links.txt
+-rw-r--r--   0 jheaminoff   (501) staff       (20)        9 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/requires.txt
+-rw-r--r--   0 jheaminoff   (501) staff       (20)       15 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/top_level.txt
```

### Comparing `echo_endpoints-0.0.3/LICENSE` & `echo_endpoints-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `echo_endpoints-0.0.3/PKG-INFO` & `echo_endpoints-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: echo_endpoints
-Version: 0.0.3
+Version: 0.0.4
 Summary: Requests formatter
 Author-email: JHEAminoff <jheaminoff@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 EchoEndpoints                                        
 
 EchoEndpoints is designed to simplify the process of making HTTP requests,
 handling responses, and interacting with APIs.
 
 It offers a suite of functions that cover various aspects of web requests,
```

### Comparing `echo_endpoints-0.0.3/README.md` & `echo_endpoints-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `echo_endpoints-0.0.3/src/echo_endpoints/echo_endpoints.py` & `echo_endpoints-0.0.4/src/echo_endpoints/echo_endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import requests
 import logging
 from typing import Optional, Dict, Any
 import json
 
 logging.basicConfig(level=logging.INFO)
 
@@ -93,30 +92,28 @@
 
     response_time = response.elapsed.total_seconds()
     status_code_color = (
         ANSIColors.GREEN if response.status_code == 200 else ANSIColors.RED
     )
     print(f"{status_code_color}Status Code: {response.status_code}{ANSIColors.RESET}")
     print(f"{ANSIColors.CYAN}Response Time: {response_time} seconds{ANSIColors.RESET}")
-    print(
-        f"{ANSIColors.YELLOW}Response Text (snippet):{ANSIColors.RESET} {response.text[:250]} ..."
-    )
+
     if "application/json" in response.headers.get("Content-Type", ""):
-        formatted_response = format_json_response(response)
-    else:
-        formatted_response = response.text[:250] + "..."
+        if print_full_response:
+            # Print the full response only if requested
+            print(f"{ANSIColors.MAGENTA}Full Response:{ANSIColors.RESET}")
+            full_content = format_json_response(response)
+            print(full_content)
+        else:
+            formatted_response = response.text[:250] + "..."  # Ensure snippet ends with "..."
+            print(f"{ANSIColors.YELLOW}Response Text (snippet):{ANSIColors.RESET} {formatted_response}")
 
-    # Print response details
-    print(f"{ANSIColors.CYAN}Response Time: {response.elapsed.total_seconds()} seconds{ANSIColors.RESET}")
-    print(f"{ANSIColors.YELLOW}Response Text (snippet):{ANSIColors.RESET} {formatted_response}")
-
-    if print_full_response:
-        # If full response printing is requested, print the entire content appropriately
-        full_content = response.text if "application/json" not in response.headers.get("Content-Type", "") else formatted_response
-        print(full_content)
+    else:
+        formatted_response = response.text[:250] + "..."  # Ensure snippet ends with "..."
+        print(f"{ANSIColors.YELLOW}Response Text (snippet):{ANSIColors.RESET} {formatted_response}")
 
 
 # Define the echo_endpoint function, the main entrypoint
 def echo_endpoint(
     url: str,
     method: str,
     headers: Optional[Dict[str, str]] = None,
```

### Comparing `echo_endpoints-0.0.3/src/echo_endpoints.egg-info/PKG-INFO` & `echo_endpoints-0.0.4/src/echo_endpoints.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: echo_endpoints
-Version: 0.0.3
+Version: 0.0.4
 Summary: Requests formatter
 Author-email: JHEAminoff <jheaminoff@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 EchoEndpoints                                        
 
 EchoEndpoints is designed to simplify the process of making HTTP requests,
 handling responses, and interacting with APIs.
 
 It offers a suite of functions that cover various aspects of web requests,
```


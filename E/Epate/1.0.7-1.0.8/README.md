# Comparing `tmp/epate-1.0.7.tar.gz` & `tmp/epate-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epate-1.0.7.tar", last modified: Fri Apr 26 18:15:56 2024, max compression
+gzip compressed data, was "epate-1.0.8.tar", last modified: Fri Apr 26 18:22:12 2024, max compression
```

## Comparing `epate-1.0.7.tar` & `epate-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 18:15:56.697060 epate-1.0.7/
-drwxrwxrwx   0        0        0        0 2024-04-26 18:15:56.659959 epate-1.0.7/Epate/
--rw-rw-rw-   0        0        0     5503 2024-04-26 18:15:42.000000 epate-1.0.7/Epate/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 17:50:18.000000 epate-1.0.7/Epate/epate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:15:56.690680 epate-1.0.7/Epate.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      562 2024-04-26 18:15:56.691677 epate-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 18:15:56.697060 epate-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      901 2024-04-26 18:15:47.000000 epate-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:22:12.794500 epate-1.0.8/
+drwxrwxrwx   0        0        0        0 2024-04-26 18:22:12.763494 epate-1.0.8/Epate/
+-rw-rw-rw-   0        0        0     5505 2024-04-26 18:21:52.000000 epate-1.0.8/Epate/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:50:18.000000 epate-1.0.8/Epate/epate.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:22:12.787611 epate-1.0.8/Epate.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-04-26 18:22:12.000000 epate-1.0.8/Epate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-26 18:22:12.000000 epate-1.0.8/Epate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 18:22:12.000000 epate-1.0.8/Epate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-26 18:22:12.000000 epate-1.0.8/Epate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-26 18:22:12.000000 epate-1.0.8/Epate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 18:22:12.000000 epate-1.0.8/Epate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      562 2024-04-26 18:22:12.790504 epate-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 18:22:12.795508 epate-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      901 2024-04-26 18:21:59.000000 epate-1.0.8/setup.py
```

### Comparing `epate-1.0.7/Epate/__init__.py` & `epate-1.0.8/Epate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 class epate:
     def login(username,password,print='no'):
         session = requests.Session()
         login_data = {'pid': '65edCTyg',
                 'identity': username,
                 'password': password}
         result = session.post('https://api.codemao.cn/tiger/v3/web/accounts/login', json=login_data)
-        code = int(result.status_code)
+        code = str(result.status_code)
         def get():
             return(result.text)
 
-        if code == 201:
+        if code == '201':
             if print == 'yes':
                 print("Login Successful[201]")
             else:
                 return('201')
         else:
             if print == 'yes':
                 print("Login Failed["+ str(code)+"]")
```

### Comparing `epate-1.0.7/Epate.egg-info/PKG-INFO` & `epate-1.0.8/Epate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.7/LICENSE` & `epate-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `epate-1.0.7/PKG-INFO` & `epate-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.7/setup.py` & `epate-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  
 from pkg_resources import parse_requirements
 
 install_requires = ['requests==2.31.0']
  
 setup(
     name="Epate",
-    version="1.0.7",
+    version="1.0.8",
     author="xiaoxlh",
     author_email="xiaoxiaogzs@outlook.com",
     description="A python library for many API of the codemao's website.",
     long_description="eds sdk for python",
     license="Apache License, Version 2.0",
     url="https://xiao.asia",
```


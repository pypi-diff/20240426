# Comparing `tmp/epate-1.0.5.tar.gz` & `tmp/epate-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epate-1.0.5.tar", last modified: Fri Apr 26 18:07:00 2024, max compression
+gzip compressed data, was "epate-1.0.6.tar", last modified: Fri Apr 26 18:12:01 2024, max compression
```

## Comparing `epate-1.0.5.tar` & `epate-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 18:07:00.819821 epate-1.0.5/
-drwxrwxrwx   0        0        0        0 2024-04-26 18:07:00.781436 epate-1.0.5/Epate/
--rw-rw-rw-   0        0        0     5577 2024-04-26 18:06:33.000000 epate-1.0.5/Epate/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 17:50:18.000000 epate-1.0.5/Epate/epate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:07:00.814075 epate-1.0.5/Epate.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-26 18:07:00.000000 epate-1.0.5/Epate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-26 18:07:00.000000 epate-1.0.5/Epate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 18:07:00.000000 epate-1.0.5/Epate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-26 18:07:00.000000 epate-1.0.5/Epate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 18:07:00.000000 epate-1.0.5/Epate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 18:07:00.000000 epate-1.0.5/Epate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      562 2024-04-26 18:07:00.816065 epate-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 18:07:00.819821 epate-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      901 2024-04-26 18:06:45.000000 epate-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:12:01.653948 epate-1.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-26 18:12:01.616961 epate-1.0.6/Epate/
+-rw-rw-rw-   0        0        0     5579 2024-04-26 18:10:59.000000 epate-1.0.6/Epate/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:50:18.000000 epate-1.0.6/Epate/epate.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:12:01.648383 epate-1.0.6/Epate.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      562 2024-04-26 18:12:01.650284 epate-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 18:12:01.653948 epate-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      901 2024-04-26 18:11:06.000000 epate-1.0.6/setup.py
```

### Comparing `epate-1.0.5/Epate/__init__.py` & `epate-1.0.6/Epate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 class epate:
     def login(username:str,password:str,print:str='no'):
         session = requests.Session()
         login_data = {'pid': '65edCTyg',
                 'identity': username,
                 'password': password}
         result = session.post('https://api.codemao.cn/tiger/v3/web/accounts/login', json=login_data)
-
+        code = int(result.status_code)
         def get():
             return(result.text)
 
-        if result.status_code == 201:
+        if code == 201:
             if print == 'yes':
                 print("Login Successful[201]")
             else:
                 return('201')
         else:
             if print == 'yes':
-                print("Login Failed["+result.status_code+"]")
+                print("Login Failed["+ str(code)+"]")
             else:
-                return(result.status_code)
+                return(code)
                
     def logout(print:str='no'):
         session = requests.Session()
         result = session.post('https://api.codemao.cn/tiger/v3/web/accounts/loginout')
 
         def get():
             return(result.text())
```

### Comparing `epate-1.0.5/Epate.egg-info/PKG-INFO` & `epate-1.0.6/Epate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.5/LICENSE` & `epate-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `epate-1.0.5/PKG-INFO` & `epate-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.5/setup.py` & `epate-1.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  
 from pkg_resources import parse_requirements
 
 install_requires = ['requests==2.31.0']
  
 setup(
     name="Epate",
-    version="1.0.5",
+    version="1.0.6",
     author="xiaoxlh",
     author_email="xiaoxiaogzs@outlook.com",
     description="A python library for many API of the codemao's website.",
     long_description="eds sdk for python",
     license="Apache License, Version 2.0",
     url="https://xiao.asia",
```


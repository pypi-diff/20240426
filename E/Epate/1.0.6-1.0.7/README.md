# Comparing `tmp/epate-1.0.6.tar.gz` & `tmp/epate-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epate-1.0.6.tar", last modified: Fri Apr 26 18:12:01 2024, max compression
+gzip compressed data, was "epate-1.0.7.tar", last modified: Fri Apr 26 18:15:56 2024, max compression
```

## Comparing `epate-1.0.6.tar` & `epate-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 18:12:01.653948 epate-1.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-26 18:12:01.616961 epate-1.0.6/Epate/
--rw-rw-rw-   0        0        0     5579 2024-04-26 18:10:59.000000 epate-1.0.6/Epate/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 17:50:18.000000 epate-1.0.6/Epate/epate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:12:01.648383 epate-1.0.6/Epate.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 18:12:01.000000 epate-1.0.6/Epate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      562 2024-04-26 18:12:01.650284 epate-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 18:12:01.653948 epate-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      901 2024-04-26 18:11:06.000000 epate-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:15:56.697060 epate-1.0.7/
+drwxrwxrwx   0        0        0        0 2024-04-26 18:15:56.659959 epate-1.0.7/Epate/
+-rw-rw-rw-   0        0        0     5503 2024-04-26 18:15:42.000000 epate-1.0.7/Epate/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:50:18.000000 epate-1.0.7/Epate/epate.py
+drwxrwxrwx   0        0        0        0 2024-04-26 18:15:56.690680 epate-1.0.7/Epate.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 18:15:56.000000 epate-1.0.7/Epate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-26 15:22:07.000000 epate-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      562 2024-04-26 18:15:56.691677 epate-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2024-04-26 15:22:07.000000 epate-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 18:15:56.697060 epate-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      901 2024-04-26 18:15:47.000000 epate-1.0.7/setup.py
```

### Comparing `epate-1.0.6/Epate/__init__.py` & `epate-1.0.7/Epate/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
 class epate:
-    def login(username:str,password:str,print:str='no'):
+    def login(username,password,print='no'):
         session = requests.Session()
         login_data = {'pid': '65edCTyg',
                 'identity': username,
                 'password': password}
         result = session.post('https://api.codemao.cn/tiger/v3/web/accounts/login', json=login_data)
         code = int(result.status_code)
         def get():
@@ -18,33 +18,33 @@
                 return('201')
         else:
             if print == 'yes':
                 print("Login Failed["+ str(code)+"]")
             else:
                 return(code)
                
-    def logout(print:str='no'):
+    def logout(print='no'):
         session = requests.Session()
         result = session.post('https://api.codemao.cn/tiger/v3/web/accounts/loginout')
 
         def get():
-            return(result.text())
+            return(result.text)
 
         if result.status_code == 200:
             if print == 'yes':
                 print("Logout Successful[204]")
             else:
                 return('204')
         else:
             if print == 'yes':
                 print("Logout Failed["+str(result.status_code)+"]")
             else:
                 return(str(result.status_code))
             
-    def usrinfo(kind:str,inputstr:str,inputint:int,print:str='no'):
+    def usrinfo(kind,inputstr,inputint:int,print='no'):
         if kind == 'nick':
             session = requests.Session()
             change = {'nickname':inputstr}
             result = session.patch("/tiger/v3/web/accounts/info",data=change)
         
         if kind == 'full':
             session = requests.Session()
@@ -68,87 +68,87 @@
 
         if kind == 'avat':
             session = requests.Session()
             change = {'avatar_url':inputstr}
             result = session.patch("/tiger/v3/web/accounts/info",data=change)
 
         def get():
-                return(result.text())    
+                return(result.text)    
             
         if result.status_code == 204:
             if print == 'yes':
                 print("Change Info Successful[204]")
             else:
                 return('204')
         else:
             if print == 'yes':
                 print("Change Info Failed["+str(result.status_code)+"]")
             else:
                 return(str(result.status_code))
                 
-    def psc(old_password:str,new_password:str,print:str='no'):
+    def psc(old_password,new_password,print='no'):
         session = requests.Session()
         change = {'old_password':old_password,'password':new_password,'confirm_password':new_password}
         result = session.patch("/tiger/v3/web/accounts/info",data=change)
         def get():
-                return(result.text())    
+                return(result.text)    
             
         if result.status_code == 204:
             if print == 'yes':
                 print("Change Password Successful[204]")
             else:
                 return('204')
         else:
             if print == 'yes':
                 print("Change Password Failed["+str(result.status_code)+"]")
             else:
                 return(str(result.status_code))
 
-    def like(workid:str,print:str='no'):
+    def like(workid,print='no'):
         session = requests.Session()
         result = session.post("https://api.codemao.cn/nemo/v2/works/" + workid +"/like")
 
         def get():
-            return(result.text())
+            return(result.text)
 
         if result.status_code == 201:
             if print == 'yes':
                 print("Like Successful[201]")
             else:
                 return('201')
         else:
             if print == 'yes':
                 print("Like Failed["+str(result.status_code)+"]")
             else:
                 return(str(result.status_code))
 
-    def coll(workid:str,print:str='no'):
+    def coll(workid,print='no'):
         session = requests.Session()
         result = session.post("https://api.codemao.cn/nemo/v2/works/" + workid +"/collection")
         
         def get():
-            return(result.text())
+            return(result.text)
         
         if result.status_code == 201:
             if print == 'yes':
                 print("Collection Successful[201]")
             else:
                 return('201')
         else:
             if print == 'yes':
                 print("Collection Failed["+str(result.status_code)+"]")
             else:
                 return(str(result.status_code))
             
-    def fork(workid:str,print:str='no'):
+    def fork(workid,print='no'):
         session = requests.Session()
         result = session.post("https://api.codemao.cn/nemo/v2/works/" + workid +"/fork")
 
         def get():
-            return(result.text())
+            return(result.text)
 
         if result.status_code == 201:
             if print == 'yes':
                 print("Fork Successful[201]")
             else:
                 return('201')
         else:
```

### Comparing `epate-1.0.6/Epate.egg-info/PKG-INFO` & `epate-1.0.7/Epate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.6/LICENSE` & `epate-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `epate-1.0.6/PKG-INFO` & `epate-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Epate
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python library for many API of the codemao's website.
 Home-page: https://xiao.asia
 Author: xiaoxlh
 Author-email: xiaoxiaogzs@outlook.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `epate-1.0.6/setup.py` & `epate-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  
 from pkg_resources import parse_requirements
 
 install_requires = ['requests==2.31.0']
  
 setup(
     name="Epate",
-    version="1.0.6",
+    version="1.0.7",
     author="xiaoxlh",
     author_email="xiaoxiaogzs@outlook.com",
     description="A python library for many API of the codemao's website.",
     long_description="eds sdk for python",
     license="Apache License, Version 2.0",
     url="https://xiao.asia",
```


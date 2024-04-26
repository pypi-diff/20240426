# Comparing `tmp/glpic-99.0.202404260848.tar.gz` & `tmp/glpic-99.0.202404260851.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202404260848.tar", last modified: Fri Apr 26 08:48:45 2024, max compression
+gzip compressed data, was "glpic-99.0.202404260851.tar", last modified: Fri Apr 26 08:51:23 2024, max compression
```

## Comparing `glpic-99.0.202404260848.tar` & `glpic-99.0.202404260851.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-26 08:48:30.000000 glpic-99.0.202404260848/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-04-26 08:48:30.000000 glpic-99.0.202404260848/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-04-26 08:48:30.000000 glpic-99.0.202404260848/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 08:48:45.000000 glpic-99.0.202404260848/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:48:45.346756 glpic-99.0.202404260848/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-26 08:48:44.000000 glpic-99.0.202404260848/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:51:23.786733 glpic-99.0.202404260851/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-26 08:51:23.786733 glpic-99.0.202404260851/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-26 08:51:10.000000 glpic-99.0.202404260851/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:51:23.786733 glpic-99.0.202404260851/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-26 08:51:10.000000 glpic-99.0.202404260851/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-04-26 08:51:10.000000 glpic-99.0.202404260851/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:51:23.786733 glpic-99.0.202404260851/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-26 08:51:23.000000 glpic-99.0.202404260851/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 08:51:23.000000 glpic-99.0.202404260851/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:51:23.000000 glpic-99.0.202404260851/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 08:51:23.000000 glpic-99.0.202404260851/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:51:23.000000 glpic-99.0.202404260851/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 08:51:23.000000 glpic-99.0.202404260851/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 08:51:23.000000 glpic-99.0.202404260851/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:51:23.786733 glpic-99.0.202404260851/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-26 08:51:23.000000 glpic-99.0.202404260851/setup.py
```

### Comparing `glpic-99.0.202404260848/README.md` & `glpic-99.0.202404260851/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404260848/glpic/__init__.py` & `glpic-99.0.202404260851/glpic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,18 +120,20 @@
         self.base_url = base_url
         self.user = user
         ssl._create_default_https_context = ssl._create_unverified_context
         headers = {'Content-Type': 'application/json', 'Authorization': f"user_token {api_token}"}
         response = _get(f'{base_url}/initSession?get_full_session=true', headers)
         self.headers = {'Content-Type': 'application/json', "Session-Token": response['session_token']}
 
-    def get_user(self, user):
+    def get_user(self, user=None):
+        if user is None:
+            user = self.user
         users = _get(f'{self.base_url}/User', headers=self.headers)
         for u in users:
-            if self.user in u['name']:
+            if user in u['name']:
                 return u
 
     def info_computer(self, computer, full=False):
         computers = _get(f'{self.base_url}/Computer?with_devices', headers=self.headers)
         if not str(computer).isnumeric():
             computers = [c for c in _get(f'{self.base_url}/Computer?with_devices',
                                          headers=self.headers) if c['name'].strip() == computer]
```

### Comparing `glpic-99.0.202404260848/glpic/cli.py` & `glpic-99.0.202404260851/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404260848/setup.py` & `glpic-99.0.202404260851/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202404260848',
+    version='99.0.202404260851',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```


# Comparing `tmp/glpic-99.0.202404252110.tar.gz` & `tmp/glpic-99.0.202404252200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202404252110.tar", last modified: Thu Apr 25 21:10:15 2024, max compression
+gzip compressed data, was "glpic-99.0.202404252200.tar", last modified: Thu Apr 25 22:00:46 2024, max compression
```

## Comparing `glpic-99.0.202404252110.tar` & `glpic-99.0.202404252200.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:10:15.119790 glpic-99.0.202404252110/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:10:15.119790 glpic-99.0.202404252110/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 21:10:02.000000 glpic-99.0.202404252110/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:10:15.119790 glpic-99.0.202404252110/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-25 21:10:02.000000 glpic-99.0.202404252110/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-25 21:10:02.000000 glpic-99.0.202404252110/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:10:15.119790 glpic-99.0.202404252110/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 21:10:15.000000 glpic-99.0.202404252110/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 21:10:15.000000 glpic-99.0.202404252110/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:10:15.000000 glpic-99.0.202404252110/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 21:10:15.000000 glpic-99.0.202404252110/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:10:15.000000 glpic-99.0.202404252110/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 21:10:15.000000 glpic-99.0.202404252110/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 21:10:15.000000 glpic-99.0.202404252110/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:10:15.119790 glpic-99.0.202404252110/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 21:10:14.000000 glpic-99.0.202404252110/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 22:00:33.000000 glpic-99.0.202404252200/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-25 22:00:33.000000 glpic-99.0.202404252200/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-25 22:00:33.000000 glpic-99.0.202404252200/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 22:00:46.000000 glpic-99.0.202404252200/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 22:00:46.385367 glpic-99.0.202404252200/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 22:00:45.000000 glpic-99.0.202404252200/setup.py
```

### Comparing `glpic-99.0.202404252110/README.md` & `glpic-99.0.202404252200/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404252110/glpic/__init__.py` & `glpic-99.0.202404252200/glpic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,50 +53,50 @@
 
 
 def _delete(url, headers):
     request = Request(url, headers=headers, method='DELETE')
     try:
         return urlopen(request)
     except Exception as e:
-        error(e)
+        error(e.read().decode())
 
 
 def _get(url, headers):
     if not os.path.basename(url).split('?')[0].isnumeric():
         encoded_params = urlencode({"range": '0-9999'})
         delimiter = '&' if '?' in url else '?'
         url += f'{delimiter}{encoded_params}'
     try:
         return json.loads(urlopen(Request(url, headers=headers)).read())
     except Exception as e:
-        error(e)
+        error(e.read().decode())
 
 
 def _patch(url, headers, data):
     data = json.dumps(data).encode('utf-8')
     try:
         return urlopen(Request(url, data=data, headers=headers, method='PATCH'))
     except Exception as e:
-        error(e)
+        error(e.read().decode())
 
 
 def _post(url, headers, data):
     data = json.dumps(data).encode('utf-8')
     try:
         return urlopen(Request(url, data=data, headers=headers, method='POST'))
     except Exception as e:
-        error(e)
+        error(e.read().decode())
 
 
 def _put(url, headers, data):
     data = json.dumps(data).encode('utf-8')
     try:
         return urlopen(Request(url, data=data, headers=headers, method='PUT'))
     except Exception as e:
-        error(e)
+        error(e.read().decode())
 
 
 def error(text):
     color = "31"
     print(f'\033[0;{color}m{text}\033[0;0m')
```

### Comparing `glpic-99.0.202404252110/glpic/cli.py` & `glpic-99.0.202404252200/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404252110/setup.py` & `glpic-99.0.202404252200/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202404252110',
+    version='99.0.202404252200',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```


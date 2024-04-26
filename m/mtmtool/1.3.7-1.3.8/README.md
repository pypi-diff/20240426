# Comparing `tmp/mtmtool-1.3.7.tar.gz` & `tmp/mtmtool-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmtool-1.3.7.tar", last modified: Tue Jan  9 08:52:53 2024, max compression
+gzip compressed data, was "mtmtool-1.3.8.tar", last modified: Fri Apr 26 17:15:31 2024, max compression
```

## Comparing `mtmtool-1.3.7.tar` & `mtmtool-1.3.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:52:53.480002 mtmtool-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-09 08:52:42.000000 mtmtool-1.3.7/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:52:53.476002 mtmtool-1.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:52:53.476002 mtmtool-1.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-09 08:52:42.000000 mtmtool-1.3.7/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-01-09 08:52:42.000000 mtmtool-1.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-01-09 08:52:42.000000 mtmtool-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-09 08:52:42.000000 mtmtool-1.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-01-09 08:52:53.480002 mtmtool-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-09 08:52:42.000000 mtmtool-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:52:53.476002 mtmtool-1.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-01-09 08:52:42.000000 mtmtool-1.3.7/docs/Python装饰器之函数池化.md
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-01-09 08:52:42.000000 mtmtool-1.3.7/docs/Python装饰器原理浅见.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-09 08:52:42.000000 mtmtool-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 08:52:53.480002 mtmtool-1.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:52:53.476002 mtmtool-1.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:52:53.480002 mtmtool-1.3.7/src/mtmtool/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-09 08:52:42.000000 mtmtool-1.3.7/src/mtmtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15704 2024-01-09 08:52:42.000000 mtmtool-1.3.7/src/mtmtool/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-09 08:52:42.000000 mtmtool-1.3.7/src/mtmtool/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-09 08:52:42.000000 mtmtool-1.3.7/src/mtmtool/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-01-09 08:52:42.000000 mtmtool-1.3.7/src/mtmtool/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-01-09 08:52:42.000000 mtmtool-1.3.7/src/mtmtool/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-01-09 08:52:42.000000 mtmtool-1.3.7/src/mtmtool/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-01-09 08:52:42.000000 mtmtool-1.3.7/src/mtmtool/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:52:53.480002 mtmtool-1.3.7/src/mtmtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-01-09 08:52:53.000000 mtmtool-1.3.7/src/mtmtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-09 08:52:53.000000 mtmtool-1.3.7/src/mtmtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 08:52:53.000000 mtmtool-1.3.7/src/mtmtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-09 08:52:53.000000 mtmtool-1.3.7/src/mtmtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-09 08:52:53.000000 mtmtool-1.3.7/src/mtmtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 08:52:53.480002 mtmtool-1.3.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-09 08:52:42.000000 mtmtool-1.3.7/test/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-09 08:52:42.000000 mtmtool-1.3.7/test/test_download_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-01-09 08:52:42.000000 mtmtool-1.3.7/test/test_map_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:15:31.377574 mtmtool-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 17:15:22.000000 mtmtool-1.3.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:15:31.369574 mtmtool-1.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:15:31.373574 mtmtool-1.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-26 17:15:22.000000 mtmtool-1.3.8/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-26 17:15:22.000000 mtmtool-1.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-26 17:15:22.000000 mtmtool-1.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-26 17:15:22.000000 mtmtool-1.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-04-26 17:15:31.373574 mtmtool-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 17:15:22.000000 mtmtool-1.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:15:31.373574 mtmtool-1.3.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-26 17:15:22.000000 mtmtool-1.3.8/docs/Python装饰器之函数池化.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-26 17:15:22.000000 mtmtool-1.3.8/docs/Python装饰器原理浅见.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-26 17:15:22.000000 mtmtool-1.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 17:15:31.377574 mtmtool-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:15:31.373574 mtmtool-1.3.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:15:31.373574 mtmtool-1.3.8/src/mtmtool/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-26 17:15:22.000000 mtmtool-1.3.8/src/mtmtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15704 2024-04-26 17:15:22.000000 mtmtool-1.3.8/src/mtmtool/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-26 17:15:22.000000 mtmtool-1.3.8/src/mtmtool/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-26 17:15:22.000000 mtmtool-1.3.8/src/mtmtool/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-26 17:15:22.000000 mtmtool-1.3.8/src/mtmtool/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-26 17:15:22.000000 mtmtool-1.3.8/src/mtmtool/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-26 17:15:22.000000 mtmtool-1.3.8/src/mtmtool/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-26 17:15:22.000000 mtmtool-1.3.8/src/mtmtool/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:15:31.373574 mtmtool-1.3.8/src/mtmtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-04-26 17:15:31.000000 mtmtool-1.3.8/src/mtmtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-26 17:15:31.000000 mtmtool-1.3.8/src/mtmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:15:31.000000 mtmtool-1.3.8/src/mtmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 17:15:31.000000 mtmtool-1.3.8/src/mtmtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 17:15:31.000000 mtmtool-1.3.8/src/mtmtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:15:31.373574 mtmtool-1.3.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-26 17:15:22.000000 mtmtool-1.3.8/test/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-26 17:15:22.000000 mtmtool-1.3.8/test/test_download_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-26 17:15:22.000000 mtmtool-1.3.8/test/test_map_pool.py
```

### Comparing `mtmtool-1.3.7/.github/workflows/publish-to-test-pypi.yml` & `mtmtool-1.3.8/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/.gitignore` & `mtmtool-1.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/LICENSE` & `mtmtool-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/PKG-INFO` & `mtmtool-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.3.7
+Version: 1.3.8
 Summary: imutum's tool packages
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mtmtool-1.3.7/docs/Python装饰器之函数池化.md` & `mtmtool-1.3.8/docs/Python装饰器之函数池化.md`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/docs/Python装饰器原理浅见.md` & `mtmtool-1.3.8/docs/Python装饰器原理浅见.md`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/pyproject.toml` & `mtmtool-1.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/src/mtmtool/download.py` & `mtmtool-1.3.8/src/mtmtool/download.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/src/mtmtool/io.py` & `mtmtool-1.3.8/src/mtmtool/io.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/src/mtmtool/log.py` & `mtmtool-1.3.8/src/mtmtool/log.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/src/mtmtool/notify.py` & `mtmtool-1.3.8/src/mtmtool/notify.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,18 +28,25 @@
         kwargs["parse_mode"] = "HTML"
     # 消息格式
     data = {
         "chat_id": chat_id,
         "text": text,
         **kwargs,
     }
+    # 发送请求
+    response = None
     try:
-        response = requests.get(url, params=data)
-        return response.json()
-    except:
-        print(f"Telegram API response:\n {response.text}")
-        raise ValueError(f"Telegram API Error.")
+        response = requests.get(url, params=data, timeout=1)
+        resp_json = response.json()
+        return resp_json
+    except Exception as e:
+        if response is None:
+            print(f"Telegram API response ({text}): {e} ")
+        else:
+            print(f"Telegram API response ({text}): {e} -> {response.text}")
+        if kwargs.get("raise_error", True):
+            raise ValueError(f"Telegram API Error. {e}")
 
 
 def pushplus(message, token, title="default", template="html", **kwargs):
     url = f"http://www.pushplus.plus/send?token={token}&title={title}&content={message}&template={template}"
     return requests.get(url=url).text
```

### Comparing `mtmtool-1.3.7/src/mtmtool/path.py` & `mtmtool-1.3.8/src/mtmtool/path.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/src/mtmtool/pool.py` & `mtmtool-1.3.8/src/mtmtool/pool.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/src/mtmtool/time.py` & `mtmtool-1.3.8/src/mtmtool/time.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/src/mtmtool.egg-info/PKG-INFO` & `mtmtool-1.3.8/src/mtmtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtmtool
-Version: 1.3.7
+Version: 1.3.8
 Summary: imutum's tool packages
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mtmtool-1.3.7/src/mtmtool.egg-info/SOURCES.txt` & `mtmtool-1.3.8/src/mtmtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtmtool-1.3.7/test/test_map_pool.py` & `mtmtool-1.3.8/test/test_map_pool.py`

 * *Files identical despite different names*


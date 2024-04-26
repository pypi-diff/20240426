# Comparing `tmp/pyhasura-1.0.7.tar.gz` & `tmp/pyhasura-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhasura-1.0.7.tar", last modified: Fri Apr 26 02:26:21 2024, max compression
+gzip compressed data, was "pyhasura-1.0.8.tar", last modified: Fri Apr 26 02:44:55 2024, max compression
```

## Comparing `pyhasura-1.0.7.tar` & `pyhasura-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:26:21.253955 pyhasura-1.0.7/
--rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.7/LICENSE
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 02:26:21.253734 pyhasura-1.0.7/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.7/README.md
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:26:21.252958 pyhasura-1.0.7/pyhasura/
--rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.7/pyhasura/__init__.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.7/pyhasura/flatten_dict.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.7/pyhasura/gql_client.py
--rw-r--r--   0 kennethstott   (501) staff       (20)    14654 2024-04-26 02:26:16.000000 pyhasura-1.0.7/pyhasura/hasura_client.py
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:26:21.253515 pyhasura-1.0.7/pyhasura.egg-info/
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/SOURCES.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/dependency_links.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/requires.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/top_level.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.7/pyproject.toml
--rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-26 02:26:21.254000 pyhasura-1.0.7/setup.cfg
--rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.7/setup.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:44:55.340172 pyhasura-1.0.8/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.8/LICENSE
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 02:44:55.339960 pyhasura-1.0.8/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.8/README.md
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:44:55.339155 pyhasura-1.0.8/pyhasura/
+-rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.8/pyhasura/__init__.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.8/pyhasura/flatten_dict.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.8/pyhasura/gql_client.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)    14675 2024-04-26 02:44:41.000000 pyhasura-1.0.8/pyhasura/hasura_client.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:44:55.339721 pyhasura-1.0.8/pyhasura.egg-info/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/SOURCES.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/dependency_links.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/requires.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-26 02:44:55.000000 pyhasura-1.0.8/pyhasura.egg-info/top_level.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.8/pyproject.toml
+-rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-26 02:44:55.340212 pyhasura-1.0.8/setup.cfg
+-rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.8/setup.py
```

### Comparing `pyhasura-1.0.7/LICENSE` & `pyhasura-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.7/PKG-INFO` & `pyhasura-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.7/README.md` & `pyhasura-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.7/pyhasura/flatten_dict.py` & `pyhasura-1.0.8/pyhasura/flatten_dict.py`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.7/pyhasura/hasura_client.py` & `pyhasura-1.0.8/pyhasura/hasura_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,16 +281,16 @@
         clf = IsolationForest(contamination=0.1, random_state=42)
         for key in self.vectorized_result:
             if training_files is not None:
                 with open(training_files[key], 'rb') as model_file:
                     clf = pickle.load(model_file)
             elif training_base64 is not None:
                 clf = pickle.loads(base64.b64decode(training_base64[key]))
-
-            clf.fit(self.vectorized_result[key])
+            else:
+                clf.fit(self.vectorized_result[key])
             scores = clf.decision_function(self.vectorized_result[key])
             merged = list(map(lambda x: add_score(self.native_result[key][x[0]], x[0], x[1]), enumerate(scores)))
             self.anomalies_result[key] = list(filter(lambda x: x['__score__'] < threshold, merged))
         return self.anomalies_result
 
     def convert_output_format(self, output_format):
         """
```

### Comparing `pyhasura-1.0.7/pyhasura.egg-info/PKG-INFO` & `pyhasura-1.0.8/pyhasura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.7/pyproject.toml` & `pyhasura-1.0.8/pyproject.toml`

 * *Files identical despite different names*


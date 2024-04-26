# Comparing `tmp/pyhasura-1.0.6.tar.gz` & `tmp/pyhasura-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhasura-1.0.6.tar", last modified: Thu Apr 25 20:32:55 2024, max compression
+gzip compressed data, was "pyhasura-1.0.7.tar", last modified: Fri Apr 26 02:26:21 2024, max compression
```

## Comparing `pyhasura-1.0.6.tar` & `pyhasura-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:32:55.414354 pyhasura-1.0.6/
--rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.6/LICENSE
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 20:32:55.414148 pyhasura-1.0.6/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.6/README.md
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:32:55.413232 pyhasura-1.0.6/pyhasura/
--rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.6/pyhasura/__init__.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.6/pyhasura/flatten_dict.py
--rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.6/pyhasura/gql_client.py
--rw-r--r--   0 kennethstott   (501) staff       (20)    13578 2024-04-25 20:32:42.000000 pyhasura-1.0.6/pyhasura/hasura_client.py
-drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-25 20:32:55.413908 pyhasura-1.0.6/pyhasura.egg-info/
--rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/PKG-INFO
--rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/SOURCES.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/dependency_links.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/requires.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-25 20:32:55.000000 pyhasura-1.0.6/pyhasura.egg-info/top_level.txt
--rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.6/pyproject.toml
--rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-25 20:32:55.414395 pyhasura-1.0.6/setup.cfg
--rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.6/setup.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:26:21.253955 pyhasura-1.0.7/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     1065 2024-04-20 12:02:03.000000 pyhasura-1.0.7/LICENSE
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 02:26:21.253734 pyhasura-1.0.7/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)     2967 2024-04-19 21:24:41.000000 pyhasura-1.0.7/README.md
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:26:21.252958 pyhasura-1.0.7/pyhasura/
+-rw-r--r--   0 kennethstott   (501) staff       (20)      136 2024-04-19 18:25:03.000000 pyhasura-1.0.7/pyhasura/__init__.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      745 2024-04-19 10:52:53.000000 pyhasura-1.0.7/pyhasura/flatten_dict.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)      359 2024-04-20 12:07:08.000000 pyhasura-1.0.7/pyhasura/gql_client.py
+-rw-r--r--   0 kennethstott   (501) staff       (20)    14654 2024-04-26 02:26:16.000000 pyhasura-1.0.7/pyhasura/hasura_client.py
+drwxr-xr-x   0 kennethstott   (501) staff       (20)        0 2024-04-26 02:26:21.253515 pyhasura-1.0.7/pyhasura.egg-info/
+-rw-r--r--   0 kennethstott   (501) staff       (20)     3545 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/PKG-INFO
+-rw-r--r--   0 kennethstott   (501) staff       (20)      295 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/SOURCES.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        1 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/dependency_links.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)       82 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/requires.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)        9 2024-04-26 02:26:21.000000 pyhasura-1.0.7/pyhasura.egg-info/top_level.txt
+-rw-r--r--   0 kennethstott   (501) staff       (20)      711 2024-04-20 12:50:35.000000 pyhasura-1.0.7/pyproject.toml
+-rw-r--r--   0 kennethstott   (501) staff       (20)       38 2024-04-26 02:26:21.254000 pyhasura-1.0.7/setup.cfg
+-rw-r--r--   0 kennethstott   (501) staff       (20)      427 2024-04-20 12:22:29.000000 pyhasura-1.0.7/setup.py
```

### Comparing `pyhasura-1.0.6/LICENSE` & `pyhasura-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.6/PKG-INFO` & `pyhasura-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.6/README.md` & `pyhasura-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.6/pyhasura/flatten_dict.py` & `pyhasura-1.0.7/pyhasura/flatten_dict.py`

 * *Files identical despite different names*

### Comparing `pyhasura-1.0.6/pyhasura/hasura_client.py` & `pyhasura-1.0.7/pyhasura/hasura_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,37 @@
 from gql import gql
 import pandas as pd
 from pyhasura import gql_client, flatten_nested_dicts
 import pyarrow as pa
 from sklearn.feature_extraction import DictVectorizer
 from sklearn.ensemble import IsolationForest
 from sklearn_extra.cluster import KMedoids
+import tempfile
+import base64
 
 
 class ExportFormat(Enum):
     FLAT = 1
     DATAFRAME = 2
     ARROW = 3
     NATURAL = 4
     PARQUET = 5
     CSV = 6
 
 
+def load_data_from_base64(base64_string):
+    # Decode the base64 string to bytes
+    binary_data = base64.b64decode(base64_string)
+
+    # Create a temporary file in memory
+    with tempfile.NamedTemporaryFile(delete=False) as temp_file:
+        temp_file.write(binary_data)
+        return temp_file.name
+
+
 def create_empty_arrays(n):
     return [[] for _ in range(n)]
 
 
 def compute_deltas(numbers):
     """
     Computes the deltas (differences) between consecutive elements in an array of numbers.
@@ -238,22 +250,27 @@
             clf.fit(self.vectorized_result[key])
             filename = os.path.join(self.output_dir, key + '.pkl')
             with open(filename, 'wb') as model_file:
                 pickle.dump(clf, model_file)
             filenames[key] = filename
         return filenames
 
-    def anomalies(self, training_files=None, threshold=0):
+    def anomalies(self, training_files=None, threshold=0, training_base64=None):
         """
-        Find anomalies in the data.
+        Args:
+            training_files: A dictionary containing the file paths of the training files for each key. If provided, the pre-trained isolation forest models will be loaded from these files.
+            threshold: A float value representing the threshold for anomaly detection. Only the anomalies with a score below this threshold will be included in the result. Defaults to 0 if not provided.
+            training_base64: A dictionary containing the base64-encoded serialized pre-trained isolation forest models for each key. If provided, the models will be deserialized and used for anomaly detection.
 
-        :param training_files: A dictionary of training file paths for each key in the vectorized result. If provided, the model will be loaded from the file before fitting. Default is None
-        *.
-        :param threshold: The threshold score below which a data point is considered an anomaly. Default is 0.
-        :return: A dictionary where each key corresponds to a category in the vectorized result, and the value is a list of anomalies with scores below the threshold.
+        Returns:
+            self.anomalies_result: A dictionary containing the anomalies found for each key. Each key maps to a list of dictionaries, where each dictionary represents an anomaly and contains the original item, its index, and the anomaly score.
+
+        Raises:
+            FileNotFoundError: If a training file specified in training_files does not exist.
+            KeyError: If a key in training_files or training_base64 does not exist in the keys of self.vectorized_result.
 
         """
 
         def add_score(item, index, score):
             item['__score__'] = score
             item['__index__'] = index
             return item
@@ -262,14 +279,17 @@
         self.vectorize_result()
         # Initialize Isolation Forest
         clf = IsolationForest(contamination=0.1, random_state=42)
         for key in self.vectorized_result:
             if training_files is not None:
                 with open(training_files[key], 'rb') as model_file:
                     clf = pickle.load(model_file)
+            elif training_base64 is not None:
+                clf = pickle.loads(base64.b64decode(training_base64[key]))
+
             clf.fit(self.vectorized_result[key])
             scores = clf.decision_function(self.vectorized_result[key])
             merged = list(map(lambda x: add_score(self.native_result[key][x[0]], x[0], x[1]), enumerate(scores)))
             self.anomalies_result[key] = list(filter(lambda x: x['__score__'] < threshold, merged))
         return self.anomalies_result
 
     def convert_output_format(self, output_format):
```

### Comparing `pyhasura-1.0.6/pyhasura.egg-info/PKG-INFO` & `pyhasura-1.0.7/pyhasura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhasura
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python library to simplify Hasura, GraphQL and Machine Learning
 Author-email: Kenneth Stott <ken@kenstott.com>
 Project-URL: repository, https://github.com/kenstott/pyhasura
 Keywords: graphql,hasura,ml,ai,machine learning,arrow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyhasura-1.0.6/pyproject.toml` & `pyhasura-1.0.7/pyproject.toml`

 * *Files identical despite different names*


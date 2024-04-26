# Comparing `tmp/vector_database-0.0.2.tar.gz` & `tmp/vector_database-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_database-0.0.2.tar", last modified: Fri Apr 26 08:44:10 2024, max compression
+gzip compressed data, was "vector_database-0.0.3.tar", last modified: Fri Apr 26 07:09:29 2024, max compression
```

## Comparing `vector_database-0.0.2.tar` & `vector_database-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 08:44:10.626463 vector_database-0.0.2/
--rw-rw-rw-   0        0        0     1089 2024-04-26 06:09:09.000000 vector_database-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1395 2024-04-26 08:44:10.626463 vector_database-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      444 2024-04-26 07:32:59.000000 vector_database-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 08:44:10.626463 vector_database-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-04-26 08:44:03.000000 vector_database-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:44:10.613319 vector_database-0.0.2/tests/
--rw-rw-rw-   0        0        0      469 2024-04-26 08:05:09.000000 vector_database-0.0.2/tests/test.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:44:10.614375 vector_database-0.0.2/vector_database/
--rw-rw-rw-   0        0        0       37 2024-04-25 08:37:46.000000 vector_database-0.0.2/vector_database/__init__.py
--rw-rw-rw-   0        0        0     7381 2024-04-26 08:04:45.000000 vector_database-0.0.2/vector_database/embedding.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:44:10.625463 vector_database-0.0.2/vector_database.egg-info/
--rw-rw-rw-   0        0        0     1395 2024-04-26 08:44:10.000000 vector_database-0.0.2/vector_database.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-04-26 08:44:10.000000 vector_database-0.0.2/vector_database.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 08:44:10.000000 vector_database-0.0.2/vector_database.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-26 08:44:10.000000 vector_database-0.0.2/vector_database.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-26 08:44:10.000000 vector_database-0.0.2/vector_database.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 07:09:29.859019 vector_database-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 06:09:09.000000 vector_database-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1168 2024-04-26 07:09:29.858017 vector_database-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-26 06:37:48.000000 vector_database-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-26 07:09:29.859692 vector_database-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2024-04-26 07:09:16.000000 vector_database-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:09:29.843906 vector_database-0.0.3/tests/
+-rw-rw-rw-   0        0        0      429 2024-04-26 06:37:34.000000 vector_database-0.0.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:09:29.845902 vector_database-0.0.3/vector_database/
+-rw-rw-rw-   0        0        0       37 2024-04-25 08:37:46.000000 vector_database-0.0.3/vector_database/__init__.py
+-rw-rw-rw-   0        0        0     5438 2024-04-26 06:07:49.000000 vector_database-0.0.3/vector_database/embedding.py
+drwxrwxrwx   0        0        0        0 2024-04-26 07:09:29.857895 vector_database-0.0.3/vector_database.egg-info/
+-rw-rw-rw-   0        0        0     1168 2024-04-26 07:09:29.000000 vector_database-0.0.3/vector_database.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-26 07:09:29.000000 vector_database-0.0.3/vector_database.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 07:09:29.000000 vector_database-0.0.3/vector_database.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-26 07:09:29.000000 vector_database-0.0.3/vector_database.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-26 07:09:29.000000 vector_database-0.0.3/vector_database.egg-info/top_level.txt
```

### Comparing `vector_database-0.0.2/LICENSE` & `vector_database-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_database-0.0.2/setup.py` & `vector_database-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import setup
 
 setup(
     name='vector_database',
-    version='0.0.2',
+    version='0.0.3',
     packages=['vector_database'],
     description='A tool to build vector database quickly',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jude Wang',
     author_email='pinkr1veroops@gmail.com',
     url='https://github.com/PinkR1ver/vector_database',
     license='MIT',
     keywords='vector database',
     install_requires=[
         'numpy',
         'pandas',
+        'tkinter >= 8.6',
         'torch',
         'torchvision',
-        'rich',
-        'opencv-python',
-        'sklearn',
+        'rich'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

### Comparing `vector_database-0.0.2/vector_database/embedding.py` & `vector_database-0.0.3/vector_database/embedding.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from torchvision import models
 from torchvision.io import read_image
 import os
 import pandas as pd
 from rich.progress import track
 import tkinter as tk
 from tkinter import filedialog
-from sklearn.cluster import KMeans
 import cv2
 import matplotlib.pyplot as plt
 
 class ImageEmbedding:
     
     def __init__(self, model_name_list: list = ['resnet50', 'SwinTransfomer', 'VisionTransfomer']):
         self.model_name_list = model_name_list
@@ -65,15 +64,15 @@
             
             vector = model(image)
             embed_vector = np.concatenate((embed_vector, vector.detach().numpy().flatten()))
             
         return embed_vector / np.linalg.norm(embed_vector)
     
     
-    def imageVectorDatabaseBuild(self, image_folder_path, save_base_path='.', save_database_name='image_vector_database.json', save_cluster_name='cluster_info.json' ,cluster_num=10):
+    def imageVectorDatabaseBuild(self, image_folder_path, database_path='.'):
     
         database_size = 0
         
         for root, dirs, files in track(os.walk(image_folder_path), description='Checking Vector Database Size...'):
             for file in files:
                 
                 if file.endswith('.png') or file.endswith('.jpg') or file.endswith('.jpeg') or file.endswith('.JPG'):
@@ -95,53 +94,24 @@
                     image_path = os.path.join(root, file)
                     embed_vector = self.imageEmbedding(image_path)
                     
                     database.loc[index, 'image_path'] = image_path
                     database.loc[index, 'embedding_vector'] = embed_vector
                     index += 1
         
-        database.to_json(os.path.join(save_base_path, save_database_name))
-        self.database_path = os.path.join(save_base_path, save_database_name)
+        database.to_json(database_path + '/image_vector_database.json')
+        self.database_path = database_path + '/image_vector_database.json'
         self.database = database
-        self.clusterDatabase(save_base_path, save_cluster_name, cluster_num)
-        
-    def clusterDatabase(self, save_base_path='.', save_cluster_name='cluster_info.json' ,cluster_num=10):
-        
-        kmeans = KMeans(n_clusters=cluster_num)
-        kmeans.fit(list(self.database['embedding_vector']))
-        
-        cluster_centers = kmeans.cluster_centers_
-        cluster_labels = kmeans.labels_
-        cluster_index = [_ for _ in range(cluster_num)]
-        for i in range(cluster_num):
-            cluster_index[i] = np.where(cluster_labels == i)
-        
-        cluster = pd.DataFrame(columns=['cluster_center', 'cluster_index'])
-        cluster['cluster_center'] = cluster_centers.tolist()
-        cluster['cluster_index'] = cluster_index
-        cluster.to_json(os.path.join(save_base_path, save_cluster_name))
-        
-        self.cluster = cluster
     
-    def imageVectorDatabaseLoad(self, database_path, cluster_path=None):
+    def imageVectorDatabaseLoad(self, database_path):
         
         database = pd.read_json(database_path)
         self.database = database
         self.database_size = len(database)
         self.database_path = database_path
-        
-        if cluster_path is not None:
-            cluster = pd.read_json(cluster_path)
-            self.cluster = cluster
-            
-        else:
-            save_path = database_path.split('/')
-            save_path.pop()
-            save_path = '/'.join(save_path)
-            self.clusterDatabase(save_path, 'cluster_info.json', 10)
       
     
     def imageQuery(self):
         
         if self.database_size == 0:
             print('Database is empty. Please build the database first.')
             return
@@ -157,38 +127,25 @@
         
         root.destroy()
         
         smallest_distance = -1
 
         
         query_vector = self.imageEmbedding(file_path)
-        
-        for index, center in enumerate(self.cluster['cluster_center']):
-            
-            distance = np.linalg.norm(query_vector - np.array(center))
+        for index, row in self.database.iterrows():
             
-            if smallest_distance == -1:
-                smallest_distance = distance
-                smallest_index = index
-            elif distance < smallest_distance:
-                smallest_distance = distance
-                smallest_index = index
-                
-        cluster_index = self.cluster.loc[smallest_index, 'cluster_index']
-        smallest_distance= -1
-        
-        for index in cluster_index[0]:
-            distance = np.linalg.norm(query_vector - self.database.loc[index, 'embedding_vector'])
+            distance = np.linalg.norm(query_vector - row['embedding_vector'])
             
             if smallest_distance == -1:
                 smallest_distance = distance
                 smallest_index = index
             elif distance < smallest_distance:
                 smallest_distance = distance
                 smallest_index = index
         
         image = cv2.imread(self.database.loc[smallest_index, 'image_path'])
         image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
         plt.imshow(image)
         plt.show()
+        input('Press Enter to Exit...')
```

